# ControlNet 1.1 模型全览：一篇看懂所有控制方式

ControlNet 1.1 把多种条件控制整合成一套模型。下面按控制类型梳理各模型的训练来源、可用预处理器、实测提示和注意事项；文中测试均固定种子 12345，且为未精挑的批量结果。

**深度控制**
训练数据由 Midas Depth、Leres Depth、Zoe Depth 三路组成，每路分辨率均为 256/384/512；多分辨率深度图生成器用于数据增强。可用预处理器为 Depth_Midas、Depth_Leres、Depth_Zoe。该模型稳定性强，渲染引擎输出的真实深度图也能处理。种子 12345、提示词“a handsome man”的未挑图批量测试：[PRE0]

**Normal 法线**
以法线贴图作为条件驱动 SD 出图。权重为 control_v11p_sd15_normalbae.pth，配置为 control_v11p_sd15_normalbae.yaml，训练来源是 Bae 的法线图估计方法。可用预处理器为普通 BAE。只要法线贴图符合 ScanNet 协议，渲染引擎产生的法线贴图也能被接受；颜色风格应接近示例图第二列。该方法比 ControlNet 1.1 里的 normal-from-midas 更合理，旧方案将被淘汰。种子 12345、提示词“a man made of flowers”：[PRE1]
种子 12345、提示词“room”：[PRE2]

**Canny 边缘检测**
用 Canny 预处理器先提取边缘，再据此控制 SD 生成图像。权重为 control_v11p_sd15_canny.pth，配置为 control_v11p_sd15_canny.yaml；训练数据是随机阈值下的 Canny。可用预处理器为 Canny。种子 12345、提示词“dog in a room”：[PRE3]

**MLSD 直线图**
以 M-LSD 直线作为控制条件，主要捕捉直线结构，室内设计场景常用。权重为 control_v11p_sd15_mlsd.pth，配置为 control_v11p_sd15_mlsd.yaml；训练数据为 M-LSD 线。可用预处理器为 MLSD。种子 12345、提示词“room”。

**Scribble 涂鸦**
用涂鸦控制 SD：既可用下方列出的预处理器，也可手绘粗线条涂鸦来生成图像。权重为 control_v11p_sd15_scribble.pth，配置为 control_v11p_sd15_scribble.yaml；训练数据为合成涂鸦。可用预处理器包括合成涂鸦（Scribble_HED、Scribble_PIDI 等）或手绘涂鸦。种子 12345、提示词“man in library”：[PRE4]
另用种子 12345，并加入描述词 the beautiful landscape：[PRE5]

**Soft Edge 软边缘**
以软边（粗线条线稿）控制 SD。权重为 control_v11p_sd15_softedge.pth，配置为 control_v11p_sd15_softedge.yaml；训练数据包括 SoftEdge_PIDI、SoftEdge_PIDI_safe、SoftEdge_HED、SoftEdge_HED_safe，可用预处理器也是这四类。该模型较旧版提升明显，建议所有用户尽快更新。ControlNet 1.1 新增“SoftEdge_safe”：HED 或 PIDI 容易在软边缘估计中藏入原图的损坏灰度版本，这种隐藏模式会分散 ControlNet 注意力，导致结果变差；解决办法是用预处理把边缘图量化成多个级别，把隐藏模式彻底去掉，具体实现在 annotator/util.py 第 78 行。性能大致可记为：鲁棒性 SoftEdge_PIDI_safe > SoftEdge_HED_safe >> SoftEdge_PIDI > SoftEdge_HED；最高结果质量 SoftEdge_HED > SoftEdge_PIDI > SoftEdge_HED_safe > SoftEdge_PIDI_safe。权衡之后，默认推荐 SoftEdge_PIDI，多数场景表现良好。种子 12345、提示词“a handsome man”：[PRE6]

