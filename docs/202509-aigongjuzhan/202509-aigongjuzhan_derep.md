# 九月起步：配好环境，做两个 AI 项目

## 1. 先把账号和基础环境备齐

# 1. 这一章讲什么

💡 一句话概括：从零起步，把开发、部署要用的环境全部搭好，给后面的编程实战打底。事情分两摊。头一摊是云端服务与账号：GitHub 负责代码托管与版本管理；Google 拿来登录各类第三方平台；Vercel 承担前端或全栈部署；Supabase 补齐数据库和认证。另一摊是本地工具：Node.js 提供 JavaScript 运行环境；pnpm 管依赖包；Git 记录代码版本；Trae/VS Code 是敲代码的地方；Postman 用来测接口。配一次，往后每个项目都受益。

# 💡

# 本章路线图

跟着本章学完、动手做完，路线图里的这一段就能往前推：

第一阶段：启航准备（约 3 天）

1. 商业模式与前景：摸清 AI+工具站怎么赚钱、机会在哪（约 1 天）

1. 环境配置：把 Vscode、Github、Vercel 这些开发环境装起来（约 2 天）

# 2. Google 账号：打通第三方登录

它的角色是把各类第三方工具、云服务串成一串，账号统一管，跨平台登录也省事。

推荐这样用：

用它在 Vercel、Supabase 这类平台完成授权。

把开发资料放进 Google Drive 或 Google Docs。

注册流程看视频：如何注册google账号.mp4【在线播放】

# 3. GitHub 账号：代码的落脚点

代码仓库存放、版本记录，以及 CI/CD（持续集成/持续部署）自动化，都归它管。

地址：https://github.com

注册演示：Github 注册.mp4【在线播放】

# 4. Vercel 账号：负责上线

前端与全栈项目的部署平台，Next.js、React 这类应用支持得相当到位。

操作方式：

打开 https://vercel.com

更推荐拿 GitHub 账号直接授权登录，代码一提交就能联动自动发布。

注册演示：Vercel注册.mp4【在线播放】

# 5. Supabase 账号：后端能力齐活

可以把它当成开源的 Firebase 平替，云端 PostgreSQL 数据库、用户认证、文件存储、实时数据管理等后端服务一应俱全。

地址：https://supabase.com/

## 1. 开发环境搭建与工具准备

动手写代码之前，先把趁手的家伙备齐。下面按顺序一步步来，争取一遍到位。整个过程已录屏并标好时间点，随时可以回看。

开发环境配置&工具安装.mp4【在线播放】

00:00-02:00 配置与工具速览

02:00-08:16 Node.js

08:16-10:56 npm、pnpm

10:56-13:10 Git

13:10-17:32 Trae

17:32-20:22 Postman

ps：登录 Trae 得先有 Google 账号

补充说明：

若在 09:13 装 npm 时，PowerShell 抛出执行策略受限的报错（见下图）：

![](img/bd77f9d9b7b77f326b441c9ad88de5ea.png)

在 PowerShell 里敲下面这行再回车，问题就解决了：

```
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned -Force
```

![](img/87c523b12686e14ae5fcb0116ca6383e.png)

## 1. 工具清单速览

开工前把要装的东西过一遍：

Node.js：JavaScript 运行时，后端开发的地基。

pnpm：装依赖更快、更省磁盘空间的包管理器。

Git：版本控制工具，多人协作离不开它。

Trae/VS Code：写代码用的编辑器。

Postman：调试后端接口、测试 API 的老手。

# 2. 详细安装步骤

# 2.1 装 Node.js（JavaScript 运行环境）

Node.js 到底是干什么的？

一句话：它让 JavaScript 走出浏览器，也能在电脑或服务器上跑起来。后面所有开发都建在它之上。

步骤：

1. 打开 Node.js 官网

1. 页面会识别你的系统，给出对应的安装命令

1. 复制这条命令

1. Mac 打开终端，Windows 打开 PowerShell

Mac：按 Command + 空格，搜索"终端"

Windows：按 Win + R，输入"PowerShell"

1. 粘贴命令，回车执行

![](img/7f59e42117598934bfcf85d7a83e59c8.png)

Mac 走终端 Shell，Windows 走 PowerShell，把命令粘进去执行就行。

![](img/9f3429a31eebef743f674c74b4500869.png)

装完查一下版本号，能显示出来就代表成功。

```
splendor@splendordeMac-mini ~ % node -v
v20.10.0
```

注意：装 Node 会顺带把 npm 一起装上，无需单独处理（Windows 版可能出岔子，照视频解决）。

![](img/5eac72d2b53bebc14f68e2544e0f621d.png)

![](img/1d7f442bf125a823207018e70dd9c6a0.png)

# 2.2 装 pnpm（高效的包管理工具）

pnpm 是什么？

它和 npm、yarn 属于同一类东西，但依赖包能复用，安装更快、占盘更少，用的人越来越多。

步骤：

npm 前面已经就位，直接拿它来装 pnpm 即可。

```
npm install -g pnpm
```

验证：

装完执行命令看看成没成：

```
pnpm -v
```

![](img/d60b8ba05966d8b408f55135e3ed294f.png)

# 2.3 装 Git（代码版本管理）

Git 是什么？

它像代码的"后悔药"：每次改动都存成一个版本，需要时随时退回旧状态，团队协作也靠它撑起来。

步骤：

1. 打开 Git 官网

1. 按你的系统下载安装包

1. 双击，一路点"下一步"

验证：

终端里敲：

```
git --version
```

出现类似信息，说明装好了。

```
git version 2.39.5
```

# 2.4 装代码编辑器

两个方案，任选其一：

方案 A：Trae（AI 增强编辑器）

1. 打开 Trae 官网

1. 下载国际版并装好

1. 内置 AI 编程助手，能力接近 Cursor；熟悉 VS Code 的话，也能以插件方式接入。

下载地址：https://www.trae.ai/ 。这里用国际版；买会员可选 Claude 等较强模型，站内也有 Deepseek 等免费模型。

![](img/49b436ea60269ca1951f8b7bdf53e6ca.png)

方案 B：VS Code + AI 插件

1. 下载 VS Code

1. 装好后可加装 AI 插件，例如 Claude Code

推荐插件：

Prettier：自动整理代码格式，保持整洁。

ESLint：检查代码规范，帮着写出更可靠的代码。

GitLens：强化 Git 能力，逐行查看改动历史。

![](img/8a1846629d6f17146060ce02af060916.png)

# 2.5 装 Postman（API 测试工具）

Postman 是什么？

专门测网络接口（API）的工具。后端开发时，用它模拟前端请求、确认接口是否正常，前后端联调少不得它。

用得上它的地方：

接口调试：开发 API 时，先用 Postman 发请求，确认返回数据对不对。

前后端联调：前端页面还没写完，可以用 Postman 模拟请求，看后端接口数据是否对得上。

自动化测试：写测试脚本，自动验证接口稳定性。

接口文档管理：生成 API 文档，团队共享更方便。

安装：

1. 打开 Postman 官网下载页。

2. 下载与你系统匹配的版本并装好。

![](img/4e824de3f582ddff34d21fca935407bf.png)

![](img/8adbc298f4c9f40483abe46597007726.png)

## 1. 热身 1：5 分钟生成第一个 AI 小游戏

# 1. 这一章讲什么

这一章安排两个热身项目，带你初步认识 AI 工具站的开发流程，也亲身感受 AI 开发和工具的价值。

项目 1（小试牛刀）：用搭好的环境，借 AI 编程在 5 分钟内做出经典"贪吃蛇"，再自动部署上线，让朋友打开就能玩。

项目 2（进阶挑战）：难度更高，会完整走一遍 需求分析 -> 产品设计 -> 编码实现 -> 项目部署上线 的标准流程，做一个视频下载工具站。

实战步骤：

项目 1：5 分钟生成 AI 小游戏

让 AI 编程产出项目代码。

把代码推送到 GitHub。

自动部署并分享网站地址。

项目 2：2 小时开发视频下载工具站

需求分析与产品设计。

技术方案敲定。

编码实现。

部署上线。

# 本章路线图

跟着本章学完、动手做完，路线图里的这一段就能往前推：

第二阶段：实战初体验（约 5 天）

1. AI 小游戏：五分钟内做出第一个 AI 小游戏并上线（约 2 天）。

1. 视频下载工具：从需求分析到落地，做出一个视频下载站（约 3 天）。

5分钟用AI生成一个游戏网站.mp4【在线播放】

00:00-03:36 使用 AI 生成项目代码

03:36-08:28 提交代码到 GitHub 仓库

08:28-09:22 自动化部署与分享

## 1. 使用 AI 生成项目代码

第一步：打开 Trae 编辑器，新建一个项目目录。

第二步：在 AI 对话框里描述需求，比如：

"帮我生成一个贪吃蛇游戏网站"

第三步：生成过程中，AI 若要求你确认或执行某步操作，按提示手动处理。

![](img/554b8ae0b52ca55778fec02f20abd180.png)

第四步：确认执行后，Trae 会自动启动 Web 服务，并预览游戏界面。

第五步：继续追加需求。比如嫌速度太快，可以接着说：

"加上速度控制，太快了，让用户可以自己控制移动速度"

第六步：等代码生成完毕，刷新预览，新增的速度控制功能就出现了。

# 3. 提交代码到 GitHub 仓库

# 3.1 在 GitHub 创建代码仓库

第一步：登录 GitHub，点右上角的"+"，选择"New repository"。

![](img/d4824fbc31a3a11591711da046f7a54b.png)

![](img/c49f27d58423589b14f2f5b23c78e3bd.png)

第二步：填写仓库名称（比如 SnakeGame），并确保是 Public（公开）。

注意：必须公开，因为后面要免费用 GitHub Pages 部署网站。

第三步：点"Create repository"，创建完成。

![](img/5b3cb6a3a20e6389e55dc717046f5d6d.png)

不要设成私有项目，否则后面 GitHub Pages 部署就卡住了。

# 3.2 配置 SSH 免密登录

让本地电脑和 GitHub 安全通信，先配好 SSH 密钥，之后推送代码就不用反复输密码。

![](img/80902fae8571cbc6b7621a90b3c8e33d.png)

第一步：生成 SSH 密钥

打开终端（Terminal 或 PowerShell），执行下面的命令（邮箱换成你自己的）：

```
ssh-keygen -t rsa -b 4096 -C "你的邮箱@example.com"
```

参数含义：

-t rsa：密钥类型为 RSA。

-b 4096：密钥长度为 4096 位，更安全。

-C "你的邮箱@example.com"：给密钥加个备注，通常填邮箱。

执行后系统会问保存路径和密码，一路回车即可。

第二步：查看并复制公钥

终端里执行下面的命令，看到公钥内容后复制：

```
cat ~/.ssh/id_rsa.pub
```

第三步：添加到 GitHub

登录 GitHub，进入 Settings -> SSH and GPG keys。

点"New SSH key"。

把刚复制的公钥粘贴进去，保存。

![](img/0e41bbc93ebf05693759500907682428.png)

# 3.3 本地仓库初始化与代码推送

# 3.3.1 初始化 Git 仓库并提交代码

第一步：回到 Trae 编辑器，在终端执行 git init，初始化本地 Git 仓库。

第二步：把所有文件加入暂存区。

第三步：提交代码（Commit）。提交信息可以自己写，也可以点旁边的 AI 按钮，让 AI 生成一条详细记录。

# 3.3.2 添加远程仓库地址并推送

第一步：回到 GitHub 仓库页面，复制 SSH 格式的仓库地址。

![](img/d306ac90351a3f1a3d58447a3bf17131.png)

第二步：在 Trae 终端执行下面的命令，把本地仓库和远程仓库关联（地址换成你自己的）：

```
 git remote add origin git@github.com:fuyunzhishang/SnakeGame.git
```

第三步：点 Trae 编辑器左侧的"发布（Publish Branch）"按钮，把代码推送到 GitHub。

![](img/ca4fd4673dc7d179612495a8f11d5417.png)

第四步：刷新 GitHub 仓库页面，刚推送的代码就在那里。

![](img/c323455b6fc391cbef3eeedc65bb33de.png)

# 4. 自动化部署与分享

# 4.1 使用 GitHub Pages 部署网站

接下来把游戏网站放到互联网上。

第一步：进入 GitHub 上的项目仓库，点"Settings"。

第二步：左侧菜单选"Pages"。

第三步：在"Build and deployment"区域：

Source 选"Deploy from a branch"。

Branch 选主分支（通常是 main 或 master）。

第四步：点"Save"。

第五步：触发部署：回到代码编辑器，随便改点东西（比如加一个 README.md 文件），再提交并推送。这次推送会自动唤起 GitHub Actions 开始部署。

![](img/1d1b4aae3b66046cb381661216f92087.png)

第六步：拿到网站地址：稍等片刻，再次进入 Settings -> Pages，部署好的网址就出现了。GitHub 会给一个默认域名，访问它就能打开你的游戏网站。

# 5. 分享你的游戏作品

现在把网址复制下来，发给朋友展示一下。

## 1. 热身 2：2 小时开发视频下载工具站

## 1. 项目准备

这次实战备了两套技术方案：

简易版：直接调第三方接口，功能快速落地。

进阶版：基于开源项目自己部署服务，挑战更大，能学到更多（涉及服务器部署等知识）。

请配合下面的视频操作，跟上节奏。点击链接，进入飞书文档观看。

AI工具站-教学视频

## 1. 需求分析

做自媒体、做社媒营销的人，经常要跑去抖音、📕这类平台扒素材，拿回来二次加工。可下载下来的视频、图片普遍带着水印，后期再处理特别费劲。现成的去水印小程序、网站不是没有，但自己动手做一个同样可行。

