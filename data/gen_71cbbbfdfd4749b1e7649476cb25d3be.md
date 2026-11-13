默认启动命令为：

`HSA_OVERRIDE_GFX_VERSION=10.3.0 python main.py`

如果你用的是 RDNA3 架构显卡，比如 7600，请改用：

`HSA_OVERRIDE_GFX_VERSION=11.0.0 python main.py`

7.

Intel GPU 用户：请先到 Intel Extension for PyTorch（IPEX）的安装页面，把对应驱动、Basekit 和 IPEX 包装好，再参照 Linux 手动安装说明启动 ComfyUI。

8.

Mac M1 或 M2 用户：先安装最新的 PyTorch nightly 版本，然后按 Linux 手动安装说明操作。

# 六、ComfyUI 配置与调优 @来来

# 📌

# ComfyUI 报错时，先自查这四件事

第 1 件：软件是不是已经升到最新版？

第 2 件：模型版本是否对得上？模型有没有放进正确目录？

第 3 件：相关节点是否保持最新？

第 4 件：工作流有没有缺节点？节点之间的连线是否正确？

# 6.1 软件更新：选对方式

# 📌

安装包一共分 4 种，所以更新手法并不完全一样。

# 6.1.1 桌面版：交给自动更新

桌面版通常会自己完成更新，不需要手动干预。若没有自动更新，进入设置，在左侧选中 ComfyUI-desktop，再把右侧的自动更新勾上即可。

# 6.1.2 纯净版：运行 update_ComfyUI

打开 `ComfyUI_windows_portable\update` 文件夹，找到 `update_ComfyUI` 文件并运行它。等到界面出现“按任意键继续”，就代表更新成功。

# 📌

优点：操作简单，省心。

缺点有两条：一是只能升级不能降级，更新后若出现兼容问题，只能重新下载并安装旧版本；二是本次升级的具体信息不够直观。

[PRE0]

# 6.1.3 Liblib 整合版：控制台与版本切换

# 📌

优点：一是简单方便；二是既能升级也能降级。

缺点：升级信息无法直观看到。

防失联+MM188166M（李李）长期更新1.

打开 ComfyUI 控制台，新版本会自动更新。

[PRE1]

2.

点击版本信息，就能快速切换版本，升级或降级都可以。

[PRE2]

# 6.1.4 秋叶整合包：用绘世启动器升内核

打开 A 绘世启动器，进入版本管理，点击内核，选择最新版本进行更新。

# 📌

好处：防失联+MM188166M（李李）长期更新

1》升级直观又方便。

2》支持升级和降级，更新后万一遇到兼容问题，可以快速切回旧版本。

3》每次升级的相关信息都能直接看到。

4》稳定版对应较大的稳定版本更新，建议初学者使用；如果你想用最新功能，可以点开发版，更新到最新版。

[PRE3]

[PRE4]

[PRE5]

# 6.2 模型管理：下载、归位与共用

# 📌

虽然安装包分 4 种，但模型下载和安装的位置是统一的。

# 6.2.1 模型从哪里下载

# 📌

# 下载站 1：Civitai

打开 https://civitai.com/models，注册登录后，点击右上角的漏斗图标，选择你感兴趣的模型种类下载。

# 下载站 2：Huggingface

打开 https://huggingface.co/stabilityai，这里汇集了许多不同版本的 Stable Diffusion 官方模型，是下载官方模型的首选地。

# 下载站 3：LIBLIB

打开 https://www.liblib.art/，在右侧点击筛选，选择不同模型种类。

# 6.2.2 模型该放哪个文件夹

# 📌

不同种类的模型，要放进 ComfyUI 对应的目录：

1.

大模型放进 `ComfyUI\models\checkpoints`

2.

controlnet 模型放进 `ComfyUI\models\controlnet`

3.

嵌入模型放进 `ComfyUI\models\embeddings`

4.

超网络模型放进 `ComfyUI\models\hypernetworks`

5.

Lora 模型放进 `ComfyUI\models\loras`

6.

视频模型放进 `ComfyUI\models\svd`

7.

放大模型放进 `ComfyUI\models\upscale_models`

8.

VAE 模型放进 `ComfyUI\models\vae`

[PRE6]

# 6.2.3 模型怎么分类更好找

# 💡

模型有两种分类思路：一是按用途分，二是按版本分。

1.

按用途分

以 LORA 模型为例，可以在 LORA 文件夹下再建多个中文子文件夹，把不同种类的 LORA 分开管理，其他模型也是同样的道理。

[PRE7]

2.

按版本分

