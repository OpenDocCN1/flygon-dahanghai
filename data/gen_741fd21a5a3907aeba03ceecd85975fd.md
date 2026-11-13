**⚠️先别慌：Claude Code 网络报错排查**

[PRE0]

[PRE1]

如果你本地没开全局代理，可能会跳出 **Unable to connect to Anthropic services，please check your internet connection and network setting** 之类的提示。后面要是用智谱、MiniMax 等国内模型来驱动 cc，这个报错可以先放一边；如果你用的是官网原版 Claude Code，就继续往下看处理办法。

**网络报错怎么修？**

[PRE2]

思路很简单：改 Claude Code 的配置文件。

Mac 路径：`/Users/[电脑用户名]/.claude/settings.json`  
Windows 路径：`C:\Users\[电脑用户名]\.claude\settings.json`

比如 Mac 用户名是 limo，文件就是 `/Users/limo/.claude/settings.json`。如果文件不存在，就新建一个同名文件。

[PRE3]

直接双击打开 `settings.json` 编辑，把代理信息按 JSON 格式补进去：

[PRE4]

[PRE5]

注意！端口要跟自己的代理软件一致。代理软件的 HTTP 端口是 7890，就填 7890；是 7897，就改成 7897。

**3. 换条路：用国产模型 MiniMax2.7 驱动 Claude Code**

Claude Code 有两种用法：一是官方版；二是让 MiniMax2.7 这类国内模型来驱动。官方版需要在 Claude.ai 订阅，目前有 Pro、5x MAX、20x MAX 三档，价格分别是 20 刀、100 刀、200 刀。再加上 Claude 对国内一直有封锁，想用官方版得同时解决网络和海外信用卡支付两道坎，门槛不低。

这次实操，我们更推荐大家用国内模型 **MiniMax2.7** 来驱动 Claude Code。

💡先科普几个后面会反复出现的词：

1. **cc-switch**：一个在 Claude Code 里快速切换不同模型 API 配置的工具。  
2. **MiniMax2.7**：由 MiniMax 公司训练出来的模型。  
3. **Claude Code**：一个编程工具。大家平时说官方使用、封号、要网络环境，其实对应的是 Claude 模型；Anthropic 这家公司既做 Claude 模型，也做 Claude Code 编程工具。

后面实操时，你会更直观地看到它们之间的关系。

**3.1 跟着视频走一遍**

cc-switch 在 Mac 上需要做安全设置，所以这里以 Mac 为例；Windows 的设置逻辑一模一样。