核心需求点：

交互界面要简洁，能粘贴分享链接。

工具能自动解析链接，覆盖多个主流平台。

解析后展示视频或图片封面，并提供无水印下载。

## 1. 产品功能设计

直接找个竞品来参考。比如下面这个网站，页面极简：输入框一个，解析按钮一个。点下解析，标题、封面、下载地址依次呈现。

![](img/d995eec29e622d02df5f1d521b6959a1.png)

我们可以在此基础上做得更好，比如加上视频封面预览。

## 1. 技术方案设计

去水印的原理是什么？

其实水印是客户端那边加上去的。关键在于拿到服务端回传的原始视频地址——那个地址指向的视频没有水印。说到底，这活儿就是个爬虫。

可以画一张简单的技术架构图理清逻辑：

按产品需求，设计一个经典的 B/S 架构。

方案 A（简易版）：前端页面直接调用第三方去水印 API，快速实现功能。

# 5.1 方案 A（简易版）：借现成接口

解析抖音视频有两条路：一条轻量，把解析环节外包出去；一条硬核，自己掌握整套后端。先看省事的那条。

# 5.1.1 开通第三方 API 账号

这次选的去水印平台是：https://qushuiyin.guijianpan.com/

价格门槛很低，最低一档 1 元就能开，拿来做开发联调正合适。

注册完之后，点开页面右上方的用户中心，先充一点余额进去。

![](img/3ad245a17ccc545eb797db5787b42799.png)

.

到账后找到“API 测试”，系统会生成一条内置密钥的接口地址。真正调用时，把地址尾部那段视频链接换成你要解析的分享地址就行。

![](img/ecda954e7a0524883fd0ad9648217860.png)

# 5.1.2 前端开发与接口对接

**步骤 1：Postman 先行验证**

接口到手别急着写页面，先在 Postman 里跑通一次。这一步既能确认对方服务可用，也能摸清它吐回来的 JSON 长什么结构，后面给 AI 下指令才够精准。

起一个新请求。

![](img/77ef32291ac987162ad479e28aa6d8e2.png)

![](img/70f3131485dd1d7866ec4dafece2aa61.png)

接下来处理分享文案，只留里面以 https:// 打头的那一段。比如下面这条，需要留下的是 https://v.douyin.com/ZOqdo9qsYuY/

4.89 03/24 cNJ:/ K@W.md 随意“搭讪”韩国美女，印度富人区的三哥能有多自信？ # 外国人 # 歪果仁真会玩 # 印度 # 旅行 # 看世界 https://v.douyin.com/ZOqdo9qsYuY/ 复制此链接，打开 Dou 音搜索，直接观看视频！

把这段地址接到刚才那条 API 链接的末尾，点击发送。

![](img/25b95a0ff37c3ebe786a9525d4bde4cd.png)

![](img/4bfea6d9ff57e15c0cc0c0a88748471a.png)

顺利的话，响应区里就能看到服务端回传的 JSON 结构。

**步骤 2：交给 AI 生成站点**

```
帮我生成一个去水印下载的网站，需求如下：
1\. 暂时不需登录注册，只加一个固定的密码验证，密码 123456
2\. 我们需要一个交互界面，可以粘贴分享链接，用户粘贴的链接如下 4.89 03/24 cNJ:/ K@W.md 随意“搭讪”韩国美女，印度富人区的三哥能有多自信？ # 外国人 # 歪果仁真会玩 # 印度 # 旅行 # 看世界  https://v.douyin.com/ZOqdo9qsYuY/ 复制此链接，打开Dou音搜索，直接观看视频！，需要通过正则提取出http 或者https链接
有一个开始解析按钮，用户点击开始解析就可以根据api返回的数据 展示解析的 标题、视频地址、封面地址，并预览封面
可以下载视频和封面
这是api地址：https://api.guijianpan.com/waterRemoveDetail/xxmQsyByAk?ak=你的秘钥&link=https://v.douyin.com/ZOqdo9qsYuY
这是api返回的数据结构：
content中的cover是封面字段，url是视频或者图片链接，你需要通过前端的方式下载
{
    "accessToken": "",
    "code": "10000",
    "msg": "成功!",
    "content": {
        "author": "",
        "avatar": "",
        "cover": "https://p26-sign.douyinpic.com/tos-cn-p-0015c000-ce/o8UTSAHbv4KjhggioEv4TFAeefM1ZwQH2sYeD7~tplv-dy-resize-walign-adapt-aq:720:q75.webp?lk3s=138a59ce&x-expires=1756515600&x-signature=%2FhPB1b95JwIWcplIBp%2BUI4E1yAw%3D&from=327834062&s=PackSourceEnum_AWEME_DETAIL&se=false&sc=cover&biz_tag=aweme_video&l=20250816093602CF8E8B9092420311F682",
        "coverList": [],
        "headUrl": "",
        "imageList": [],
        "likeNum": 0,
        "msg": "",
        "originText": "https://v.douyin.com/ZOqdo9qsYuY",
        "shortUrl": "https://v.douyin.com/ZOqdo9qsYuY",
        "shuiYinPlatform": null,
        "success": true,
        "title": "随意“搭讪”韩国美女，印度富人区的三哥能有多自信？ #外国人 #歪果仁真会玩 #印度 #旅行 #看世界",
        "type": "VIDEO",
        "url": "https://v9-default.365yg.com/2e3a0ce3b41372f7fe68bd18b4143c7e/689fef86/video/tos/cn/tos-cn-ve-15c000-ce/oIR085Eh9CfIXAL7fJRE1wVRdCBIgreuksvGIs/?a=2011&ch=0&cr=0&dr=0&cd=0%7C0%7C0%7C0&cv=1&br=3144&bt=3144&cs=0&ds=3&ft=aT_7TQQqUYqfJEZPo0OW_QYaUqiXXtqmRVJEjUJEpvPD-Ipz&mime_type=video_mp4&qs=0&rc=ZWRpaTU1ODM8M2ZlZDg6OEBpM3lqaHk5cjplNTMzbGkzNEAxMDJjMi4yXy4xMjIwLS0yYSNqZWhsMmRrby9hLS1kLWJzcw%3D%3D&btag=c0000e00030000&dy_q=1755308162&feature_id=fea919893f650a8c49286568590446ef&l=20250816093602F50CD29B5E9166D76423",
        "videoList": []
    },
    "timestamp": 1755308162803
}
```

等上几分钟，一份能跑的代码就出来了。

![](img/118d3ca548542af7789883000992b927.png)

打开浏览器直接预览，逐项点一遍确认功能正常；哪里不对劲，或者还想加点东西，再把需求丢回给 AI 迭代。

# 5.2 方案 B（进阶版）：自建解析服务

这条路要自己管后端，复杂度明显上来。适合懂一点 Linux、Docker 命令，也愿意折腾的朋友。

# 5.2.1 开通云服务器

机器选 DigitalOcean。新账号注册即送 200 美元额度，60 天内免费用。

注册入口： https://m.do.co/c/39f17dfb48be

开通时要绑支付方式，支付宝、Visa 卡都认，操作不麻烦。

![](img/1471ea15039a399c7df103a37cec3f21.png)

我本人走的是支付宝，图个省事

![](img/c87032ad2e59cd852505bac40ac06849.png)

# 5.2.2 初始化服务器

**步骤 1：** 顶部菜单点 Create -> Droplets，新建一台云主机。

![](img/9bb4afe926ffc344ba6705ee4703a7db.png)

机器开好之后，就能登进去开始部署了

![](img/425ab42e0ab2bb37ea965b16c0224f56.png)

**步骤 2：** 把这台机器的公网 IP 记下来。

**步骤 3：** 打开本机终端（Mac 是 Terminal，Windows 是 PowerShell），敲 SSH 连上去：

```
ssh root@你的服务器IP地址
```

随后输入创建时设的密码。屏幕上出现系统欢迎横幅，说明已经连上了。

![](img/e0ad3940fd1818c67134caa6283a153a.png)

小提醒：刚分配的 IP 有时在国内直连不通。碰上这种情况，一是挂全局 VPN，二是干脆销毁这台、重新开一台。

# 5.2.3 用 Docker 跑起 API 服务

后端我们直接拿开源项目 Douyin_TikTok_Download_API 来用。作者已经把镜像打好了，省去自己编译的麻烦。

**步骤 1：装 Docker（环境准备）**

登进机器后，按顺序跑下面几条命令：

```
# 更新 apt 并安装必要依赖
sudo apt-get update
sudo apt-get install -y ca-certificates curl gnupg lsb-release

# 添加 Docker 官方 GPG key
sudo mkdir -p /etc/apt/keyrings
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg

# 设置稳定版仓库
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```

**步骤 2：执行安装**

```
sudo apt-get update
sudo apt-get install -y docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
```

![](img/5ceba3ce3503031a6a0736a383660618.png)

**步骤 3：确认装好了**

跑一下检查命令，能打印出版本号就算成功。

```
docker --version
docker compose version
```

![](img/ecfd4b2aff8b653312cc3ef4d37ad7a9.png)

**步骤 4：拉镜像、起容器**

先取镜像：把 Douyin_TikTok_Download_API 拉到机器本地

```
docker pull evil0ctal/douyin_tiktok_download_api:latest
```

![](img/6ac25da596961393a80f1a44b39f43dd.png)

再启容器：基于刚才那个镜像跑一个实例，命令与参数如下

```
docker run -d --name douyin_tiktok_api -p 80:80 evil0ctal/douyin_tiktok_download_api
```

各参数含义：

-d：让容器在后台常驻（detach 模式）。

--name douyin_tiktok_api：给这个容器起名 douyin_tiktok_api。

-p 80:80：把宿主机的 80 端口对接到容器内的 80 端口，端口冲突时可自行调整。

evil0ctal/douyin_tiktok_download_api：所用的镜像名。

**步骤 5：检查容器状态**

敲 docker ps，列表里能看到 douyin_tiktok_api 在跑，就代表服务起来了。

```
docker ps
```

![](img/a9aa9a0078218ffa80511605ebd03f43.png)

从输出能看出容器处于运行中，80 端口已在监听。

这时候用浏览器访问那台机器的 IP，项目自带的 Web 页面就会显示出来。但我们的目标是它背后的 API。

![](img/fa338146dd63cc6a2981cf7b68699700.png)

![](img/0b0ee22533c3de9bbc05a42e9b7b1020.png)

**步骤 6：写入 Cookie（关键一步）**

服务要正常解析，必须填上自己的抖音 Cookie。

Cookie 如下：

![](img/add900aa426c6e00730a636b693f2bda.png)

先登进容器：

```
 # 进入容器
 docker exec -it 951f3ab723df bash
```

镜像里没预装编辑器，手动补一个 vim：

```
apt update
apt install vim -y
```

照项目文档找到对应配置，把 Cookie 粘进去。

![](img/18d9636c65867f1936d8fff6da5eb068.png)

**步骤 7：调通接口**

按官方文档，整个流程要分两次请求：

第一次：请求 /api/douyin/web/get_aweme_id，把分享地址传进去，换回该视频的 aweme_id。

第二次：请求 /api/douyin/web/fetch_one_video，把上一步拿到的 aweme_id 传进去，取回完整视频信息（含无水印地址）。

公网 IP 拼上接口路径，就组成你自己的 API 地址：

http://68.183.189.191/api/douyin/web/get_aweme_id?url=https://v.douyin.com/ZOqdo9qsYuY/

丢进 Postman 发一次，确认能拿到数据。

![](img/728b6007841bf980dc94b0e46039bb8d.png)

数据成功返回了。

**步骤 8：让 AI 同步改前端**

把新的接口地址、调用顺序、返回结构重新整理好喂给 AI，请它据此把前端改一遍。Prompt 可以这样写：

# 收尾前，先过这两道关