可以按模型版本或研发公司来分。不同版本的大模型，对应的辅助模型（LoRA、ControlNet、Embedding 等）版本需要严格匹配，所以我建议安装时多建一个文件夹来区分模型版本，比如下面这种结构：

📁ComfyUI_windows_portable_nvidia

├── 📁ComfyUI

│ ├──📁 models

│ | └── 📁 checkpoints

│ │ ├── 📁 SD1.5

│ │ ├── 📁 SD2.0

│ │ ├── 📁 SDXL

│ │ ├── 📁 FLUX

│ │ ├── 📁 可图

│ │ ├── 📁 混元

# 6.2.4 让 ComfyUI 与 WebUI 共用模型

# 📌

1.

如果你电脑里装过 WebUI，模型文件通常放在 webui 目录下的 models 文件夹。把同样的模型再复制一份到 ComfyUI，会白白占用大量硬盘空间。ComfyUI 作者提供了共用模型的方法，可以避免重复拷贝大量模型文件。

1.

如果你没装过 WebUI，这一步直接跳过。

1.

在 ComfyUI 目录中找到 `extra_model_paths.yaml.example` 文件，把后缀名 `example` 去掉。

[PRE8]

2.

用记事本打开 `extra_model_paths.yaml`，把里面的 `base_path` 改成你本地 webUI 的文件夹路径。比如我的是“F:/AIGC/TOOL/SD/”。下面还可以把 VAE 模型、LORA 模型、嵌入模型等在 webui 中的路径分别填上，注意要使用 `/` 斜线。

3.

启动 ComfyUI 后，就能在模型栏读取到本地模型了：

[PRE9]

[PRE10]

# 6.3 节点管理：安装、补缺与更新

# 📌

安装包分 4 种，节点安装和更新方式会略有区别。

# 6.3.1 新节点安装的五种路径

# 📌

ComfyUI 的节点类似于 WebUI 的插件，每个节点都有若干子节点来实现特定功能。工作流，就是把这些子节点连接起来形成的。

# 💡

安装 ComfyUI 节点一共有 5 种方式：官方纯净版安装、手动安装、ComfyUI 管理器安装（推荐）、秋叶启动器安装（推荐）、Liblib 整合包安装（推荐）。

# 6.3.1.1 纯净版：先装管理器

# 💡

# 温馨提醒

官方桌面版、秋叶整合版、LIBLIB 整合版已经内置 ComfyUI 管理器，无需执行这一步。

1.

官方纯净版只有内置核心节点。若要安装其他第三方节点，需要先安装第一个节点：ComfyUI 管理器。

2.

先访问 ComfyUI 管理器节点的 GITHUB：https://github.com/ltdrdata/ComfyUI-Manager。页面通常会提供安装说明，照着操作即可。

3.

打开网址下载 Git：https://git-scm.com/downloads/win

4.

下载完成后点击安装，安装选项里只有一项需要修改，其他保持默认即可。

[PRE11]

5.

下载下方的批处理文件，放到 ComfyUI 安装根目录下。

[PRE12]

6.

双击文件，点击运行。

7.

右侧出现 Manager，就代表 ComfyUI 管理器节点安装成功。

[PRE13]

# 6.3.1.2 手动安装：压缩包兜底

1.

有些 ComfyUI 节点比较新，ComfyUI 管理器可能还没收录，无法通过管理器安装，这时可以手动安装。

2.

还有一种情况：部分节点用 ComfyUI 管理器安装不成功，可以尝试用压缩包手动安装。但要注意，不是所有节点手动安装都一定生效。

3.

以常用的 ComfyUI 汉化节点为例，打开网址：https://github.com/AIGODLIKE/AIGODLIKE-ComfyUI-Translation

[PRE14]

4.

点击页面中绿色的 `<>code` 按钮，在弹窗里点击 `Download ZIP`。

[PRE15]

5.

下载完成后解压，把解压后的文件夹复制到 `ComfyUI/custom_nodes` 插件目录下。

6.

记得删除 `-main` 后缀，节点压缩包也可以删掉。

[PRE16]

7.

重启 ComfyUI。如果右侧队列处显示中文，就代表节点安装完成。

# 6.3.1.3 管理器安装：推荐路线

1.

首先确认已经装好 ComfyUI Manager 节点。旧版 ComfyUI 界面，点击 Manager 进入管理器。

[PRE17]

2.

新版 ComfyUI 界面，点击右上角进入管理器。

[PRE18]

3.

弹窗中能看到“节点管理”和“安装缺失节点”两个选项。如果是安装新节点，选择第一项即可。

[PRE19]