视频学习链接：[安装 cc-switch](https://shengcaiyoushu01.feishu.cn/docx/Qr2NdoezHo87gIxcMy9c1vs6nIf)

视频位置如下方截图。

[PRE6]

**3.2 用 cc-switch 配置 MiniMax2.7**

**3.2.0 先看学习资料**

套餐购买地址：

https://platform.minimaxi.com/subscribe/coding-plan?code=G4YsAHUVMT&source=link

用这个链接可以打 9 折购买。

这个链接是 MiniMax2.7 注册账号和充值的地方。MiniMax2.7 模型由 MiniMax 公司提供服务，通常是付费使用的。点进去后先注册账号，再购买 Token 额度或会员套餐，才有资格调用该模型。

[PRE7]

API-KEY 设置地址：

https://platform.minimaxi.com/user-center/basic-information/interface-key

这里是获取 MiniMax Token Plan Key 的地方。账号有余额后，也不能直接把账号密码填给软件（cc-switch）。你需要在这个页面生成一个 API Key，也就是一串很长的字符密钥。它相当于专门给软件用的“专用密码”，填进软件配置后，软件才有权限代表你去调用 AI 模型。

💡一定要用“Token Plan Key”，不是上面的普通 API Key，别选错。

[PRE8]

MiniMax2.7 官方配置文档参考：

https://platform.minimaxi.com/docs/coding-plan/claude-code

这份文档相当于官方操作说明书，会详细说明在 cc-switch 里具体参数怎么填，比如 API 地址填什么、模型名称填什么。建议先点开自行学习。

[PRE9]

**3.2.1 买套餐**

MiniMax2.7 是 MiniMax（一家中国 AI 模型公司）提供的商用大语言模型。模型运行依赖 GPU、显存等计算资源，相关算力服务需要收费，所以用户要先购买套餐，拿到调用额度。

（1）点击链接打开大模型官网：

https://platform.minimaxi.com/subscribe/coding-plan?code=G4YsAHUVMT&source=link

第一次访问需要登录，直接用手机号注册即可。登录后能看到页面，点击特惠套餐后会跳到付费套餐界面。如果你注册过大模型官网，点上方链接也会出现类似的套餐选择页面。

[PRE10]

（2）按自己的情况选套餐：

- 新手观望期，或只想试试 Claude Code 功能：建议先选 29/月上手，推荐 49 的套餐。  
- 确认后期会大量使用，或需要上线产品功能：建议选 119/月。  
- 对生成速度有要求（3 倍生成速度）：选对应量套餐的极速版。

💡注意：默认会按月继续订阅。如果不想下个月继续用，记得在支付宝里取消订阅；取消后，这个月仍然可以使用。

**3.2.2 拿到 API KEY**

API Key 是一串独一无二的“身份凭证”，也是工具自动帮你登录系统的“钥匙”。系统靠它识别你是谁、买了什么套餐、还有多少额度。每次你调用 MiniMax 模型，比如让它写代码、回答问题，你的电脑或工具（如 cc-switch）都会把这个 Key 一起发送给服务器。

打开上面给出的 MiniMax 页面，就能看到如下界面。

[PRE11]

复制 API key。我这边已经配置过，所以能看到一个「复制」按钮。

💡切记保存好 Key，避免泄露，带来不必要的安全问题。

[PRE12]

**3.2.3 用 cc-switch 填入 API Key**

AI 模型本身没有聊天窗口，必须配合 cc-switch 这类软件填入 API Key，才能进行对话。这款软件的好处是界面直观，可以让你在 ChatGPT、MiniMax2.7 等多种模型之间一键切换。这次我们用 cc-switch 来配置 api-key，并使用 MiniMax2.7 模型，对新手更友好。

注意：如果你已经有官方 Claude 账号，就不需要用 CC-Switch，直接进入 Claude Code 终端，在对话框里使用 `/login` 登录即可。

第一步：下载 cc-switch。

这里用一个简单的模型切换工具 cc-switch。它是 GitHub 开源项目，能帮我们更快地切换不同模型来驱动 Claude Code。原地址：

https://github.com/farion1231/cc-switch

下面是 Windows 版和 Mac 版，开箱即用。

Windows 版本下载这个：

[PRE13]

[CC-Switch-v3.12.3-Windows.msi](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/UxmTbcWTQoR19FxZMCkcw0HJndh?response-content-disposition=attachment%3B%20filename%3D%22CC-Switch-v3.12.3-Windows.msi%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260526%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260526T134056Z&x-oss-expires=86400&x-oss-signature=8cd2adefaa862a13e11240b77379c6f25908630517e99f2c6df940580afab7f9&x-oss-signature-version=OSS4-HMAC-SHA256)

Mac 版本下载这个：

[PRE14]

[CC-Switch-v3.12.3-macOS.dmg](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/LxWqb0wRJotGMLxJ0hhcULDGnwc?response-content-disposition=attachment%3B%20filename%3D%22CC-Switch-v3.12.3-macOS.dmg%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260526%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260526T134056Z&x-oss-expires=86400&x-oss-signature=a1c74d9cce5f9b55c99749f9253a762226e5c3631de70df625f56d5f5a55203b&x-oss-signature-version=OSS4-HMAC-SHA256)

也可以直接在这里下载：

https://github.com/farion1231/cc-switch/releases

网络慢的话，下载上面直接提供的安装包。如果访问超时，可以到国内 gitee 镜像仓库下载：

https://gitee.com/iamzhihuix/cc-switch-mirror

Windows 安装时如果遇到类似错误，可以下载下面的免安装版本：

[PRE15]

这里是免安装下载的安装包：

[PRE16]

[CC-Switch-v3.12.3-Windows-Portable.zip](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/XvYKbUJIco4LBVx04PecsX8Lnxb?response-content-disposition=attachment%3B%20filename%3D%22CC-Switch-v3.12.3-Windows-Portable.zip%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260526%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260526T134056Z&x-oss-expires=86400&x-oss-signature=66864f124e6eb666df9bfefe3be2c4754cc95fc6c4ed0aa303800e37c3b4edd5&x-oss-signature-version=OSS4-HMAC-SHA256)

1. 直接解压到一个目录，不要删除这个目录。  
2. 最好右键以管理员身份运行。  
3. 可以右键发送到桌面快捷方式。

💡⚠️注意：CCswitch 版本更新比较频繁。如果你从 GitHub 下载的版本跟当前文档里的版本不一致，可以下载最新版本，大致安装流程差不多；也可以选择从这个文档的安装包下载。

这个链接点击后，Windows 电脑会显示页面。点击第一个 3.12.3 标题进去，然后把页面拉到最下面，看到 Assets，这里就是软件下载的地方，选择下方安装包即可。

⚠️注意：网络下载慢是正常的。

[PRE17]

页面往下滑会看到 Assets，就会有下载安装包的地方。

[PRE18]

如果发现没有想要的包，可以点击页面上的「Show all 17 assets」链接，就能看到所有安装包。

[PRE19]

Windows 安装包如下：

[PRE20]

Mac 安装包如下，下载完后是个压缩包。安装方法：直接双击解压，然后拖拽到「应用程序」即可。

[PRE21]

⚠️注意：如果 Mac 打不开，提示「移到垃圾篓」或者「文件损坏」之类，看 3.3 常见问题解决。

第二步：安装 cc-switch。

Windows 安装步骤：遇到这种弹窗，选择「运行」按钮。

[PRE22]

就能看到下面界面。

[PRE23]

选择安装路径。

[PRE24]

安装并等待完成即可。

[PRE25]

[PRE26]

[PRE27]

**3.2.4 配置 MiniMax2.7**

使用 MiniMax2.7 接口，等于真正让你的工具和模型开始对话，让指令能发给模型，并拿到回应。

安装完成 cc-switch 后，打开如图。第一次安装点进去是这个页面，点击右上角【添加供应商】即可。

[PRE28]

把上面在 MiniMax 页面复制的 Coding Plan Key，粘贴到下面的框里。如果已经不记得在哪里，可以再看下截图，或者打开这个链接：

https://platform.minimaxi.com/user-center/basic-information/interface-key

[PRE29]

最后点击添加即可。

[PRE30]

如下图，鼠标移上去，如果配置的 MiniMax 模型显示“使用中”，就表示配置成功。

[PRE31]

如果出现如下界面，最后别忘了点击「启用」。

[PRE32]

**3.3 安装 cc-switch 常见问题**

Q1：VSCode 插件如何使用自定义 API key？  
A：打开 CC-switch 的设置。