```
我先需要替换视频解析的API，获取流程也有变化，你需要先通过 这个接口获取 aweme_id http://152.42.210.73/api/douyin/web/get_aweme_id
然后通过这个接口获取视频信息，用get请求 http://152.42.210.73/api/douyin/web/fetch_one_video
入参是： aweme_id：  作品id/Video id
这是视频信息的数据结构, 下载地址取download_addr 中的 第一个 ：
{
    "code": 200,
    "router": "/api/douyin/web/fetch_one_video",
    "data": {
        "aweme_detail": {
            "cover_url": "https://p3-pc-sign.douyinpic.com/image-cut-tos-priv/f715424fb432b1e04d7eaa8a682bd6c9~tplv-dy-resize-origshort-autoq-75:330.jpeg?lk3s=138a59ce&x-expires=2070691200&x-signature=LLZjf2y9xMKq%2Fno8OmIoq2%2BCn4k%3D&from=327834062&s=PackSourceEnum_AWEME_DETAIL&se=false&sc=cover&biz_tag=pcweb_cover&l=20250816163832CBE436E3F1F51A29206C",
            "desc": "随意“搭讪”韩国美女，印度富人区的三哥能有多自信？ #外国人 #歪果仁真会玩 #印度 #旅行 #看世界",
            "video": {
                "download_addr": {
                    "data_size": 124010130,
                    "file_cs": "c:0-261633-e63a",
                    "height": 720,
                    "uri": "v1e00fgi0000d22br7nog65voekghvm0",
                    "url_list": [
                        "https://v3-dy-o.zjcdn.com/c96f32aebf4d0d875e3c950c587b39e6/68a06eac/video/tos/cn/tos-cn-ve-15c800-ce/o4gsjQXQRJhmvf9fAMCleiGCXjsQ8I874BqDEY/?a=6383&ch=26&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=3916&bt=3916&cs=0&ds=3&ft=~MeSYs809o0PD1tvSz7g9wG8albvEeC~P5&mime_type=video_mp4&qs=0&rc=ZjNmOzNlOTk2Nmc7PGZnOkBpM3lqaHk5cjplNTMzbGkzNEBgMWJiMmJhNjMxNWAyMjAzYSNqZWhsMmRrby9hLS1kLWJzcw%3D%3D&btag=80000e00030000&cc=1f&cquery=100x_100z_100o_100w_100B&dy_q=1755333512&feature_id=dc6e471fd69cf67451806384e04f2b47&l=20250816163832CBE436E3F1F51A29206C&req_cdn_type=",
                        "https://v3-dy-o.zjcdn.com/c96f32aebf4d0d875e3c950c587b39e6/68a06eac/video/tos/cn/tos-cn-ve-15c800-ce/o4gsjQXQRJhmvf9fAMCleiGCXjsQ8I874BqDEY/?a=6383&ch=26&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=3916&bt=3916&cs=0&ds=3&ft=~MeSYs809o0PD1tvSz7g9wG8albvEeC~P5&mime_type=video_mp4&qs=0&rc=ZjNmOzNlOTk2Nmc7PGZnOkBpM3lqaHk5cjplNTMzbGkzNEBgMWJiMmJhNjMxNWAyMjAzYSNqZWhsMmRrby9hLS1kLWJzcw%3D%3D&btag=80000e00030000&cc=1f&cquery=100o_100w_100B_100x_100z&dy_q=1755333512&feature_id=dc6e471fd69cf67451806384e04f2b47&l=20250816163832CBE436E3F1F51A29206C&req_cdn_type=",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v1e00fgi0000d22br7nog65voekghvm0&line=0&ratio=540p&watermark=1&media_type=4&vr_type=0&improve_bitrate=0&biz_sign=NRPI1lC4AlkgB1YZ_o3IkPAfESQSvePEcuaR9NwmI3OwTcZpH5ZUm80f5LmE9VaaOzLa7CA0Ou-V1V2BgVoXftUQ6E7HDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xs1hA&logo_name=aweme_search_suffix&source=PackSourceEnum_AWEME_DETAIL"
                    ],
                    "width": 720
                }
            }
        }
    }
}
```

别急着收工，先把测试跑一遍。

![](img/13ccecc84ddb3298eb18db9d26663dd5.png)

跑起来后，浏览器会拦下跨源请求。所谓跨源，就是网页想访问不同域名、不同协议或不同端口上的服务，浏览器出于安全默认不放行。

处理办法不复杂：再次进入容器，打开 app/main.py，在响应头里加上允许跨源的设置；保存后让容器重新启动，配置才会真正生效。

```
from fastapi.middleware.cors import CORSMiddleware

# 允许的前端来源（域名）
origins = [
    "*",   # React/Vue 本地开发
]

# 添加 CORS 中间件
app.add_middleware(
    CORSMiddleware,
    allow_origins=origins,            # 允许的源
    allow_credentials=True,           # 允许携带 Cookie
    allow_methods=["*"],              # 允许所有请求方法：GET、POST...
    allow_headers=["*"],              # 允许所有请求头
)
```

把放行跨源的代码补进去。

![](img/d7e129fd5afcd8e74c8f7fc64eef1668.png)

：wq 保存退出

重启容器

接口地址已经换成我们自己部署的那套 API。

1. 把前端也部署上去

后端安排好了，前端不能落下。继续用 GitHub Pages 可以，把前端搬到自己的服务器也行。

步骤一：新开一个本地终端，用 scp 把前端代码目录拷到服务器：

```
scp -r ./VideoDownloader root@你的服务器IP:/home
```

![](img/14091411af60c854ff1d948b63d05070.png)

步骤二：登录服务器，进入代码目录，用 Python 起一个轻量 HTTP 服务来托管页面：

```
cd /home/VideoDownloader
nohup python3 -m http.server 8000 > server.log 2>&1 &
```

这条命令会让一个监听 8000 端口的网页服务在后台运行。

步骤三：在浏览器输入 http://服务器公网IP:8000，你的视频下载工具站就能打开了。

![](img/0fb646911fba6ddea60748bc0e1fd361.png)

![](img/908e1ebfdd98ad6a69fd265dd5fada07.png)

1. 一个人怎么跑通产品全流程

# 1. 这一章讲什么

这一章要回答的是：独立开发者如何把产品从零做到上线、再做到能赚钱。起点是找到真实需求，然后用敏捷思路快速做出可验证的版本（MVP）。技术侧会重点聊 JavaScript 全栈，尤其是 Next.js，还会带上 AI 编程助手和调试方法。产品上线之后，持续集成与持续部署（CI/CD）、拉新增长、根据数据和反馈打磨迭代，也都会涉及。

换成大白话：先找到值得做的点子，用最短时间做出来，上线后想办法让更多人用、把收入跑通，再一轮轮改得更好。

⭐️这一章内容多，截图和文字说不全，我录了配套视频，建议边看边练。

点击下方链接，去飞书文档看视频：

AI工具站-教学视频

# 路线图

学完并动手做完本章，路线图上的这一阶段就能打勾：

第三阶段：运营与商业化（约 7 天）

1. 找需求：做用户调研、看同行产品，把方向定下来（约 2 天）。

1. 做流量：用搜索引擎优化和社交媒体推广，把访问量拉起来（约 2 天）。

1. 设计赚钱方式：接入 Stripe 收款，规划订阅方案（约 2 天）。

1. 不断打磨：收集反馈，改进功能（约 1 天）。

1. 产品是怎么被做出来的

多数线上产品团队通常拆成需求、设计、研发、测试、上线、运营、迭代几个环节，每个环节都有专人。独立开发者或小团队往往一个人全包，所以得同时具备想点子、做产品、搞技术、部署上线、获取用户、跑通变现这一整条链路的本事。

这些本事不是娘胎里带的，靠学习和实战一点点攒。这次航海就是帮大家补短板、放大优势，完成从量变到质变的积累。

独立开发者更适合敏捷式推进。它的核心是盯着用户价值，小步快跑，持续交付能用的版本，而不是憋到所有功能做完再一次性上线。

到了 MVP 阶段，不必堆功能，先做一个能跑通核心流程的最小版本，拿真实反馈来迭代。

一个人也要有章法。就像盖楼先打地基（技术底子和规范），上面才稳；经验不够时先盖几间“小房子”，等技能和经验上来了，再去碰“摩天大楼”。

1. 技术底子不能太薄

1. 全栈到底指什么？

这一章不展开技术理论，但产品开发绕不开的基础还是要交代。

全栈，说白了就是一个人既能做用户看到的界面，也能处理背后的业务逻辑和数据，甚至还能管数据库、服务器运维。这样的人能独立把完整功能撑起来，是个多面手。

独立开发者必须往全栈方向走；好在 AI 把门槛砍低了不少，可以边干边学，先动起来最关键。

通常说全栈，主要是指前端和后端都能独立完成。

前端管界面和交互。

前端常用：HTML、CSS、JavaScript，以及 TypeScript。

框架：React、Vue、Angular，还有 Next.js、Nuxt.js。

移动端：React Native、Flutter。

后端管业务逻辑、接口、权限和安全。

后端常用：Node.js、Python 的 Django/FastAPI、Java 的 Spring Boot、Go、PHP。

接口风格：REST API / GraphQL。

你会发现前后端都出现了 JavaScript。Node.js 让 JS 不再困在浏览器里，服务器上也能跑；于是同一门语言就能把前后端一起写了，这就是 JS 全栈。

JS 全栈的好处就一个字：快。

学得快：只啃一门语言。

改得快：前后端代码能复用，生态统一，npm 包通用。

上得快：独立开发者和小团队能迅速验证想法。

这次主线用的是 React 加 Next.js。

React 是 Meta（原 Facebook）做的前端 JavaScript 界面库，主要用来搭用户界面，特别适合 SPA 这类单页形态。

它的特点：

组件拆分：页面拆成一个个独立组件，好复用也好维护。

Virtual DOM（虚拟节点树）：页面渲染性能更好。

数据单向流动：从上往下走，逻辑清楚。

周边生态成熟：能配 React Router、Redux、Tailwind 等，搭出完整前端应用。

一句话，React 只管视图层，像一套拼图，完整应用还得自己拼。

Next.js 是 Vercel 基于 React 做的全栈框架，正好补 React 的短板。

它的能力：

SSR：页面先在服务器生成，首屏更快，对 SEO 更友好。

SSG：构建阶段产出静态页面，性能更好。

API 路由：直接写后端接口（比如 /api/user），前后端一体化。

路由自动生成：按 pages/ 目录结构自动生成路由。

前后端通吃：前端后端接口都能写，是真正的 React 全栈框架。

可以记成：Next.js = React + 服务端渲染 + 路由系统 + API 支持。

AI 能接手大部分开发，但基础语法多少要懂，至少能看懂它生成的代码，关键时候自己上手调试。

1. JavaScript 一日入门

JS 可以直接在浏览器里试：打开空白页，右键“检查”调出开发者工具，在控制台输入代码就能看到结果。

![](img/0580937d5e2b56addf91608c26313eed.png)

![](img/a50b1cfaae003455fb7308dccf1f0bbd.png)

# 语法入门

. JavaScript 是什么

一门能在浏览器和服务器（Node.js）上运行的编程语言，用来做网页交互、逻辑处理，也能写后端。

. Hello World

新建一个文本文件，存成 .html，用浏览器打开就行。

```

我的第一个JS 

```

. 声明变量、常量

```
let name = "Tom";   // 可变
const age = 18;     // 常量
var oldWay = "不推荐"; // 老写法
```

. 常见值类型

字符串："hello"

数字：123

布尔：true / false

数组：[1, 2, 3]

对象：{name: "Tom", age: 18}

null / undefined

```
let arr = [1, 2, 3];
let person = {name: "Tom", age: 18};
console.log(arr[0]); // 1
console.log(person.name); // Tom
```

# 判断、循环与函数

. 运算符

```
console.log(5 + 2);  // 7
console.log(5 > 2);  // true
console.log("5" == 5);  // true (宽松比较)
console.log("5" === 5); // false (严格比较)
```

. 条件分支（if...else）

```
let score = 80;
if (score >= 90) {
  console.log("优秀");
} else if (score >= 60) {
  console.log("及格");
} else {
  console.log("不及格");
}
```

. for 循环

```
// 打印 0 到 4
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```

. 函数定义（function）

```
// 定义一个函数
function add(a, b) {
  return a + b;
}
// 调用函数
console.log(add(3, 5)); // 输出 8

// 箭头函数 (更现代的写法)
const multiply = (a, b) => a * b;
console.log(multiply(2, 4)); // 输出 8
```

# 页面元素与事件

. 改动页面元素：JS 能直接调整网页上的内容。

```
Hello

```

. 监听事件

# 进阶实战

. 数组的常用操作

```
let nums = [1, 2, 3, 4];
let doubled = nums.map(n => n * 2);   // [2,4,6,8]
let filtered = nums.filter(n => n > 2); // [3,4]
let sum = nums.reduce((a, b) => a + b, 0); // 10
```

.

Promise 与 async/await：异步流程入门

```
function getData() {return new Promise(resolve => {setTimeout(() => resolve("数据加载完成"), 1000);
  });
}

async function show() {let result = await getData();console.log(result);
}
show();
```

· 动手做：计数器

```
0

```

# 收尾：学习目标盘点

目标不只是背语法，而是能组织出可运行的简单逻辑；函数、条件判断与循环要会用；页面元素能被脚本操控，按钮点击也能响应；数组处理和异步流程要弄懂，最后交出一个可演示的小作品。

1. 一天拿下 React 与 Node.js

# 3.1 Node.js 起步：跑通首个 HTTP 服务

执行 Node 程序前，先要装好运行环境。源码存成 .js 文件后，在命令行里输入 node 加文件名即可启动。

接着搭一个轻量 HTTP 服务：

① 新建 server.js 文件。

② 把下面这段代码放进去：

```
// 引入 http 模块
const http = require("http");

// 创建服务器
const server = http.createServer((req, res) => {
  res.writeHead(200, { "Content-Type": "text/plain" });
  res.end("Hello from Node.js server!");
});

// 监听 3000 端口
server.listen(3000, () => {
  console.log("服务器运行在 http://localhost:3000");
});
```

③ 命令行里敲：node server.js

④ 用浏览器打开 http://localhost:3000，页面会显示 "Hello from Node.js server!"。

# 3.2 React 上手：第一个组件落地

用 Vite 起 React 工程更省事。

① 命令行运行下面命令：

```
# 创建项目
npm create vite@latest my-react-app -- --template react
# 进入项目目录
cd my-react-app
# 安装依赖
npm install
# 启动开发服务器
npm run dev
```

② 浏览器会自动跳到 http://localhost:5173。

③ 查看 src/App.jsx，它承载 React 的核心单元——组件。

JSX 的妙处是能在 JS 中直接描述页面结构，写法接近 HTML。

State 负责组件内部数据的保存与变化，数据一改，视图随即刷新。

下面是最简计数器代码：

```
import { useState } from "react";

function App() {
  // 'useState(0)' 创建一个名为 count 的 state，初始值为 0
  const [count, setCount] = useState(0);

  return (

# Hello React

当前计数：{count}

      {/* 点击按钮时，调用 setCount 来更新 count 的值 */}

  );
}

export default App;
```

1. 再走一步：Next.js 概览

Next.js 把 React 扩展成全栈方案，前后端能力收在一处。

