**混音模式（--remix）**：开启混音模式，可对已有图像进行局部修改。

**设置（--settings）**：查看和调整 MidJourney 机器人的各项配置。

**简化提示（--shorten）**：提交较长提示词，获取精简版本建议。

**显示作业（--show）**：借助图像作业 ID，在 Discord 中重新调出并生成作业。

**隐身模式（--stealth）**：面向专业计划订阅者开放的隐身模式。启用后，你生成的图像不会出现在 MidJourney 的公共画廊或社区空间，仅你本人可见。

**订阅（--subscribe）**：生成专属链接，指向你的用户账户页面。

**风格调整（--tune）**：依据提示词生成风格调整器，帮助你自定义图像风格。

**涡轮模式（--turbo）**：切换至涡轮模式，让图像生成速度大幅提升。

[PRE0]

## 3.4 MidJourney（应用篇）

💡

**章节概要**

这一章，我们将一起探索如何用 MidJourney 制作个性化的手机与电脑壁纸，以及怎样借助 AI 绘画完成人物幼年化图像和表情包创作。同时，还会介绍如何利用时间、场景与人设上的反差，做出趣味十足的梗图。

具体分为 4 个小节：

1. **定制手机电脑壁纸**：本节带你学会用 MidJourney 把灵感变成独属于你的壁纸，掌握调整图像尺寸以匹配不同设备屏幕的方法，并尝试多种风格的图像生成方式。

2. **个人形象换风格**：手册将教你如何把现有的人物照片，通过 MidJourney 转换为幼年版形象，并展示具体步骤以及所需的命令和参数设置。

3. **表情包制作**：这一部分聚焦如何运用 MidJourney 的 niji 模型与 cute 风格，制作表现力丰富的动漫风表情包，并讲解图像优化调整的技巧。

4. **用各种反差来制作有趣的梗图**：最后，我们会探索如何通过制造时间、场景和人物设定上的反差，做出吸引眼球的梗图，并提供具体实例与创作技巧。

学完本章，你将掌握 MidJourney 的高级应用技巧，把创意想法落地为视觉作品。准备好就开始吧！

### 3.4.1 定制手机电脑壁纸

你是否厌倦了千篇一律的壁纸？想让自己的壁纸多几分个性，成为独一无二的存在？接下来，我就带你走进定制壁纸的奇妙世界！

#### 3.4.1.1 网页入口

💡

网址：https://www.midjourney.com/home?callbackUrl=%2Fexplore

#### 3.4.1.2 操作演示

**第一步：写壁纸提示词**

这里给大家整理了一个提示词公式： **[主体] + [风格] + [特定要求] + [附加描述]**

我们只要在公式对应位置填入相应内容，AI 就能帮我们完成壁纸制作。那“主体”“风格”“特定要求”“附加描述”到底指什么？举个例子你就清楚了。

比如，现在我想要一幅美少女的油画。直接用大白话说出来：“一幅美少女油画”。这里“美少女”就是 **[主体]**，“油画”就是 **[风格]**。

如果想让美少女更具体一些，可以多加描述：猫耳、洛丽塔。

想让她出现在指定场景，还可以加入森林、小河、树枝、石头等元素。

猫耳、洛丽塔、森林、小河、树枝、石头，这些就是 **[特定要求]**。

若还想让画面更有质感，可以加入柔和的光线、耶稣光，这就是 **[附加描述]**。

最后完整的描述词是：“这是一幅关于美少女的油画，美少女有着猫耳朵，身穿洛丽塔。身处在森林里面，森林里面有小河，树枝和石头。整幅画面有着柔和的光线和耶稣光”。

听起来有点复杂？

那简单点，换一套描述词：“美少女，油画风格，猫耳装饰，洛丽塔服饰，森林，小河，树枝，石头，柔和光线，耶稣光”。这样是不是简洁多了。

这两段描述词，我们分别生成一遍，看看效果如何。

[PRE1]

[PRE2]

你能分辨出上面两组图分别对应哪组描述词吗？

揭晓答案：前者由自然语言生成，后者由词汇组合生成。对比两幅图可以看出，用词汇生成的图像更精准；而自然语言生成的图像，AI 对内容识别稍弱，像猫耳朵、河流、石头、树枝、柔和的光线等元素都没有出现。

[PRE3]

[PRE4]

**第二步：调整壁纸尺寸**