**Segmentation 语义分割**
用语义分割图控制 SD 生成图像。不同颜色代表不同物品和场景，可先识别再手绘对应颜色；网上能搜到语义分割的颜色与物品对应图。权重为 control_v11p_sd15_seg.pth，配置为 control_v11p_sd15_seg.yaml；训练数据为 COCO + ADE20K。可用预处理器包括 Seg_OFADE20K（Oneformer ADE20K）、Seg_OFCOCO（Oneformer COCO）、Seg_UFADE20K（Uniformer ADE20K），也支持手动创建掩码。模型现在能接收 ADE20K 或 COCO 两类注释；ControlNet 编码器识别分割协议并不困难，多协议联合训练还能带来更好性能。种子 12345、ADE20K 协议、提示词“house”：[PRE7]
种子 12345、COCO 协议、提示词“house”的未挑图批量结果：[PRE8][PRE9]

**Openpose 骨骼识别**
通过骨骼图生成图像，用于固定人物姿态和动作；新版还增加了面部表情识别。动作与表情的具体玩法可自行研究。权重为 control_v11p_sd15_openpose.pth，配置为 control_v11p_sd15_openpose.yaml。模型训练时可接受身体、手、脸，以及身体+手、身体+脸、手+脸、身体+手+脸等组合；全部开放太复杂，建议只给用户两个选项：“Openpose”=身体；“Openpose Full”=身体+手+脸。此次改进主要来自对 OpenPose 实现的优化：仔细对比了 PyTorch OpenPose 与 CMU C++ OpenPose 的差异，处理器更准确，尤其是手部；处理器改进也推动了 Openpose 1.1 的进步。新版还支持更多输入（手和脸）。旧版 cnet 1.0 的训练数据存在几个问题：1. 少量灰度人像被复制数千次，导致旧模型可能生成灰度人像；2. 部分图像质量低、模糊或 JPEG 伪影明显；3. 数据处理脚本出错，使少量图片的配对提示有误。新模型修复了上述数据问题，很多情况下结果更合理。种子 12345、提示词“man in suit”的未挑图批量测试：[PRE10]
种子 12345、多人场景、提示词“handsome boys in the party”的未挑图批量测试：[PRE11]

**Lineart 线稿**
用 Lineart 预处理器提取线稿，再控制 SD 生成图像；适合在不改变形状的前提下生成同类产品。权重为 control_v11p_sd15_lineart.pth，配置为 control_v11p_sd15_lineart.yaml。模型在 awacke1/Image-to-Line-Drawings 上训练；预处理器可从图像生成详细或粗略线稿（Lineart 和 Lineart_Coarse）。模型经过充分数据增强，也能接收手绘线稿。种子 12345 的未挑图批量测试（详细艺术线条提取器、提示词“bag”）：[PRE12]
种子 12345 的未挑图批量测试（粗线条提取器 lineart、提示词“Michael Jackson's concert”）：[PRE13]
种子 12345 的未挑图批量测试（手绘线稿、提示词“wolf”）：[PRE14]

**Anime Lineart 动漫线稿**
可用动漫线稿提取预处理器，或上传手绘线稿来生成图像；这一版比旧版保留更多细节。以动漫艺术线条控制 SD。权重为 control_v11p_sd15s2_lineart_anime.pth，配置为 control_v11p_sd15s2_lineart_anime.yaml。训练数据和实现细节已删除说明；模型可接收真实动漫线条图或提取出的线条图。种子 12345 的未挑图批量测试（提示词“1girl， in classroom， skirt， uniform， red hAIr， bag， green eyes”）：[PRE15]
种子 12345 的未挑图批量测试（提示词“1girl，saber，at night，sword，green eyes，golden hAIr，stocking”）：[PRE16]
种子 12345 的未挑图批量测试（提取线稿，提示词“1girl， Castle， silver hAIr， dress， Gemstone， cinematic lighting， mechanical hand， 4k， 8k， extremely detAIled， Gothic， green eye”）：[PRE17]