SSR 指页面先在服务器完成渲染，对 SEO 和首屏加载更友好。

API Routes 允许在 pages/api/ 下直接定义服务端接口。

初始化命令：

```
npx create-next-app my-next-app
cd my-next-app
npm run dev
```

接口文件 pages/api/hello.js 的写法：

```
export default function handler(req, res) {
  res.status(200).json({ text: "Hello from Next.js API" });
}
```

前端随后可用 fetch('/api/hello') 请求它：

```
useEffect(() => {fetch("/api/hello")
    .then(res => res.json())
    .then(data => setMsg(data.text));
}, []);
```

# 5. 让智能编码来帮忙

大模型进步飞快，智能编码工具早已不只是补全片段，更像一个能分担任务的初级开发搭档。在我们真实项目里，借助它，交付速度大约翻了十倍。

以其中一个工程为例：5 月我单月提交量只有 6k 行；到 7 月，在工具协助下接近 3w 行。当然同期手上不止一个工程。

![](img/62366ac0f85e91df09e84ecc709bc503.png)

另一个工程同样累计到 3w+ 行。

除了写码，它还能出原型图、UI 稿，覆盖面越来越广。

![](img/5dad8e581dc99cecf33f67ae90a5683b.png)

![](img/b34d0972aecc17b7173e632390316367.png)

我平时用的是 Trae 和 Claude Code。Trae 基于 VSCode 二次开发，界面与操作习惯接近 VSCode，字节出品，上手顺；它接入了不少模型，其中 Claude4 体验最好。

![](img/579af18edffce78681f1234fc90dcce1.png)

Trae 的一个顺手点：可以把某段源码或某个文件塞进提示词，让模型做精确改动；不过 Claude Code 插件更新后，这个优势不再明显。另一个贴心设计：改动完成后会列出可选项，让你挑要保留的修改，不满意还能撤回。

![](img/da11dbc5032fb5209f960fd69451394a.png)

Trae 最近还加了 Solo 模式（前提：升级 Pro；邀请码目前难拿）。它主打从写码到部署的一站式流程：先理解需求、产出开发文档，再编码、连库建表，最后发布。官方称之为从插件升级为 AI 工程师；实际体验更像串好了几个固定流程，发布接 Vercel、数据库接 Supabase，服务器自行登录部署似乎还不行。对需求不复杂的开发者来说，已经省事不少。

![](img/e0ce2d403d9f18cc7cf935b8693e9c80.png)

Solo 模式界面如下。

![](img/e64c56463f808602c8b66108c8e1237d.png)

Claude Code 没有图形界面，是纯命令行工具（CLI），但本事很大。它能把握整个工程，做跨文件重构，速度快、结果稳，关键在它能容纳很长的上下文。后续章节会细讲这些工具。

# 6. 前后端排错指南

再强的智能编码也会翻车，遇到它搞不定的场景，还是得自己上手。下面这些排查手段值得掌握。

# 6.1 浏览器端排查

a) 设断点：打开 Sources 面板，在行号左侧点一下即可下断点；右键可选“Add conditional breakpoint”做条件断点；典型用途是让程序只在某个变量满足条件时暂停。

b) 观察变量：在调试面板添加 Watch Expressions，值的变化会实时显示。

c) 单步运行：Step over（F10）逐行走；Step into（F11）进入函数；Step out（Shift+F11）跑完当前函数再返回。

![](img/228c31b4af244b2067656f0c036aba8e.png)

d) 网络面板排错：看请求是否成功（状态码、请求头、响应体）；筛选 XHR/fetch 专注接口调用；Replay XHR 可重发同一请求。

![](img/5c50940b286e74841046b3408900cbb5.png)

e) 存储数据排查：Application 面板可看 localStorage / sessionStorage / cookies / IndexedDB；常用来模拟登录状态或改缓存。

f) 页面样式调整：Elements 面板能实时改 CSS；追踪 DOM 变化可右键 → Break on → attribute modifications。

![](img/e516d7ace523eeabf4bda2f9690435e6.png)

问题规模对应手段：小毛病用 console 或断点；中等故障看 Network / Application / Source Map；复杂情况上性能分析、移动端远程调试或 Mock API；线上异常靠日志与错误监控。

# 6.2 服务端排查

# 6.2.1 通用手段

a) 日志法（最常用）：用 console.log / print / logger.info 输出关键变量；级别可分 DEBUG、INFO、WARN、ERROR、FATAL；建议上 winston、log4j、pino 这类专业日志库，支持 JSON 格式化和日志轮转。

b) 断点法：在 VSCode、IntelliJ、PyCharm 等 IDE 里下断点，单步执行并查看变量与调用栈；复杂业务或难定位的 bug 很依赖它。

c) 调试工具 / REPL：Node.js 用 node inspect 或 ndb；Python 用 pdb / ipdb；Java 走 JDWP 协议做远程 attach。

# 6.2.2 服务端专项手段

1. 接口排查：用 Postman / Insomnia / curl 模拟请求验证逻辑；配合 Fiddler / Charles 抓 HTTP/HTTPS 包。

2. 数据库排查：在 SQL 执行前后打印语句和参数；慎用 ORM 的 lazy load，调试时打开 SQL 日志；用事务回滚测试逻辑，避免污染真实数据。

3. 远程排查：服务器运行时 attach 调试器（Java：-agentlib:jdwp，Node：--inspect）；Docker 容器里可用 docker exec -it 加调试工具进入环境。

4. 配置与环境排查：打印当前加载的配置文件和变量；常见问题是本地 dev 配置和 prod 配置不一致；用 .env 或配置中心统一管理环境。

# 7. 自动交付流水线

产品迭代频繁，一天发几次都正常；每次手工打包上传太费劲。CI/CD 就是把这段流程自动化。

CI（持续集成）：代码推到 GitHub 后自动构建、跑测试，尽早发现新代码引入的 bug。

CD（持续部署）：测试全过就自动发到服务器，做到提交后尽快上线。

这次会接触两种工具：

Vercel 自带 CI/CD，Next.js 工程配置少、开箱即用。

GitHub Actions 更强更灵活，可自定义复杂发布流程，比如部署到自己的机器。

![](img/48cc3abade9367f7a5d9872bac1a9ca6.png)

GitHub 每个账号每月有 500 分钟免费额度，项目设置里能看已用时长和任务数。

1. 智能编码起步

# 1. 智能编码的演进

早期 GPT-3 阶段：靠网页问答或 API 产出代码片段，交互有限。

中期 Copilot 阶段：以 VS Code 插件形态出现，能结合上下文自动补全，体验自然不少。

现在 Agent 阶段：Cursor、Trae、Claude Code 等能理解整个工程，跨文件重构、调试，甚至执行部署命令，形成较完整的开发闭环。

智能编码的核心瓶颈之一是模型能同时容纳多少代码，也就是上下文长度；一次看到的源码越多，对意图的把握越准。Claude Code 的强项正是超长上下文管理，这也是它处理复杂任务时更稳的原因。

# 2. 智能编码工具实战

# 2.1 Trae：直观好上手

Trae 的亮点是交互直接、上下文引用准。

Chat 模式像对话一样对代码库发问，拿建议或优化方案。

上下文引用可用 @ 指向某个文件或整个工程，让模型改动更精确。

代码变更预览会以 diff 呈现，接受或拒绝由你决定，安全性高。

![](img/aae9ca916aeac6dd4f321f3d9a3602eb.png)

# 2.2 Claude Code：命令行里的能手

# 2.2.1 Claude Code 到底是什么

它能理解整个源码库，而不只看当前文件；能跨文件重构、调试；能帮你写 PR、跑测试、修 bug；还能与 Git、CI/CD、数据库、API 等工具链配合；用自然语言交互，让模型成为仓库里的协作伙伴。

它的代码理解方式很特别：不做索引，也不用 RAG（检索增强生成），更像新人进团队后靠探索熟悉项目，称为“智能体式搜索”。它会用 glob、grep、find 等命令在代码库中查找、读文件，理解结构与逻辑。于是模型可以先搜一轮，再根据结果判断还需要补哪些信息，继续搜索，逐步建立对工程的认知。

![](img/e20c92e05746831abe847d91b35f99df.png)

# 2.2.2 Claude Code 使用窍门

1. 项目初始化（/init）

新工程先用 /init 初始化，让 CC 理解业务逻辑、功能、技术栈、启动方式等；后续任务时它会自动加载该文件读取工程信息。

CLAUDE.md 是一个特殊文件，Claude 发起对话会自动把它放进上下文。它可存：工程业务逻辑、核心文件和实用函数、代码风格与仓库规则、开发者环境设置与测试说明、项目特有的异常行为或警告、其他信息。

![](img/869c50bb081f9934267bc95d80e063da.png)

2. 常用命令

- /init 生成 CLAUDE.md 项目记忆文件
- /clear 清空会话历史
- /compact 压缩会话历史
- /model 切换模型
- /permissions 查看/更新权限
- /status 查看账户/系统状态
- /resume 恢复对话

3. 自动模式

```
claude --dangerously-skip-permissions
```

--dangerously-skip-permissions 是跳过权限检查的开关。

Claude Code 在执行读写文件、运行 shell 命令、调用外部工具等操作时，默认会弹确认，防止模型在你不清楚的情况下改关键文件、删数据或跑危险命令。

开启后它不再询问，直接执行认为需要的动作：直接访问/修改文件；直接运行 Bash 命令；直接调用已配置的 MCP 工具。

4. 提示词技巧

规则约束：CC 也有常见毛病——幻觉、一本正经地胡说、自作聪明、爱 Mock 数据、爱模拟结果、写冗余代码等；所以要在 CLAUDE.md 里立规矩，比如编码风格、常用技术栈等。

![](img/011db972388bcf2c2f09e095d212cbf3.png)

善用上下文：Claude Code 能读取当前目录全部源码，建议从工程根目录启动，这样依赖关系理解得更准。

分步描述复杂任务：任务太大就拆成多个小步骤，让 Claude Code 逐步完成，降低出错率。

有效管理上下文：模型有 20 万 token 的超大上下文窗口，但长会话仍可能塞满。右下角出现“上下文即将用尽”的警告时，有两个选择：/clear 清空当前会话重新开始；/compact 启动内部提示，让模型把当前会话总结成摘要，再用摘要作为新会话的种子，无缝继续工作。

构建高效工作流：先计划后执行。不要直接命令“修复这个 bug”，可以说“我遇到了这个 bug，请先调查原因，然后给我一个修复计划”，这样能在它动手前验证思路。

利用待办事项（To-Do List）：复杂任务中 Claude 会生成待办列表，观察列表，发现方向不对就按 Escape 打断并调整计划。

拥抱测试驱动开发（TDD）：让 Claude 小范围修改、运行测试、检查代码规范，然后提交；小步快跑能确保项目不偏离轨道。

做UI开发的时候，最烦的就是需求传不到位。以前得写一堆说明，现在直接截个图丢给Claude，它就能照着视觉稿把界面搭出来；也可以让它打开图片文件，比如mock.png，然后根据设计一步步实现，沟通成本大大降低。

写代码也别裸奔，Git一定要用起来。我当时给CC立了个规矩：每次改动范围尽量小，万一某一步改错了，版本库里随时能找回之前的状态。我的流程是先用 `stash` 把改动收起来，一段一段确认没问题，最后再打一个完整的 `commit`。举个例子：一个功能常常要拆成好几个小步，或者CC一口气生成的代码差了点意思、需要来回调，这时候就把每个临时改动先放进暂存区，审完再统一提交，历史记录始终干净清楚。

![](img/c00f8f1c9e998be9cae9dec88d778e46.png)

**1. 需求挖掘**

需求找准了，后面每一步都省力。下面这些方法都比较接地气。

**1. 在自己的生活里找线索**

最简单的方式就是盯住自己和身边人的抱怨。你平时用某个软件觉得卡、觉得烦、觉得反人类的地方，就是机会——因为你就是一手用户，痛在哪只有你最清楚。身边的朋友同事吐槽某款产品不好用的时候，也别只当八卦听，那可能就是没人填上的坑。

**1. 去排行榜里选方向**

思路可以照搬电商选品：打开Toolify这类AI导航网站，翻一下月度榜单。几个技巧：多留意排名一百名开外的产品，近期冲上来的新面孔一般藏在那儿；再看看它的流量结构，如果自然搜索带来的比例高，比如超过50%，说明这个赛道的需求已经被市场验证过了。挑一个自己技术hold住的，先照着做一遍，再琢磨怎么比原作更进一步——模仿不是终点，超越才是。

![](img/7da53095ef03306de2b41397b05e0996.png)

**1. 拿竞品当试金石**

方向有了，但拿不准是不是真需求，那就去拆对应的竞品。看什么？一看商业路径，它是靠广告还是订阅赚钱；二看流量来源，是花钱砸出来的，还是靠SEO、口碑长出来的。只要竞品有稳定流量、又能赚到钱，这个需求大概率是真实的，可以放心往前推。

![](img/03256b2a2f2d33488d2f8d85f9323e7c.png)

![](img/7ae4cd96d7c8f922c75b329e913bbecd.png)

**1. 用MVP做验证**

《精益创业》最重要的一句话：先写假设，再写代码。我们脑子里冒出来的需求，说白了都只是猜。关键是花最少的钱、用最快的方式去证明它。MVP要的就是“小”和“能用”——不用做得多精致，只要把最核心的那个痛点解决了，就马上丢到市场上去，让真实用户告诉我们答案。Dropbox当年甚至都没写产品，只录了一段概念演示视频发出去，结果一晚涌进来几万个想用的用户，需求是否成立当场就有了结论。我们做的第一个版本大概率又丑又糙，但那不重要，重要的是让第一批种子用户用上它，验证方向到底对不对。