回到案例本身，我们要定制手机和电脑壁纸，就必须保证壁纸尺寸比例适合手机或电脑屏幕。这时要用到 `--ar` 参数来调整出图比例。

常见屏幕比例中，手机以 9:16 为主，平板电脑以 4:3 为主，电脑显示器以 16:9 为主。对应参数为：

手机屏幕：`--ar 9:16`

平板电脑：`--ar 4:3`

电脑显示器：`--ar 16:9`

注意，`--ar` 与具体数值（如 9:16）之间要留一个空格。

在生图界面右下角点击重新生成按钮，再把数值放到描述词末尾。以 9:16 为例，只需将“--ar 9:16”加在描述词后面。

[PRE5]

[PRE6]

[PRE7]

Muted landscape, light gray and dark beige, bronze and blue, 1800's era, farm field, tranquil colors, antique, vintage, oil paint, brush strokes, dull colors, biege colors, saturated, pressure strokes, attention to detail, award winning, Artemisia Gentileschi style

[PRE8]

[PRE9]

A contrast image split in half. One side shows Elon, confident and victorious, with the Zip2 logo and$ 300 million floating behind him. The other half: Elon, contemplative, almost on the edge, with the PayPal logo and question marks clouding the backdrop. The two sides are separated by a shimmering, uncertain veil representing the risk and unpredictability. Bright colors and sharp contrasts emphasize the gamble and stark choices. 对比度图像一分为二。一面显示埃隆，自信和胜利，与 Zip2 的标志和 3 亿美元漂浮在他身后。另一半: 埃隆，沉思，几乎在边缘，与贝宝的标志和问号云的背景。双方被一层闪闪发光、不确定的面纱隔开，这层面纱代表着风险和不可预测性。明亮的色彩和鲜明的对比强调了赌博和赤裸裸的选择。

A mysterious black and white pen and ink illustration of a beautiful woman with a large spectator hat, dynamic composition, low angle and exaggerated perspective, clean lines and elegant curves, stylized and simple, lovely

[PRE10]

[PRE11]

Close - up, Enigmatic, All - orange cheetah, poster - like, spotted backdrop Ethereal all - orange cheetah adorned with Moiré and Matelassé - patterned elements, manifesting a pulchritudinous presence by Hajime Sorayama

特写，神秘，全橙色猎豹，海报样，斑点背景空灵的全橙色猎豹装饰着莫尔和马特拉塞图案的元素，显示出一个由 Hajime Sorayama 美丽的存在

定制壁纸并非标准品，因此主流变现路径是在自媒体平台发布高质量壁纸后售卖；或者引流到私域，做知识付费变现、包月取图变现。这条路径门槛不高，坚持做一个月以上，一定能看到成绩。有兴趣的圈友不妨一试。

《公众号写作流量主变现之美女图片方向》@叶华

《公众号流量主，ChatGPT + AI 绘画，3 天入池，5w+》@元彻

[PRE12]

[PRE13]

[PRE14]

💡

**对应航线图任务：用 MidJourney 定制一张手机壁纸**

想知道自己 AI 绘图学得如何，最快的方法就是把图片发出来，尤其是发到小红书、抖音等公域平台，看看大家的评价和整体数据表现。

我们鼓励大家从现在开始，把作业直接发布到小红书平台。具体操作可查看👉 检测 AI 绘图能力

[PRE15]

### 3.4.2 个人形象换风格

前段时间，一张 AI 生成的马斯克婴儿照在社交媒体上疯传，引发网友热议，还得到了特斯拉 CEO 马斯克本人的回应。

这张照片由一个名为“Not Jerome Powel”的网友分享，配文中幽默地暗示，马斯克对抗衰老秘方的追求可能有些过头了。推文写道：“据报道，埃隆·马斯克正在研究一种抗衰老配方，但结果失控了。”照片很快获得广泛关注，收获数万个点赞。

[PRE16]

不得不说，这样的图片实在太有趣了。用 MidJourney 也能做出这种效果，下面我就一步步教你怎么制作人物幼年化图像。

#### 3.4.2.1 网页入口

💡

网址：https://www.midjourney.com/home?callbackUrl=%2Fexplore

#### 3.4.2.2 操作演示

**第一步：将图片导入 MidJourney**

首先，导入一张想要幼年化的人物图片——可以是你，可以是我，也可以是任何人。

[PRE17]

把图片拖入对话框后上传。上传成功的图片会显示成这样。