**Shuffle 洗牌**
可以理解为把图像中的颜色和内容打散，再重新组合成新图。用内容随机播放来约束 SD。权重为 control_v11e_sd15_shuffle.pth，配置为 control_v11e_sd15_shuffle.yaml；模型经过重组图像训练，用随机流打乱图像，再由 ControlNet 控制 SD 重组。种子 12345、提示词“hong kong”的未挑图批量测试：[PRE18]
右侧 6 张图里，左上角是“打乱”后的输入，其余为输出。由于模型学的是重组图像，有时甚至不用打乱输入，直接拿原图也能用；这样便可借助提示词或其他 ControlNet 引导来改变风格。注意，该方法与 CLIP 视觉等模型无关，是纯 ControlNet。种子 12345、提示词“iron man”的未挑图批量测试：[PRE19]
种子 12345、提示词“spider man”的未挑图批量测试：[PRE20]

**Instruct Pix2Pix**
可理解成图生图：在原图基础上加入描述词来修改图像。用 Instruct Pix2Pix 控制 SD。权重为 control_v11e_sd15_ip2p.pth，配置为 control_v11e_sd15_ip2p.yaml；模型在 Instruct Pix2Pix 数据集上训练。与官方版不同，它用 50% 指令提示和 50% 描述提示训练，例如“一个可爱的男孩”是描述提示，“让男孩变得可爱”是指令提示。因为它是 ControlNet，所以不用折腾原版 IP2P 的 double cfg tuning，也能套用到任何基础模型。另外，“将其变成 X”这类指令通常比“将 Y 变成 X”更有效。种子 12345 的未挑图批量测试（“make it on fire”）：[PRE21]
种子 12345 的未挑图批量测试（“make it winter”）：[PRE22]
该模型被标为“实验性”，因为有时需要挑选样本。例如种子 12345、指令“让他成为钢铁侠”的未挑图批量测试：[PRE23]

**InpAInt 蒙版重绘**
ControlNet 的蒙版重绘；简单测试下来，效果比自带图生图重绘更自然，蒙版边缘拼接也更顺。用 InpAInt 控制 SD。权重为 control_v11p_sd15_inpAInt.pth，配置为 control_v11p_sd15_inpAInt.yaml。注意事项：1. 该修复 ControlNet 训练时使用 50% 随机掩码和 50% 随机光流遮挡掩码，因此不仅支持修复应用，也能处理视频光流扭曲；未来是否提供示例取决于工作量。2. 这个 Gradio 演示不含后处理。理想做法是在每次扩散迭代后处理潜像，并对 VAE 解码后的图像再做后处理，让未遮罩区域保持不变；但实现较复杂，也许更适合在 a1111 中完成。当前示例只输出扩散原始结果，未遮罩区域可能因 VAE 或扩散过程而变化。种子 12345、提示词“a handsome man”的未挑图批量测试：[PRE24]

**Tile 拼接（模型尚未完成）**
简单说，就是把一张图切成多张小图，逐块做细节重绘，完成后再拼回原图。用 Tile 控制 SD。权重为 control_v11u_sd15_tile.pth，配置为 control_v11u_sd15_tile.yaml。越来越多人尝试在拼贴处采用不同扩散方法，以便做出 4K 或 8K 大图。问题在于，Stable Diffusion 的提示词会影响每个板块：比如提示“a beautiful girl”，把图切成 4×4=16 个 block 分别扩散，会得到 16 个“beautiful girls”，而不是一个“a beautiful girl”，这是众所周知的问题。现有做法是使用“清晰、清晰、超清晰”这类无意义提示来扩散块，但去污强度一高结果就会很糟，而且提示本身糟糕，内容也非常随机。ControlNet Tile 正是为解决此问题：对给定图块，它会识别块内内容并增强语义影响；如果内容不匹配，还会降低全局提示的影响。