![](img/7d67b57e87b619d2199a360420882bfe.png)

**1. 数据收集与分析**

产品该怎么调优？别拍脑袋，看数据。数据就是产品的仪表盘。

# 2.1 不同阶段，数据重心不一样

那么这些指标和数据从哪儿来？借助现成的统计分析工具是比较快的路子。

# 2.1.1 用户行为数据从哪里拿

**1. 百度统计**：https://tm.baidu.com/

国内免费，用起来也很顺。UV、PV、新老用户占比、流量来自哪里，这些基础指标一目了然。

![](img/903bf22528446f836b2ca2ed20bdf268.png)

![](img/f94853146ce9e297c90882a09624cb23.png)

![](img/25ffc42f066e1b7dc9ef06b3273005af.png)

这些数字能告诉你网站的真实状态：UV看的是每天来了多少人、新来的占几成，做增长的人得死盯这个指标；搜索词和外链则暴露了SEO功夫深不深。我们官网的搜索词几乎都是品牌名，说明产品词根本没有自然排名，SEO这块还差得远。外链那边经常能看到Doubao、Kimi这样的来源点进来，这是AI推荐带来的流量，也就是最近大家都在说的GEO。

**2. Umami**：https://us.umami.is/

我平时也常用，开源项目，可以部署在自己的服务器上，数据完全自主掌控。

![](img/e754552a143f9c581f69fc0e8643c6ce.png)

**3. Google Analytics**：https://analytics.google.com/

功能很强大，用户的行为轨迹、流量来源、转化漏斗都能查，适合深度分析产品表现、优化营销动作。

![](img/62ed140076edade99ed8f3365a548e18.png)

![](img/0b104d83029280cb33494eab99178025.png)

![](img/550e36257101e4d35601fa3deb57f259.png)

**4. Microsoft Clarity**：https://clarity.microsoft.com/projects

免费工具，主打热力图和用户录屏回放。注册好、把代码接进网站就能开始观察用户到底怎么操作。

# 2.1.2 用户反馈怎么收集

最直接的是在应用里加上反馈入口，让用户顺手就能告诉你“这个功能好用”或者“这里出了问题”。

![](img/2c097543827f941f471cff208e804148.png)

![](img/a9332503778ddc23f8169b039ce6296f.png)

我们还用扣子搭过一个AI客服。用户咨询产品功能怎么用，它会先去查产品知识库，很多简单问题当场就能答复。以前这些重复问题都得靠人工接，每天大概要吃掉0.5人天；接上AI之后，人工进线量掉了70%，剩下的都是需要排查bug的疑难杂症，省下来的时间和成本都很可观。

![](img/f3a733a5511e8c4e875016cff785a4e0.png)

![](img/e86f6fccd20c9fb510883ce2315f58dd.png)

**1. 怎么找到产品的PMF**

增长真正要过的关是找到PMF，也就是产品跟市场之间的契合点。

# 1. PMF是什么？

说白了，用户需要的东西你恰好做出来了，而且做得不错。

# 2. 怎么知道已经找到了？

几个信号可以参考：用户不请自来，而且这个势头还在涨（活跃用户持续走高）；用过的人愿意再次打开（留存率好看）；他们会主动转发、安利（口碑好，NPS高）；掏钱也痛快（付费转化率可以）。

# 3. 通向PMF的四个台阶

第一步：定人+定痛点。先想清楚服务谁、解决什么问题。还得问两句：这是刚需还是伪需求？频率是高是低？创业的话，“刚需非高频”或“刚需高频”是更稳的选择。

第二步：用MVP去碰。别一上来就搞大而全，集中火力攻最痛的哪一点，尽快做出一个能看能用的版本推进市场。

第三步：盯着行为迭代。用前面说的工具去看：用户留住了吗？核心功能被反复用吗？有人愿意买单吗？哪不行就改哪。

第四步：亮出价值，放大传播。小范围验证通过以后，把产品的独特价值主张（UVP）抽出来，用内容、投放去触达更大的圈层。

**1. 运营增长**

**1. 冷启动阶段（0 → 1）**

目标很单一：让“没人知道、没人用”变成“有人来、有人夸”。

常用打法：

- 精准圈种子用户：从合伙人和身边人的关系网出发（朋友、行业人脉、社区）；去目标用户浓度高的地方蹲点（🛰️群、Reddit、Discord、论坛、垂直圈子）；用邀测、内测的名额制造一点稀缺感。
- 靠价值说话：给一小撮用户提供体验上碾压级的产品价值（“10倍好”）；搞“首批体验官”“测试者”招募，让用户觉得被重视、有面子。
- 低成本做内容：写产品故事、开发日记、踩竞品痛点长处的对比分析；然后在垂直社区持续露脸（比如indiehackers、掘金、知乎、X/Twitter）。
- 设计激励：早期拉新奖励（推荐一个人送Pro月卡、周边）；内测用户反馈给权益。

上面这些办法都不贵、也好上手。想更快验证MVP的话，也可以直接砸点广告。我们自己冷启动走的是两条路：一是在B站这类社交平台发内容，二是在目标用户聚集的社群里持续分享干货，第一批精准种子用户就是这么圈到的，假设也随之得到验证。产品确实帮到了人，口碑自然就传开了。

![](img/fba43396ae4fafb02f75b17e6bb1ce30.png)

![](img/08960815053ccac76f9e4a87d0f8c6f5.png)

![](img/e3dc20318f6a1b7c299cb9709d9a93ab.png)

**1. 增长加速阶段（1 → 10）**

目标：把增长曲线拉起来，同时确认留存和转化靠得住。

常用打法：

- 增长黑客类：对注册→使用→付费的核心路径做A/B测试；看行为数据找留存下滑的环节。
- 口碑+裂变：搞邀请机制（推荐返利、团队协作中强制邀请）；制造用户愿意晒出去的社交货币（分享成果、展示身份）。
- 内容+SEO：围绕产品持续产出（教程、真实案例、竞品对比）；做好SEO/ASO，让用户搜得到你。
- 场景化合作：跟上下游工具/服务做集成（如Zapier）；请垂直领域的达人做测评，把外部流量引过来。

到这一步，需要用更系统的增长方法了——也就是前面反复提到的数据统计、分析、再调优。我们自己的增长也完全是数据驱动的，不少用户反馈说我们响应快、更新勤，其实是这套流程在起作用。

**1. 规模化扩张阶段（10 → 100）**

目标：把已验证的模式放大，做大规模获客与营收。

常用打法：

- 品牌+市场：明确品牌定位、做差异化传播；加大广告投放（Google Ads、Facebook Ads、抖音/快手）。
- 渠道+生态：入驻主流平台（App Store、Chrome插件商店、SaaS Marketplace）；开放API/插件，拉上开发者一起玩。
- 增长飞轮：UGC和分享成果→带来新用户；付费收入→再投广告→继续获客；用数据不断优化→提升转化和留存。
- 国际化/多市场：做本地化适配（语言、支付方式、文化细节）；分渠道运营（国内抖音/📕，海外Reddit/HN/Product Hunt）。

我们走过1-10的阶段后，增长模型基本跑通了，后面就是放大。这时广告会成为主要的获客引擎，品牌建设也要同步跟上。品牌是自带溢价的——就像苹果、特斯拉，不需要花太多力气解释，用户自己就会传播、会买单。

**1. 核心思路总结**

冷启动靠精准，找最痛的用户、给最极致的价值；增长靠裂变，让用户替你把产品介绍给更多用户；规模化靠体系，品牌、渠道、生态互相拉动，形成持续增长的飞轮。

# 08 产品上线只是开始，迭代永不停

做产品最忌讳完美主义。敏捷开发的本质就是边走边看、快速试错、不停迭代。独立开发者和小团队最大的优势是船小好掉头；大公司一旦投入资源就难回头，我们没这个包袱。产品持续变好的关键在于：跑通“用户反馈→数据分析→产品迭代→验证”的闭环，并且在不同阶段有不同的侧重点。拆开来看就是一整套可落地的打法：

**1. 建立反馈机制**

**1.1 用户直接说的**

- 应用内放“意见反馈”入口，让用户随手能提。
- 定期做调研问卷、NPS调查。
- 客服渠道、用户社群里收集意见。

**1.2 用行为表达的**

- 事件埋点：关注点击、停留、转化路径。
- 看使用时长、留存率、核心功能使用频率。
- 用热力图/录屏（比如Hotjar）找交互卡点。

前面提到的反馈表单可以放在网站右下角，AI客服也可以一直开着。

![](img/68b7bf6a070ecb7e1a3e360cda34b454.png)

![](img/dde21bef62db33d22a968fc909c2550f.png)

![](img/8648b3b6ec29bb3ebe62571a3cf5816c.png)

**1. 数据驱动决策**

**2.1 用AARRR拆指标**

- Acquisition（获客）：新用户从哪里来。
- Activation（激活）：有没有顺利完成第一次关键操作。
- Retention（留存）：过一阵子还会不会回来。
- Revenue（收入）：付费转化率、客单价怎么样。
- Referral（推荐）：用户愿不愿主动推荐给身边人。

**2.2 异常定位**

- 留存差→产品给的价值还不够。
- 转化差→收费方式没设计好，或者价值没有讲清楚。
- 增长停了→推荐和分享机制还不够强。

用前面提到的那些数据工具持续盯这些指标，及时调整。

![](img/547e70981f229457a3dc41622c9ae243.png)

**1. 迭代优化方法**

**3.1 MVP验证**

新功能上线前先低成本试：原型、灰度、小范围内测。先不追求完整，重点是确认用户真的需要。

**3.2 小步快跑**

单次迭代只咬住一个核心目标（比如提升留存、改善转化），每1~2周发一个小版本观察效果。

**3.3 灰度发布 + A/B测试**

先给一小部分用户用，避免全量上线踩雷；多个版本并跑，谁的数据好就让谁胜出。

迭代速度比什么都重要。我们自己经常先脑补一堆点子，结果多半是错的，所以唯一靠谱的办法就是赶紧上线验证，错了马上改。建议按1-2周的节奏推进，我们的产品到现在已经迭代了30多版了。

**1. 形成增长飞轮**

**4.1 用户共创**

把种子用户拉进设计流程（比如功能投票池）；靠社区共建，让用户自己产出案例、模板和脚本。

**4.2 数据驱动优化**

每个版本上线后对比关键指标，留下有效的改动，砍掉无效的尝试。

**4.3 迭代节奏**

- 早期：快速试错，两周一个版本。
- 成长期：稳定迭代，一月一个版本。
- 成熟期：按季度做版本规划。

这套流程跑下来，你的产品会慢慢长出一张价值网，这就是增长飞轮。你之后要做的就是转动它、提速它、让它转得越来越顺。

**1. 总结成一句话**

用户的声音是方向盘，数据是仪表盘，MVP和A/B测试是实验台，迭代是发动机。这四样配合好，产品才能不断向前滚，用户体验和商业价值才会一起往上涨。

# 1. 本章概览

这一章是一个完整的实战项目：带你从零手搓一个AI工具站，目标是把一个月流量过百万的真实站点复刻出来。全程会从选品、需求分析起步，接着设计技术方案、开发后端接口与前端页面，框架安装、UI绘制、联调测试都不落下；最后还要完成上线发布、用户登录、域名绑定、SEO优化和数据监控，走完整个流程。

# 本章航行路线

学完本章并动手实操，就可以点亮航线图中的：

第四阶段：百万流量站复刻（约 4 天）

1. 产品实现：从需求到技术、前后端开发与UI实现（约 2 天）。

1. 项目部署：联调、发布、用户管理、域名绑定与SEO优化（约 2 天）。

教学视频在这里：点击下方链接，进飞书文档查看⬇️
AI工具站-教学视频

有一次我翻Toolify榜单，注意到一个排名涨得很猛的网站：https://imageprompt.org/。它做的事情是优化图片提示词（Prompt），实现难度不高，月访问量却做到了一百多万。这简直就是“从0到1复刻AI工具站”最合适的练手标本。

![](img/93358506c90ab608c4f8c41181167ecc.png)

![](img/a2fe4106f830bf513d7d7871edecbd0a.png)

# 2. 需求分析

先理一下需求清单。

网站的核心功能是提示词反推：上传一张图，自动生成适合Midjourney、Stable Diffusion等模型的提示词。

![](img/f18c4478dc4e7017b277bd157baca3ff.png)

图片上传支持两种方式：本地文件和URL链接。

![](img/2a317737dbf99af7604569a421f076e2.png)

还提供提示词的多语言翻译。

![](img/3fb14887e6fcf4fe11b2a624d3eb07eb.png)

另外有提示词优化：把用户随口写的一句话整理成AI模型能看懂的语法。

![](img/ff07adbfe3b763302af22f15864ea825.png)

其他周边功能还包括：文生图、图生图、视频提示词反推、图片生成视频等等。我们精力有限，只保留最核心的提示词反推。

# 3. 技术方案设计

# 3.1 技术分析

主要看四种提示词结果怎么返回。

1. General Image Prompt（通用提示词）——用多模态大模型的视觉理解能力即可，图片丢给模型，让它输出一段自然语言描述。这边选豆包Doubao-Seed-1.6-vision。
2. Flux——对应的提示词反推插件叫PromptGenV2。
3. Midjourney——本身就带提示词反推。
4. Stable Diffusion——用前面提到的WD14 Tagger插件。

# 3.2 方案设计

具体怎么做？方案一是自己部署模型：给Midjourney、Stable Diffusion各配一台专门跑反推模型的GPU服务器。效果肯定最好，但成本完全扛不住——每个模型一台服务器，一个月就是几千块起步，不适合我们这种轻量打法。