4.

搜索或浏览找到需要的节点，点击 Install 即可。

[PRE20]

5.

搜不到的节点，也可以通过 ComfyUI 菜单中的“通过 GIT URL 安装节点”来安装。

[PRE21]

# 6.3.1.4 秋叶启动器：扩展安装

1.

打开 A 绘世启动器，进入版本管理，点击安装新扩展，输入关键词，就可以按需选择安装节点。

2.

如果没找到需要的节点，可以把对应插件的安装地址粘贴到界面最下方的扩展 URL 处，通过 git 来安装。

[PRE22]

# 6.3.1.5 LIBLIB 整合包：扩展管理

点击 ComfyUI 生图，进入扩展管理，点击安装新扩展，在右侧搜索节点名称，点击安装即可。

[PRE23]

# 6.3.2 缺失节点怎么补

1.

打开别人制作的工作流时，很可能遇到缺失节点的情况。缺失的节点会被直接标红，工作流也无法运行。必须先装上缺失节点，界面上会提示缺失节点的名称。

[PRE24]

2.

在右侧选择管理器，点击进入。

[PRE25]

3.

在管理器中选择“安装缺失节点”。

[PRE26]

4.

点击后会自动搜索缺失节点，出现缺失节点界面后，点击安装。

[PRE27]

安装中。装好节点后，点击重启 ComfyUI，节点才会生效。

[PRE28]

[PRE29]

# 6.3.3 节点版本更新

# 6.3.3.1 纯净版/桌面版：管理器 UPDATE

1.

打开官方纯净版或桌面版 ComfyUI，点击右上角管理器，进入管理器。

2.

在管理器滤镜中选中“更新”，点击 UPDATE 即可更新节点。可以等全部节点更新完，再统一重启 ComfyUI。

[PRE30]

# 6.3.3.2 秋叶整合版：一键更新

打开 A 绘世启动器，进入版本管理，点击扩展，再点击一键更新，就能把所有节点一次性更新到最新版本。

# 📌

好处：

1》升级直观又方便。

2》支持升级和降级，节点更新后若出现兼容问题，可以快速选择旧版本降级。

3》能直接看到节点的更新信息。

[PRE31]

# 6.3.3.3 Liblib 整合版：扩展管理里切换

点击 ComfyUI 生图，进入扩展管理，点击已安装，然后点击更新，或者切换到不同的旧版本。

建议 LIBLIB 增加一键更新按钮。

# 📌

好处：

1》升级直观又方便。

2》支持升级和降级，节点更新后若出现兼容问题，可以快速选择旧版本降级。

3》能直接看到节点的更新信息。

[PRE32]

[PRE33]

# 6.3.4 节点学习手册

# 💡

如果想详细学习 ComfyUI 内置的所有节点，推荐资料：https://ComfyUI-wiki.com/zh-CN/ComfyUI-nodes

[PRE34]

# 6.4 工作流管理：下载、加载与整理

# 📌防失联+MM188166M（李李）长期更新

安装包虽然分 4 种，但工作流的下载和放置位置是统一的。

# 6.4.1 工作流下载站防失联+MM188166M（李李）长期更新

# 📌

下面 7 个网站可以下载 ComfyUI 工作流文件，工作流文件是 JSON 格式。

Openart

https://openart.ai/workflows/

ComfyUI workflows

https://comfyworkflows.com/

Esheep

https://www.esheep.com/app

LibLib

https://www.liblib.art/workflows

Tensor

https://tensor.art/

吐司

https://tusiart.com/

ComfyUI 示例工作流

https://comfyanonymous.github.io/ComfyUI_examples/

C 站

https://civitai.com/models，选择 workflows

# 6.4.2 加载工作流

点击“加载默认”，可以加载默认的文生图工作流。

点击“加载”，就能把你下载的工作流用起来。

[PRE35]

# 6.4.3 整理工作流与云端体验

通过左上角如图文件夹，可以打开 Workspace 节点，专门用来分类整理工作流文件夹。

如果没有这个节点，安装网址：https://github.com/11cafe/ComfyUI-workspace-manager

[PRE36]

分类工作流文件。

[PRE37]

另外，如果你想直接体验一些现成的工作流，可以通过“仙宫云”来实现。

仙宫云网址：https://www.xiangongyun.com/

登录后先注册。这个平台和手册里用的“端脑云”一样，属于云端部署，需要先充值。

接着可以点击来来教练的这个镜像使用，里面有 150+ 工作流、162+ 节点、300+ 模型供大家使用。

[PRE38]

# 6.5 ComfyUI 快捷键

1.