[PRE18]

[PRE19]

[PRE20]

[PRE21]

[PRE22]

[PRE23]

[PRE24]

#### 3.4.3.1 网页入口

💡

网址：https://www.midjourney.com/home?callbackUrl=%2Fexplore

#### 3.4.3.2 操作演示

表情包大多走动漫风格，针对这类图像，MidJourney 有一个模型叫 niji，简直是为动漫风表情包量身打造的！

[PRE25]

[PRE26]

[PRE27]

下面是我生成的图片，怎么样？还不错吧！快去试试你自己的表情包吧。

[PRE28]

[PRE29]

**万能魔法公式**

💡

卡通风格：卡通风格是一种特殊的艺术风格，以夸张的形象、明亮的色彩和简化的线条来表现人物或物体。卡通风格常带有夸张的表情与动作，以及简化的形象和特征，让画面更有趣、更可爱。卡通风格辨识度高、易于传达信息、轻松愉悦，因此深受人们喜爱和接受。

公式：Showing different expressions + 主题描述 + 各种表情

魔法词：various expressions and movements

辅助词：Emoji design（表情符号设计），multiple poses and expressions（多个表情和动作），exaggerated movements（动作夸张），Four cute poses and expressions（四种可爱的姿势和表情），white background（白色背景），cartoon style（卡通风格），Joy（喜悦），fear（害怕），anger（愤怒），disgust（厌恶），gratitude（感激），sadness（伤心），surprise（惊讶），shyness（害羞），f/64 group，

EMidJourneyi sheet（表情）

#### 3.4.3.3 变现方向

用 AI 制作表情包高效又好用，发到自媒体平台也能获得不错的流量，之后引流私域或开店铺做表情包定制也是不错的选择。而且定制表情包属于非标品，操作空间很大，但并不适合挣快钱。以下方向都可以尝试：

1. 微信开放表情包平台：通过创作表情包获得打赏。
2. 广告分成：在抖音、快手等平台发布表情包相关的图文或视频。注册小程序作者并上传表情包，用户观看广告获取表情包，你则获得广告收入。
3. 制作并销售文创产品：比如表情贴纸、定制真人/宠物表情包等。
4. 教学服务：提供收费的表情包制作教学。
5. 表情包群：通过低价会员群引流，群内定期分享表情包，实现收益转化，尤其对女性用户转化效果更佳。

[PRE30]

比如拟人动物：

[PRE31]

这些案例的描述词是怎么写出来的？这里简单总结了三个实用小方法，方便大家轻松利用各种反差做出有趣图像。

#### 3.4.4.1 网页入口

💡

网址：https://www.midjourney.com/home?callbackUrl=%2Fexplore

#### 3.4.4.2 操作演示

[PRE32]

[PRE33]

[PRE34]

[PRE35]

用好人物设定反差，就能做出宠物拟人、佛祖上班之类的热门图片。

用好人物设定反差，就能做出宠物拟人、佛祖上班之类的热门图片。

掌握这三种反差描述词，轻轻松松做出热门爆款！

#### 3.4.4.3 变现方向

目前，AI 绘画在梗图领域尚未探索出体系化的变现方式，大家可以尝试做先驱者，躬身探索。

💡

**对应航线图任务：用 MidJourney 制作一张有趣的梗图**

想知道自己 AI 绘图学得如何，最快的方法就是把图片发出来，尤其是发到小红书、抖音等公域平台，看看大家的评价和整体数据表现。

我们鼓励大家从现在开始，把作业直接发布到小红书平台。具体操作可查看👉 检测 AI 绘图能力

[PRE36]

# 四、【项目实操 3/3】提升 AI 绘图能力——描述词 @天辉 @大刘 @瑾糖🔥

💡

**章节概要**

经过前面的教程，相信你已经能做出不同类型的图了。

但是，与网上那些大神相比，自己做出的图总显得逊色不少，该如何提升呢？

关键就是——描述词。

描述词，也叫提示词，是学习 AI 绘画的关键一环。

简单来说，描述词就是与 AI 沟通的语言。通过描述词让 AI 听懂你的需求，给出你想要的画面。想学好 AI 绘画，学习描述词是必经之路。

我们可以通过以下两个步骤，由易到难逐步优化描述词，提升自己的绘图能力。

第一步：简单了解描述词的逻辑，模仿优秀对标来写描述词（这里会提供大量描述词供大家模仿参考）。