方案二（寻找现成 API）：直接找能反推提示词的接口。一圈找下来，这类服务少得可怜，绝大多数还是文生图接口。

方案三（折中路线，也是我们最终采用的做法）：先用豆包 Doubao-Seed-1.6-vision 这类通用多模态模型理解图片，产出一段自然语言描述；再让另一个大模型结合我们准备好的提示词模板与语法规则（放在知识库里），把这段描述转译成 Midjourney、Stable Diffusion 等不同模型能用的专业提示词。这条路线花费最少、落地最快。后端 API 直接交给扣子（Coze）工作流，我们只需把前端页面做好。

业务流程图如下：
![](img/9bbf32ae4d43119d3ef8f8e3321bd625.png)

服务端接口准备用扣子工作流实现，因为扣子能调用大模型和知识库，本身还提供知识库，所以项目里只要完成页面交互即可。

1. 后端接口开发

# 4.1 在扣子中搭工作流

打开扣子主页 https://www.coze.cn/home ，新建一个工作流；工作流也能通过 API 调用。

名称定为 imagePromptAPI，作用是根据用户上传的图片和选择的模型，生成对应提示词。这个工作流要放 4 个大模型节点，分别产出 4 类提示词；再加 1 个选择器，依据用户选的提示词类型把请求分发给不同的大模型；最后用 1 个变量聚合节点，把 4 个模型的输出汇总起来。

需要为 3 个模型找提示词风格实例，存进知识库供大模型调用。例如找 Stable Diffusion 提示词，可以直接在 Google 搜关键词：
![](img/da597ef7fc9c585e423cc136438d2b37.png)

不同模型的提示词结构并不一致。以 SD 为例，结构通常是（质量）+风格+主体+细节+其它，还会用到权重符号（）和 [] 等。SD 的提示格式化完整 Prompt 可以写成这样：
```
Stable Diffusion prompt 助理

你来充当一位有艺术气息的Stable Diffusion prompt 助理。

## 任务

我用自然语言告诉你要生成的prompt的主题，你的任务是根据这个主题想象一幅完整的画面，然后转化成一份详细的、高质量的prompt，让Stable Diffusion可以生成高质量的图像。

## 背景介绍

Stable Diffusion是一款利用深度学习的文生图模型，支持通过使用 prompt 来产生新的图像，描述要包含或省略的元素。

## prompt 概念

- prompt 用来描述图像，由普通常见的单词构成，使用英文半角","做为分隔符。
- 以","分隔的每个单词或词组称为 tag。所以prompt和negative prompt是由系列由","分隔的tag组成的。

## () 和 [] 语法

调整关键字强度的等效方法是使用 () 和 []。 (keyword) 将tag的强度增加 1.1 倍，与 (keyword:1.1) 相同，最多可加三层。 [keyword] 将强度降低 0.9 倍，与 (keyword:0.9) 相同。

## Prompt 格式要求

下面我将说明 prompt 的生成步骤，这里的 prompt 可用于描述人物、风景、物体或抽象数字艺术图画。你可以根据需要添加合理的、但不少于5处的画面细节。

### 1\. prompt 要求

- 你输出的 Stable Diffusion prompt 以“**Prompt:**”开头。
- prompt 内容包含画面主体、材质、附加细节、图像质量、艺术风格、色彩色调、灯光等部分，但你输出的 prompt 不能分段，例如类似"medium:"这样的分段描述是不需要的，也不能包含":"和"."。
- 画面主体：不简短的英文描述画面主体, 如 A girl in a garden，主体细节概括（主体可以是人、事、物、景）画面核心内容。这部分根据我每次给你的主题来生成。你可以添加更多主题相关的合理的细节。
- 对于人物主题，你必须描述人物的眼睛、鼻子、嘴唇，例如'beautiful detailed eyes,beautiful detailed lips,extremely detailed eyes and face,longeyelashes'，以免Stable Diffusion随机生成变形的面部五官，这点非常重要。你还可以描述人物的外表、情绪、衣服、姿势、视角、动作、背景等。人物属性中，1girl表示一个女孩，2girls表示两个女孩。
- 材质：用来制作艺术品的材料。 例如：插图、油画、3D 渲染和摄影。 Medium 有很强的效果，因为一个关键字就可以极大地改变风格。
- 附加细节：画面场景细节，或人物细节，描述画面细节内容，让图像看起来更充实和合理。这部分是可选的，要注意画面的整体和谐，不能与主题冲突。
- 图像质量：这部分内容开头永远要加上“(best quality,4k,8k,highres,masterpiece:1.2),ultra-detailed,(realistic,photorealistic,photo-realistic:1.37)”， 这是高质量的标志。其它常用的提高质量的tag还有，你可以根据主题的需求添加：HDR,UHD,studio lighting,ultra-fine painting,sharp focus,physically-based rendering,extreme detail description,professional,vivid colors,bokeh。
- 艺术风格：这部分描述图像的风格。加入恰当的艺术风格，能提升生成的图像效果。常用的艺术风格例如：portraits,landscape,horror,anime,sci-fi,photography,concept artists等。
- 色彩色调：颜色，通过添加颜色来控制画面的整体颜色。
- 灯光：整体画面的光线效果。

### 2\. 限制：
- tag 内容用英语单词或短语来描述，并不局限于我给你的单词。注意只能包含关键词或词组。
- 注意不要输出句子，不要有任何解释。
- tag数量限制40个以内，单词数量限制在60个以内。
- tag不要带引号("")。
- 使用英文半角","做分隔符。
- tag 按重要性从高到低的顺序排列。
- 我给你的主题可能是用中文描述，你给出的prompt和negative prompt只用英文。
```

其他模型同理：
```
Flux Prompt 助理
你来充当一位有艺术气息的 Flux Prompt 助理。

## 任务

我用自然语言告诉你要生成的主题，你的任务是根据主题想象一幅完整的画面，然后转化成一份详细的、高质量的 Flux Prompt，让 Flux 可以生成高质量的图像。

## Prompt 概念

Flux 的 Prompt 更接近自然语言，语法结构比 Stable Diffusion 更自由。它常常由几个用竖线 “|” 分隔的部分组成，每个部分包含画面描述的不同维度。

## Prompt 格式要求

Flux 的 Prompt 输出时，需包含以下部分（从左到右，按重要性排列）：

主体 (Subject)
画面的核心内容，用英文详细描述（人、物体、场景、抽象概念等）。
如果是人物，必须包含面部细节（eyes, lips, nose, eyelashes, expression 等）。

风格 (Style/Medium)
图像的艺术形式或媒介，例如：photography, oil painting, digital art, anime, 3D render, concept art。

画质与细节 (Quality & Details)
永远包含高质量标签：best quality, ultra-detailed, 8k, masterpiece。
可以加入 HDR, sharp focus, cinematic composition, professional, extreme detail 等词。

光影与氛围 (Lighting & Atmosphere)
描述画面的光影和氛围，例如：soft sunlight, cinematic lighting, moody atmosphere, dramatic shadows, studio lighting。

色彩 (Color Palette)
描述整体色调，例如：vivid warm colors, pastel tones, monochrome, cyberpunk neon, golden hour。

附加修饰 (Extra Elements)
用来补充画面的独特感，如 dreamy, futuristic, surreal, elegant, romantic atmosphere。

## 限制
只用英文单词或短语，不要整句。
使用竖线 “|” 分隔各部分。
单词数量不超过 60 个。
Tag 按重要性从左到右排序。
只输出 Flux Prompt，不要解释。

✅ 示例
输入主题：少女在玫瑰花园里微笑
输出 Flux Prompt：
A beautiful young girl standing in a rose garden, detailed eyes, lips, nose, long eyelashes, soft smile | hyper-realistic photography | best quality, ultra-detailed, 8k, masterpiece, cinematic composition | soft sunlight, HDR, dreamy atmosphere | vivid warm colors, golden hour tones | elegant, romantic mood
```

Midjourney 提示词：
```
Midjourney Prompt 助理
你来充当一位具有艺术敏感度的 Midjourney Prompt 助理。

## 任务
我用中文告诉你一个主题，你的任务是根据这个主题构想完整画面，然后生成一份高质量的 Midjourney Prompt，可以直接用于 Discord 的 /imagine 命令。
Prompt 语法结构要求

使用 /imagine 作为开头，后跟 prompt 文本。
Prompt 包含以下主要部分（尽量简洁且丰富）：

主体 (Subject)：画面核心内容，用英文详细描述（人、物、景或抽象概念）。
若为人物，务必包含面部特征，如 eyes、lips、nose、expression 等。

媒介/风格 (Medium / Style)：例如 photography, oil painting, digital art, illustration, concept art 等。
环境 (Environment)：场景或背景，包括地点、氛围、时间等。
光影 (Lighting)：例如 golden hour、soft lighting、cinematic lighting 等。
构图 (Composition)：视角，如 close-up, aerial view, wide angle, portrait 等。
色彩与氛围 (Color & Mood)：如 vibrant colors, moody tones, pastel, romantic 等。
参数 (Parameters)：加在结尾，控制 aspect ratio、stylize、chaos、style、weird 等（如 --ar 16:9 --stylize 750 --v 6）。

## 推荐结构示例：
/imagine 主体, 媒介风格, 环境, 光影, 构图, 色彩氛围 --ar 宽高比 --stylize 数值 --v 版本号
可以使用 多重提示权重（multi-prompting） 通过 :: 语法调整关键词重要性（可选）。例如：
subject::2 environment::1 mood::0.5

## 限制
不要出现中文，prompt 必须是英文。
不要包含解释性文字，仅输出一行完整的 prompt。
保持词语简洁明了，不要超过 60 个词左右。
避免否定描述，若需排除元素请使用 --no 参数，例如 --no text, --no watermark。

## 示例
输入主题（中文）：
 “夕阳下海边戴草帽的少女微笑着看向远方”
输出 Midjourney Prompt：
/imagine a smiling young woman wearing a straw hat on the beach at sunset, digital painting, soft golden light, wide angle, warm pastel colors, serene romantic mood --ar 16:9 --stylize 750 --v 6
```

我们定义的 API 输入数据结构如下：
```
{
    "userQuery": "请描述一下这个图片",
    "img"： 图片二进制数据,
    "promptType": "" // 提示词类型 "midjouney" || "stableDiffusion" || "flux" || "normal"
}
```

因此开始节点要按这个输入结构设置：
![](img/18eec3607e1b705c3c36122edb22f918.png)

第二个节点做图片理解：先让豆包 1.6 理解图片，生成自然语言提示词。这个节点的用户提示词是：
![](img/82746a7b6085214aa389cd2de3a2de70.png)
```
## 图片描述助手
你是一个图片描述助手，可以理解用户提供的图片，并用自然语言描述出来

## 技能

用自然语言描述图片画面，并用模型能理解的语言描述，需要提供AI绘画模型能理解的语言描述

## 工作流

根据用户输入的图片{{img}} 和 需求{{userQuery}}进行图片处理任务
```

第三个节点是选择器，按条件匹配模型，相当于代码里的 if else。之后 3 个节点分别对应其余 3 类大模型生成节点，提示词前面已经写过；模型可选 deepSeek-V3.1，速度与效果都比较好。

再下一个节点是变量聚合，把前面 4 个模型的输出合并成一个变量输出：
![](img/9d3dcfcf00748265dc082a1b1719234b.png)

结束节点返回聚合结果：
![](img/f05273e79eb29cdc0a520e369d7afbdd.png)

工作流试运行通过后即可发布：
![](img/8ca1e091ff08c6ffb0c99bd9d6028380.png)

# 4.2 配置扣子 API

调用扣子 API 前，先创建个人访问令牌，再写入配置文件。

1. 前端 UI 开发

TIPS：过程中遇到问题，直接让 Claude Code 处理即可：
![](img/1296d2ce0cab43a6dcf65e07ac52e814.png)
![](img/7f5ab1017fc9f454b7cd27728081bdea.png)

# 5.1 Saasfly 框架速览

我们会用 Saasfly 这个开源 Next.js 框架。它已经集成了登录鉴权、用户管理、数据库、多语言、支付等 SaaS 常用基础能力，让我们能把精力放在核心业务上。

# 5.2 主要框架

Next.js：面向 Web 的 React 框架（使用 App Directory）；NextAuth.js：Next.js 的认证方案；Kysely：TypeScript 类型安全 SQL 查询构建器；Prisma：面向 Node.js 与 TypeScript 的新一代 ORM，也作为 schema 管理工具；React-email：用 React 组件渲染精美邮件的渲染器。

# 5.3 平台服务

Clerk：功能全面的用户管理平台；Vercel：轻松部署 Next.js 应用；Stripe：面向互联网业务的支付处理；Resend：面向开发者的邮件营销平台。
![](img/661d28fcd4208e8d8c6fcd5b8ca198e2.png)

而且这个框架开源，可以免费使用。

# 6. 安装与初始化

# 6.1 拉取源码

前面已经装好 git，直接打开 Saasfly GitHub 仓库，复制克隆地址：
![](img/98c493ba3ce8f5d8bf7bb436d5ebd6bb.png)

在终端执行命令：
```
git clone https://github.com/nextify-limited/saasfly.git
```
![](img/e6f554e30621d4284036279ef4c0f7ee.png)

# 6.2 初始化 Claude Code

用 Trae 打开项目目录：
![](img/3d96b677e79c335aeb531f9b972f93ef.png)

再开一个终端，打开 CC，执行 /init 做项目初始化，会生成一个介绍项目的 CLAUDE.md 文档：
![](img/163e1664448e7d818e87cee0a0386786.png)

这份文档会说明项目技术栈、主要功能和启动方式等；我们也可以把自定义编码规范写进去。

# 6.3 推送至 GitHub 仓库

把本地项目接进自己的 GitHub 账号，第一步是在 GitHub 上开一个新仓库，作为源码托管目的地。随后把项目当前指向的远端地址切换到新仓库 URL。

```
git remote set-url origin git@github.com:fuyunzhishang/imagePrompt.git
```

运行 git push，本地提交就会上传到远端。

![](img/05cc6550e58cd0b957b8d9a58c6e13b8.png)

回到 GitHub 刷新一下，代码已经出现在新仓库中。

![](img/38406fd651179ab9099430cf1a801072.png)

# 6.4 接入 Vercel

打开 Vercel，新建一个项目。

![](img/4352085e0b9cc6c086d959836ca3dc5f.png)

从列表里选中刚才建好的 GitHub 仓库进行导入，框架预设切换为 Next.js。

![](img/7fb917025733f5f27ab60cafbe09ab74.png)

1. 还原界面

# 7.1 环境配置与本地启动

首先安装项目所需依赖，并让它在本地跑起来。官方手册中记录了完整流程：https://docs.saasfly.io/zh-cn/get-started/manual-setup/

Saasfly 官方建议以 Bun 替代 npm，因此需要先装好 Bun。文档原话是：若想获得更流畅的体验，请用 Bun 取代 npm 或 yarn。Bun 本身可以通过 npm 来安装。

```
npm install -g bun # the last `npm` command you'll ever need
```

安装完 Bun 后，用它拉取项目依赖。

```
bun i
```

接下来生成 Prisma 类型。先确认终端定位在 saasfly 目录下，再执行 Bun 命令生成 Prisma types：

```
cd packages/db/
bun db:generate
```

运行后输出：

```
✔ Generated Kysely types(1.7.1) to./ prisma in 1.32s
```

配置环境变量：仍在 saasfly 目录内，把 .env.example 复制一份，将副本命名为 .env.local，然后填入你自己的变量值。

```
cd saasfly
cp .env.example .env.local
```

前提是有一个能连通的 Postgres 数据库；如果还没有，按文档提示先建一个。已经存在 Postgres 的，直接改环境变量即可；也可以在 Supabase 里新开一个库。

![](img/62c16e115888222cf843cdd29106eaed.png)

找到新库的密码等连接参数，逐一写入 .env.local 的对应项。

![](img/073f618f61719e456a9a2c965c32ff18.png)

![](img/81f560675c55edcf2c98d87d5a154474.png)

连接方式的选择要留心，直连模式不支持 IPv4。POSTGRES_URL 这一项必须在 .env.local 中声明：

```
# 格式例子：
# POSTGRES_URL="postgres://{USER}:{PASSWORD}@{DB_HOST}:{DB_PORT}/{DATABASE}"

POSTGRES_URL="postgres://postgres:123456@127.0.0.1:5432/saasfly"
```

![](img/178810344f641d6bd6a5cf5ea9175bfb.png)

接着用 Bun 建数据库表：

```
bun db:push
```

输出如下：

![](img/5730f963a9e79f3bc5fc93464eaaf04d.png)

回到 Supabase 控制台确认，表已经建好了。

![](img/b42419cf72f07c79b4cd3d2f3bc2d7b3.png)

启动本地 Web 服务。

```
# 注意要先切换到项目根目录
cd ..
bun run dev:web
```

![](img/2fb7cc61d35438e21ef18b05a8534741.png)

服务会监听本机 3000 端口。但打开浏览器却是 404，于是让 CC 来定位。日后碰到任何故障都可以交给 CC 处理。

![](img/986de045b32b7103039250357cb9d3a9.png)

问题根源在于 Saasfly 出厂默认走 Clerk 鉴权，当前没有配置所以抛错。Clerk 要注册账号、做一堆设置，我觉得太繁琐，索性让 CC 换成 NextAuth 鉴权。

![](img/d939ea42432174df057ccfc89fbd83b8.png)

```
 把鉴权改成NextAtuh    
```

![](img/06ec5b8bdd223914ca04eb30d680674b.png)

等几分钟，CC 完成了替换。

![](img/fe9ffcae3de071af6c1be10ec4138de5.png)

如果还有报错，把错误原文贴给 CC，让它接着修，直到跑通为止。

![](img/6c112cb42de52dbc3b110ec2b522795a.png)

顺利启动后，Saasfly 的默认界面就出现了。

![](img/eaaa963341a7a1c6902484d2a2942fad.png)

现在提交代码。建议小步提交，防止丢失，然后同步到远端。

![](img/9abe491cefbae4617c41365d80db9096.png)

# 7.2 前端界面搭建

# 7.2.1 落地页实现

落地页承担着承接网站流量的职责，用来介绍产品能力，并把访客导向二级功能页面。这里我们直接参照对标站点来做。然后把该页面交给 CC 还原，产出我们自己的登录页。

```
复刻这个页面，实现落地页面，完成后要测试没有报错
```

![](img/7963fcc2bba6a9b7f395cbc918f4806b.png)

几分钟后 CC 交付了结果。

![](img/437592b0673a927347bd1eb273fd5963.png)

有问题就继续让 CC 处理。CC 一般没法一次改到位，常常需要逐轮微调。我们根据它的产出逐步给出反馈。比如样式已经换好但文案还没动，就再让它改文案。

![](img/bb26bea0618b5cdb6e839055efaccd05.png)

页面已经初具雏形，先把核心功能做出来，细节留到后面打磨。

# 7.2.2 功能页实现

落地页就绪后，接着做功能页面。

![](img/70c1ad2b29ad043107a92e1ad67012dd.png)

```
根据这个页面截图，进行功能页面的开发，并在落地页加上链接导航
```

# 7.2.3 细节打磨

CC 的产出往往遗留不少小毛病，例如多语言文本硬编码、样式不统一等，需要围绕这些点持续让它改进。

1. 上线发布与长期运营

# 1. 联调、测试、发布

让 CC 把前端页面与后端扣子的 API 打通。扣子平台支持通过 API 触发工作流，官方说明在：https://www.coze.cn/open/docs/developer_guides/workflow_run，我们直接把文档丢给 CC 研究，由它落地相关能力。

```
实现一下image to prompat 的功能，需要调用扣子工作流来实现图片的提示词生成，步骤如下：
1\. 调用文件上传接口实现图片上传 这是接口文档 https://www.coze.cn/open/docs/developer_guides/upload_files
2\. 然后通过工作流API调用提示生成功能 生成API，这是接口文档 https://www.coze.cn/open/docs/developer_guides/workflow_run
3\. 接口鉴权的token 和workflow_id 配置到配置文件中
```

功能大体就绪。随后发布到 Vercel。

在 Vercel 创建一个项目，绑定我们那个 GitHub 仓库。

![](img/891989bf4e4cab320ab61473ea6e287c.png)

部署阶段若出问题就交给 CC，直到成功为止。由于环境差异，本地能编译通过、线上却失败，这属于正常现象。反复部署几十次后终于成功。

![](img/43d0126d3960f1f2a02630dcbef52855.png)

来访问一下。

![](img/eefce5dff74eb533ef5664a10783ea56.png)

部署完成后，Vercel 会分配一个默认域名。

1. 用户登录接入

先调整默认登录页的视觉样式，再接入 Google 登录。

![](img/61f80624db1bf0b378798ca359040f1a.png)

```
1\. 优化登录页样式，去掉saasfly的文案，改成imagePrompt
2\. 去掉github登录
3\. 实现google登录
```

CC 改完后，只需填好 Google ID 与 SECRET。Google 登录凭证需要申请：打开 Google Cloud，进入 APIs & Services，在左侧点击“凭证”。

![](img/099052dc1a336e0114f68dc056453514.png)

创建一个凭据。

![](img/91404c48531e1a68d363644c23f1d553.png)

类型选 OAuth 客户端 ID，应用类型设为 Web 应用。授权与回调 URL 填 http://localhost:3000；目前是本地开发阶段就填本地地址，上线后再替换为线上域名。等约 5 分钟再测登录。若登录失败，把错误详情交给 CC。

![](img/065093b5990d6d4274e6a3a89c6da864.png)

我碰到的问题是回调地址写错了，正确值应为 http://localhost:3000/api/auth/callback/google。修正后即可正常登录。

![](img/13821d94f99458013b40c272c4f5de2a.png)

![](img/96d5e0d3be30a89f6534b59eb7989061.png)

之后在 Supabase 后台就能看到已登录用户的信息。

![](img/cc7cf0845cb0c93d45b6ae71eaa614b2.png)

1. 域名绑定

网站发布后，需要为它绑定自有域名。域名可在阿里云、腾讯云、Porkbun 等平台注册，注册完成后做解析即可。Vercel 提供自定义域名能力：进入设置-域名，新增一个域名，再把解析记录填到域名服务商的 DNS 配置里。

![](img/f746d4343ad5341ed781b07d8a6724a1.png)

以我使用的 Porkbun 为例，把 Vercel 给出的 CNAME 记录复制到域名的 DNS 设置中。

![](img/54be68aefd735003bfb661e2353f86b3.png)

绑定完成后，别忘了把新域名补进 Google 凭证的授权 URL。

1. SEO 关键词布局

借助 AITDK 粗略分析关键词，先做一轮基础的 SEO 关键词规划。把这些关键词交给 CC，让它在落地页中合理分布。

```
对落地页做一下SEO关键词布局，需要围绕着几个关键词进行内容布局：image to prompt, impage to prompt generator, image prompt, prompt generator
```

从结果看，关键词的分布还算合理。

1. 数据监控接入

这里选用百度统计来做数据监控。先注册百度统计账号：https://tm.baidu.com/，然后添加站点。

![](img/7b12c31ec3a32542eb8d3c0abd0b9335.png)

拿到统计代码。

![](img/b8cb548fbc7ad38f2f857a4fd2344cdc.png)

复制这段代码，嵌入网页，再交给 CC 处理。

![](img/d89058bdd80485801e2fc3ab806243d8.png)

1. 运维工具快速入门

1. 服务器管理面板

先认识一下 BT 面板（宝塔）。这是一款图形化的主机运维工具，核心作用是降低建站、运维与管理的门槛。它提供基于 Web 的可视化操作界面，即便对 Linux/Windows 命令行不熟，也能比较快地部署与维护网站、数据库、FTP、SSL 等服务。

![](img/70e9647e9daca1c52f21b7549d40c5a6.png)

1. 功能一览

- 环境一键搭建
  - 覆盖 LNMP（Linux + Nginx + MySQL + PHP）、LAMP（Linux + Apache + MySQL + PHP）、Tomcat、Node.js、Java 等常见组合。
  - 支持一键安装、升级、切换 Nginx、Apache、PHP、MySQL/MariaDB 等组件的不同版本。
- 站点管理
  - 快速建站、绑定域名、配置 HTTPS（免费 Let's Encrypt 证书）。
  - 提供伪静态规则、301/302 重定向、反向代理、负载均衡等能力。
- 数据库管理
  - 兼容 MySQL、MariaDB、PostgreSQL、MongoDB。
  - 自带 phpMyAdmin、Adminer 等可视化工具，同时支持远程连接。
- FTP/SFTP 管理
  - 内置 FTP 服务，支持按用户分级授权。
- 文件管理
  - 在 Web 界面完成上传、下载、编辑、解压缩。
  - 支持在线修改代码。
- 安全管理
  - 防火墙：端口放行、IP 黑白名单。
  - 系统安全体检，提示风险配置。
- 计划任务
  - 定时备份数据库与站点文件，支持自动清理日志、按计划执行脚本。
- 监控能力
  - 实时查看主机 CPU、内存、硬盘、流量等指标。

![](img/947eb4ff89470258032699fb5b7e22c5.png)

![](img/6e867addd494a8b4f3b16890d4d0168d.png)

1. 优势

- 门槛低：对新手及非专业运维人员比较友好。
- 功能齐全：建站、运维、管理、监控都能在同一个面板内完成。
- 插件生态丰富：应用商店中有缓存、负载均衡、监控告警、云端备份等插件（部分付费）。
- 跨平台：Linux 与 Windows 均可运行。

1. 不足

- 安全风险：BT 面板默认监听 8888 端口，若未修改默认端口、限制来源 IP、设置强密码，容易成为扫描攻击的目标。
- 性能开销：相较纯命令行操作，会额外消耗一部分主机资源。
- 商业化：基础功能免费，高级插件与部分能力需付费。

1. 适用对象与场景

- 个人站长、独立开发者：快速搭建 WordPress、Discuz 或类似 Shopify 的系统。
- 中小企业：建站、内部系统部署。
- 学习测试环境：练习 LNMP、LAMP 环境搭建。

1. 安装方式

详见官方文档：https://www.bt.cn/new/download.html。

通用安装脚本：

```
if [ -f /usr/bin/curl ];then curl -sSO https://download.bt.cn/install/install_panel.sh;else wget -O install_panel.sh https://download.bt.cn/install/install_panel.sh;fi;bash install_panel.sh ed8484bec
```

CentOS/OpenCloud/Alibaba：

```
url=https://download.bt.cn/install/install_panel.sh;if [ -f /usr/bin/curl ];then curl -sSO $url;else wget -O install_panel.sh $url;fi;bash install_panel.sh ed8484bec
```

Debian：

wget -O install_panel.sh https://download.bt.cn/install/install_panel.sh && bash install_panel.sh ed8484bec

Ubuntu/Deepin：

```
wget -O install_panel.sh https://download.bt.cn/install/install_panel.sh && sudo bash install_panel.sh ed8484b
```

1. 项目部署到服务器

# 1. 部署方式对比：

- 自有主机：约 16 美元/月，时间投入少，可维护性高。
- Vercel + Supabase：20 美元 + 25 美元，配置较繁琐，可维护性中等。

用自有主机部署更省事，不必折腾太多配置，想装什么工具都随意。一台机器能承载多个站点，通常 2 核 2G 的配置至少能跑几十个站点。这套思路是通用的，不局限于某个框架。

# 2. AI 辅助部署

AI 部署需要能力较强的模型，例如 Claude Code，比较适合测试环境。线上环境尽量不要让 AI 直接操作，操作前请先备份数据或创建快照。主机可以沿用前面用过的 DigitalOcean 或其他云平台。AI 的表现不一定稳定，可能需要多尝试几次。

# 2.1 第一步：在设置中上传公钥

这次改用 SSH Key 登录，主要原因是 Windows 环境下 AI 无法用明文密码登录服务器。需要先上传公钥，创建主机时选中对应公钥，系统才会加载它。

![](img/3714947d45ed3ee68f8d8ac6d02ab12a.png)

# 2.2 开一台云主机

![](img/6d237bc551ddca6ac4adcbb3ebcced10.png)

# 2.3 远程登录验证

机器起来后，用 SSH 连上去确认能正常进入。

![](img/787c0a69132700d088286e037467fce0.png)

# 2.4 Claude Code 自动搭建

先结合当前环境，把目标和需求尽量讲具体，别让 AI 靠猜。

![](img/04186f01844b9851d4aa31fb8beb4b89.png)

等它自己跑完。

![](img/897c348f6b2ab1939ed696cbfec61df8.png)

# 3. 手动上线方案

如果自动流程不称手，也可以手动来。宝塔面板先装好，安装方法前面已经讲过；PostgreSQL 直接在宝塔里选环境安装。

![](img/45425d08c15c1463e832a3926999f450.png)

建一个数据库。

![](img/46138b18f723c7798ba7e7b6fad2b56a.png)

连库并初始化表结构。常见故障是默认配置没开放公网监听、权限也没配好，导致连不上；真遇到就让 CC 登机器改。

![](img/5d666d44ee2a3a6528df02bd784f7808.png)

![](img/4a1d8247980107ba0eadd2df107844f0.png)

![](img/3610f7c681fae1bf9d62696814270c11.png)

同步完成。

![](img/00b830c4a6c4850f6093e508bc7f5ee3.png)

先在测试环境跑通项目，再编译、打包。

![](img/7d3b4b8e19747600be59493927b38aa2.png)

如果 Vercel 相关配置报错，直接删掉对应配置，这套方案不走 Vercel 托管。

![](img/9e35e62ee5ac9a0d1d55d10547046aaf.png)

![](img/8ac622982c19500c2ec433b914fd137a.png)

Node 和 Pm2 都从宝塔里装。

![](img/d7fc22bf3fccffd8698f27371f30dcf9.png)

打开 Node.js 版本管理，刷新列表，安装 22.19.0 这个长期支持版。

![](img/ab00f55e90ab401e8f594af34aad8f29.png)

命令行默认版本也要切到它。项目还要 bun，一并装上。

构建产物在 /saasfly/apps/nextjs，压缩后传到服务器 /www 目录。

![](img/3560a2af7741ff69d4c1acd01385fdc1.png)

![](img/81d5187572172ea9160e94d299eafece.png)

![](img/c89d35fdd392929da87dac9663442ce3.png)

最后用 pm2 拉起服务。这个框架第三方依赖耦合多，先让 AI 把有问题的包剥掉，否则生产环境容易报错；报错后再让 AI 修，会比较花时间。嫌折腾就换别的框架。

![](img/ac0a66d7e9fef3261954cfaeb9136dc5.png)

![](img/9d546b64e1f45e945f2717d54286ddb8.png)

# 收尾：部署坑点汇总成文档

部署期间碰到的故障和坑，我请 AI 整理成了一份文档。

1. 工具站盈利升级

# 1. 本章速览

这一章把工具站商业化拆成两块：一块是产品和支付，一块是流量。前者包括打磨产品、接入支付、设计订阅档位、搭好收款通道；后者覆盖搜索、社交、买量，目标是让增长可持续。

实战步骤：

产品与支付：
- 先弄清境内、境外支付通道各自的门槛，再做选择；
- 规划订阅方案，覆盖 0 元、起步、专业、企业几档，讲清设计逻辑和常见结构；
- 拆解 Stripe 和海外主体注册流程，包括手机号准备、注册地选择（英国/美国）、Firstbase 一站式服务，以及 Mercury 银行优势；
- 开通 Stripe 商家账号，并用 Wise 做个人收款和提现。

流量运营：
- 搜索优化：关键词挑选、内容建设、权重提升、体验优化；
- 社交传播：海外看 Twitter/X、Reddit、YouTube Shorts、TikTok、LinkedIn；国内看📕、抖音、知乎、🧣，梳理常见打法；
- 付费买量：谷歌广告、Meta 系广告、TikTok 广告等渠道的精准定向、转化追踪和规模化投放。

# 本章进阶地图

学完并实操本章，即可完成路线图中的：

第五阶段：商业化进阶（约 2 天）

1. 产品订阅与收款通道：定套餐、接支付（约 1 天）。
1. 流量打法：理解搜索、社交、买量（约 1 天）。

# 2. 打通支付

现在接支付大致四条路：

- 大陆个人身份几乎没戏，先得有香港银行卡；
- 用个人名义申请港卡，封号概率不低；
- 海外企业实体最稳；
- 境内企业实体也相对可靠。

# 3. 订阅方案与收款通道

只要工具站准备收订阅费，收款方式就不能临时抱佛脚。常见两条线：

- 个人侧可以走 Creem；
- 企业侧建议 Stripe，并且用海外公司名义注册更稳。

本章重点拆 Stripe 和配套准备；Payoneer、Lemon Squeezy、Paddle 等渠道可以自己试。

# 3.1 订阅档位怎么设计

订阅档位不是简单列价格，它决定商业模式怎么转：既要让不同人群各取所需，也要让收入和增长同时成立。

# 3.3.1 设计逻辑

1. 按人群分档

0 元档负责降低门槛、做大用户池；付费档给核心能力和效率；高阶档面向专业或企业场景，再叠加 API、协作、专属服务等价值。

2. 价格锚点

档位至少放三档，低中高齐备。多数人会自然落向中间，这就是折中效应。

3. 差异化维度

差异可以落在四类地方：额度（视频时长、生成次数、存储空间）、权限（高级功能、API、批处理）、服务（客服响应、成员席位、白标/定制）、结算（月付/年付，年付让利）。

我们产品的会员档位就拆成了多级，下面这张图是结构：

![](img/861b39b7851ecacb781465c9092a61ac.png)

# 3.3.2 常见档位模板

下面用 AI 工具/视频剪辑 SaaS 举例，给出一种可套用的档位模板。

1. 0 元版（Free）

目标：拉新，并让用户建立使用习惯。

内容：限制部分功能（如导出结果加标识）；每月设置使用上限（如视频处理 30 分钟、AI 调用 100 次）；提供社区支持。

2. 起步版（Starter / Pro）

目标：个人用户或刚起步的创作者。

定价：月费 9.9–19.9 美金。

内容：去水印；提高额度（如每月 10 小时视频）；开放常用高级功能（字幕编辑、批量导出、AI 解说）；邮件客服。

3. 专业版（Advanced / Creator）

目标：重度个人创作者或小团队。

定价：月费 29–49 美金。

内容：更高额度（每月 50 小时视频）；全功能解锁（API、自动化工作流、跨平台发布）；团队协作（3–5 人）；优先客服（实时聊天）。

4. 企业版（Enterprise / Custom）

目标：中小企业或大客户。

定价：月费 99–299 美金，也可定制报价。

内容：无限额度或大幅扩容；专属客户经理；白标/二次开发能力；发票和法人合规支持；SLA（服务级别协议，保障稳定性）。

# 3.2 收款通道

# 3.2.1 Stripe 与海外主体注册

先回答一个问题：为什么大家愿意折腾海外公司？因为收款和付款需要稳定通道，也需要一个海外银行账户。很多海外服务对大陆身份不友好，风控也更紧，换成海外主体后，接入会顺很多。

号码准备有两条常见路线：

- 英国 giffgaff：180 天发一条短信即可保号，成本约 £0.3，官网能免费申请；
- 美国 Ultra Mobile PayGo：月租约 $3；
- 懒得自己弄，也可以在淘宝或京东上找人代办。

注册地怎么选：

- 英国公司办理快、成本低，常用 [1st Formations]，开 Wise 企业账户即可；
- 美国公司更适合做业务扩张，个人开发者常选 Wyoming 的 LLC。

我走的是 Firstbase，整体像在用 SaaS：公司注册、地址公证、EIN、银行开户都能代办。

流程大致四步：

1. 注册 Wyoming LLC；
2. 租一个私人邮箱地址做地址公证，用 Notarize 视频完成 1583 Form，身份证明（护照或驾照翻译件，电商平台可代办）要准备好，照片和地址需出现在同一页；
3. 让 Firstbase 代办 EIN，约 10 个工作日会收到 IRS 信件；
4. 开 Mercury 账户，把 EIN 和护照关联后，通常 1 个工作日内过审。

四步走完，你手里会有：公司实体、EIN、私人地址、银行账户、海外手机号。

Mercury 的好处：

- 虚拟卡数量不限，能按商户做限制，订阅和退款管理方便；
- 虚拟卡可绑支付宝，单笔 200 元以内免 3% 手续费；
- 能收账单地址信件，比如 Google AdSense 的验证信；
- 实体卡也能申请，再转寄回国。

Stripe 商家号开通：

- 用 EIN 就能注册；
- 页面可切中文填写；
- 个人验证交护照；
- 提现账户绑 Mercury；
- 建议顺手把 Lemon Squeezy、Paddle 也注册了做备用，不过它们要验证产品站点。

Wise 个人账户：

- 支持大陆身份和护照注册；
- 入金可以走 Mercury 转账，也能在电商平台代充；
- 实体卡（含 3 张虚拟卡）费用 $9，激活后可改地址再申请；
- 提现能到国内银行卡、支付宝、🛰️，手续费低，汇率比国内结汇更划算。

👉 想找更稳的结汇方式，可看参考资料。

# 1. 搜索流量：SEO 玩法

在我的判断里，产品永远先于流量：先看它是否真的解决用户问题。所以我们反复强调 PMF，也就是产品与市场的匹配。匹配度足够高，流量通常不会缺；特斯拉、🛰️这种产品，本身就不靠营销。但新产品冷启动，还是得先弄来一批种子流量，等产品跑起来，再决定放大方式。

搜索优化更像慢变量，回报周期长，但能持续带来免费访客。

关键动作：

- 选词：贴近真实搜索意图，找相关性高、竞争没那么凶的长尾词；可用 Google Keyword Planner、Ahrefs、Semrush 辅助；
- 内容：持续做落地页、教程、问答和博客，把用户搜索背后的疑问讲透；
- 权重：靠友链、投稿、媒体报道积攒高质量外链；
- 体验：页面打开速度、手机端适配、交互顺手，都会影响停留。

适用场景：适合愿意慢慢沉淀品牌资产的工具站、知识站。

案例：TAAFT、Futurepedia 这类海外 AI 导航站，用海量长尾页面持续吃自然访问。

# 2. 社交传播：SMM 打法

社交平台适合快速起量，关键是让内容自带传播钩子，借平台机制让用户愿意转发、讨论。

常见平台：

- 海外：TikTok、YouTube Shorts、X/Twitter、Reddit、LinkedIn；
- 国内：知乎、📕、抖音、🧣。

常见打法：

- 短内容演示：用前后对比、操作演示、短教程把卖点演出来；
- 热点互动：跟话题、参与讨论，在评论区做轻量引导；
- 达人借势：找 KOL 或有影响力的人快速放大传播。

适用场景：冷启动期很合适，尤其是视觉化强、话题性高的产品。

案例：换脸与绘画类 AI 产品，很多先在 TikTok 用效果视频引爆，再放大获客。

# 3. 付费买量：Paid Ads

买量是获取精准用户最快的路径，用预算直接换流量和转化。

常见渠道：

- 海外：谷歌广告（搜索、展示、YouTube）、Meta 家族（Facebook、Instagram）、TikTok 广告；
- 国内：百度、抖音、快手。

操作关键点：

- 定人群：按兴趣、地区、年龄、消费力筛目标；
- 看转化：用像素或转化 API 回传行为，持续优化投放；
- 先小后大：先用多组小预算测试，筛出 ROI 高的素材，再逐步加码。

适用场景：需要快速拉新，或想验证需求真伪时，适合用。

案例：一些 SaaS 团队会先用谷歌关键词广告加免费试用，测市场反应，再决定是否长期加码。

# 尾声

路是一段段走出来的。财富与能力增长，背后都有复利在起作用。它不追求一夜翻盘，而是把持续行动换成越来越大的斜率。眼下这件事，本质上是一笔低风险的长线投入。前期多半没有即时反馈，可每学一点、每做一次、每拿到一个小结果，都会沉淀成以后爆发的底牌。风口到来时，你手里的能力与资源，会让你获得高于平均线的回报。

所以，人和人的分野，常常不是某个瞬间决定的，而是长时间累积的结果。

从今天起，开始攒你的复利；把耐心和坚持当成本金，让未来的你感谢此刻动手的自己。

最后，愿你的产品能越过下面这条增长曲线。