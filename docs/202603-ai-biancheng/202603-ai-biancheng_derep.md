# 零基础三件套：装好、跑通、做出一个产品

> 原始资料：  
> [https://my.feishu.cn/docx/Fv3ldAuehoDvWuxMxdicmrSDnEf](https://my.feishu.cn/docx/Fv3ldAuehoDvWuxMxdicmrSDnEf)  
> 同步地址：  
> <https://my.feishu.cn/sync/Lj5sd8APisk896bxImEcYvjMnlF>

# 引言：开船之前

## 第一课：先弄清这趟要做什么

### 零基础怎么进这个项目？

1. 项目情况

模型能力这两年涨得很快，外行也能靠 AI 把脑子里的点子做成能用的东西。赚钱办过几期 AI 编程方向的航海，反馈里出现最多的一句是“还是卡在开头”。

所以这一期换了打法：不从深奥处讲起，而是挑最省力、最顺手的工具组合切进去，用 Claude Code、Skills 和近期声量很大的 OpenClaw（圈里叫小龙虾）把门槛削平，让工具真正落到自己的业务里。

目标就三句短话：装得上、跑得动、做出一个真能用的东西。

为什么偏偏是这三样？

**Claude Code**

在面向零基础的 AI 编程工具里，它算脾气最好的一位。不需要你会写程序，把想要什么讲清楚，它就能出代码、搭产品。前几期航海里，不少圈友已经靠它做成了网站、小程序和 App。

**Skills**

它负责接管那些天天重复的杂活。写👸号、发📕、整理表格，过去得在 n8n 里拖节点、连线条，如今只要用一句话把需求说清楚，流程就能建起来。

**OpenClaw**

这是眼下讨论度很高的 AI 助手。你建好的 Skills 可以交给它跑，相当于一个不用下班的人，替你盯邮箱、按点发内容、归置文件。

三样都用顺之后，分工自然就出来了：Claude Code 管把东西做出来，Skills 管把重复动作自动化，OpenClaw 管全天候执行。串在一起，才是一条完整的 AI 工作流。

考虑到大多数人对这几样工具只停留在“听说过”，本期把重心压在入门和上手。

必修部分从环境准备讲到安装、基础操作，先把三个工具跑通，再放进真实场景里练手——比如用 Skills 做自媒体自动化、改漫剧剧本，用 OpenClaw 搭个人知识库、做 IP 型👸号自动化、配一个专属 AI 客服。

选修部分留了进阶内容，像开发 AI 应用类 Skills、用 OpenClaw 生成 AI 漫剧这类有难度的案例，给愿意继续钻的船员。

![](img/e3c47a8ff1f3510c149a297c671309af.png)

1. 项目完整操作思路

**2.1 项目完整操作思路**

先啃下 Claude Code 的安装部署（关键）> 跑通 Claude Code 的新手案例 > 再搞定 Claude Skills 的安装部署（关键）> 跑通 Claude Skills 的新手案例 > 接着完成 OpenClaw 安装部署（关键）> 最后跑通 OpenClaw 的新手案例。

![](img/26a3ab9060b3a8496ced6891260b5adb.png)

**2.2 操作重点**

手册里会同时出现 Claude Code、Claude Skills、OpenClaw 三个工具，数量看着吓人，其实不必慌。把 Claude Code 装顺之后，剩下两个的安装与使用会轻很多。

更希望大家借这段过程练出一个习惯：有问题先丢给 AI。照着手册操作时，不管是报错还是卡壳，截图发给 Claude Code，让它帮你判断、给方案。

这样带走的不只是 Skills 和 OpenClaw 的用法，更是一套用 AI 处理麻烦的思路，把工具变成业务里的助力。

**2.3 新手入门建议&避坑指南**

**新手入门建议：**

• 完全没碰过代码，能跟上吗？答：能。航海从装环境、认工具起步，提示词和案例都是现成的，带着你一步步完成部署和练习，不要求你会写代码；每个案例都配了视频和图文，照着走不容易掉队。

• 一定要买 Claude 官方订阅吗？贵不贵？答：不用。这次主要用国产的 MiniMax2.7 去驱动 Claude Code，部分套餐 50 元/月；对比官方 20 美元/月，花费少一截，也不受网络限制。

• 搭建时蹦出报错、或者不会操作怎么办？答：报错太常见了，别被吓住。我们会尽量把流程做稳；实操中卡住就先问 AI，也可以在群里举手找教练。

• Skills 跟 n8n、Coze 差在哪？答：Skills 属于“说出来就行”的一类，用自然语言描述需求即可生成；n8n 和 Coze 属于“拖出来”的一类，要摆节点、连线条。前者更省事、更聪明，还能自动触发，复杂工作流不必手动搭。

**风险挑战和应对建议：**

挑战一：编程工具门槛不低，本地环境配置容易翻车。对策：手册按 Windows、Mac 两套步骤拆开演示，从零带你装 Git、VS Code、Claude Code，还整理了常见报错截图对照表。碰到“没有权限”“命令无效”之类，照着示例一步步查；视频和图文教程也可以同步看。

挑战二：Skills 建不出来，或者效果不如预期。对策：效果好坏，很大程度取决于需求说得够不够清楚。起步阶段先照手册的步骤搭（👸号自动生成、📕自动发布之类），流程熟了再自己动手。手册里堆了不少现成案例，可以直接拿来改。

挑战三：实际操作时发现跟手册对不上。对策：不用慌。每台电脑的系统版本、环境都不一样，出现差异很正常。把结果截图发给 AI，问它这是什么、为什么会这样、报错该怎么改，通常就能往下走。

风险一：AI 编程本身有难度，先做好心理准备。对策：心态放开放平，付出一分才有一分回响，每次学习都是往前挪一步。同时把“有问题先问 AI”练成肌肉记忆——装好 Claude Code 之后，卡住就去找它要答案。

风险二：OpenClaw 部署门槛偏高，本地跑还有隐患。对策：本期主推云服务器部署（腾讯云或阿里云），手册里有详细教程，把难度压下来。先装起来用上再说；同时权限别放太宽，避免文件被删了还不知情。

风险三：Token 掉得快，成本要盯住。对策：模型用得克制些，别动不动批量生成。OpenClaw 跑任务是要烧 Token 的，把执行频率设好，减少无意义的重复动作。

**2.4 开船前必备工具**

• 能正常访问外网的环境

• 飞书账号（OpenClaw 集成要用）

• Claude 账号，或 MiniMax / GLM-5 / Kimi 等国内模型（部分最低 50 元/月）

• 云服务器（腾讯云或阿里云，部署 OpenClaw 用），入门套餐 20 元/月起

• 一台能正常干活的电脑（Windows、Mac 都行，Mac 更省心）

AI 时代已经铺到脚下，普通人想往上走，从 AI 编程切入是条实在的路。往前走一步，就有一寸的欢喜，愿你把这段入门之旅走得踏实。

![](img/eda5047bcedbb9e0ca507069411e1e59.png)

# 必修篇：

## 一、Claude Code：安装与部署

### 01.入门：先认识 Claude Code

1. 本章概要

💡引言里已经见过 Claude Code 这位 AI 编程助手，大概也好奇它到底能把开发效率抬多高。可工具再强，只停在概念上，也帮不了你解决具体问题。

现在该动手了——把它装进自己的电脑。本章带你跨过从“知道”到“做到”的第一道坎，亲手把 AI 编程环境搭起来。手头的家伙什儿不趁手，后面的事都难顺；基础环境配好，才算真正站上起点。

本章会带你亲手完成：

• **搭好底座**：认识并安装 Git、Node.js、VS Code 这些必需的组件，让电脑具备跑 Claude Code 的基本条件。

• **把工具装上**：跟着学 Mac 与 Windows 下用命令行正确安装 Claude Code，摸清最基础的终端指令，让 AI 助手随时叫得动。

• **接国产模型**：用 cc-switch 把国产模型接进来，绕开网络与支付的麻烦，做到便宜、稳定地本地运行。

• **做出第一个产品**：装好之后，照案例一步步把那个早读工具做出来，亲身感受 AI 开发产品的路子。

学完这一章，你就不只是站在旁边看 AI 编程的人了：自己的 Claude Code 能装好，也能借它做出一个产品。动手吧，给后面的路垫上第一块石头。

💡

**本章航线图**

把本章的学与练做完，就走完了航线图的第一段。

第一阶段：装好并部署 Claude Code（约 7 天）

环境配置到位（约 5 天）

熟悉 Claude Code 的界面与常用操作（约 0.5 天）

跑完第一个实战案例（约 1.5 天）

![](img/6a06080d13eddb134d98ef0b12e27437.png)

2. Claude Code 是什么

**提醒：想装、想用 Claude Code，得先准备好能访问外网的环境。**

**一句话讲清**：它是一位能看懂你的代码库、也能用日常语言陪你一起写代码的编程助手。

**正式一点的解释**：底层是 Anthropic 的大模型，针对写代码这件事做了加强——能处理长上下文、按项目整体改写、自动生成与修复、解释和重构代码等；既能待在命令行里干活，也能跟编辑器、项目工具链配合，从零搭起一个项目，也能应付日常维护。

作为 AI 编程工具中的一员，Claude Code 让没有技术背景的人也有机会把产品做出来。

从前，想法要落地成能用的东西，得靠专职程序员一条条写需求。现在风向变了：哪怕你完全看不懂代码，也能借这类工具把点子迅速变成实物。这不是小修小补，而是把旧规则整个翻过来。

在赚钱，这样的例子一抓一把：不少圈友一行代码没写过，却用 Cursor、Claude Code 这些工具，真真切切做出了能跑的应用。有人做了面向海外的工具站，有人搭起自动化流水线，还有人做的小程序已经能带来收入。

差距早已不是“快一点”的层面。懂 AI 编程和不懂的人放在一起，产出可能差十倍，甚至百倍。一个会和 AI 配合的人，一天能顶过去一个小团队一周的量。更要紧的是，“谁能创造价值”这件事正在被重写：技术不再是那道墙，想法与执行力才是。

有了 Claude Code 这类工具，八成精力不必再耗在敲代码上，可以挪到真正要紧的地方——创意、产品设计、用户体验。实现部分交给 AI；你只管想明白“做什么”“为什么做”，“怎么做”由它接手。时间和精力就这样被松绑出来。

3. 为什么要用 Claude Code

从前想当开发者，先得抱着厚书啃术语、啃概念，再去折腾框架和配置。学个半年只是起步价，时间成本高得让人退缩。很多人就在这一段掉了队——不是脑子不够用，而是坡太陡。

AI 把规则改了。今天最值钱的能力不是背语法，而是会跟 AI 打交道：把需求说明白，用最普通的语言告诉 Claude Code 你要什么。它会照你的描述出代码，还常给几种方案。你要做的是挑出最对路的那一种，再接着聊——“这段逻辑能不能改一改”“能不能补个导出”。几轮来回，项目就在你俩的配合里长了出来。

不同阶段的人，用它的方式也不一样。

**对新手**

• **起跑快**：不会写也能跑起来——需求说清楚，它给你一份能执行的初稿。

• **学得省力**：让它一行行讲、对比不同写法、点出 bug 的根因，边做边学比死记语法轻松。

• **不怕报错**：出错就让它定位，顺手给出修法和测试样例。

**对老手**

• **产出翻倍**：样板和重复活交给它，人把心思放在架构、边界和质量上。

• **原型飞快**：过去一周才成形的雏形，半天就能搭出来；还能同时试几条技术路线。

• **质量有托底**：代码走查、补注释、写测试都交给它，技术债少欠一点。

**对团队和项目**

• **经验显性化**：把藏在脑子里的做法写成对话、注释和脚本，新人上手更快。

• **沟通变短**：需求、接口、验收标准都在对话里定下来，来回拉扯少一些。

下面从几个维度看看传统编程和 AI 辅助编程的差别：

| 维度 | 传统编程 | AI 辅助编程 |
| --- | --- | --- |
| 定义与驱动 | 人自己写代码、定逻辑、排流程，“做什么、怎么做”都由开发者拍板。 | 借助大模型、代码生成与补全等工具来产出、建议和优化代码，项目由“人 + AI”共同完成。 |
| 编码工作量 | 算法、流程、结构、接口、细节，全得从零设计。 | 重复、模板化、样式化的部分多由 AI 代劳，人负责提需求、验收和盯质量。 |
| 技能重心 | 看重语言熟练度、逻辑、数据结构、算法与架构。 | 除传统功底外，更看重怎么跟 AI 配合、怎么写出好提示、怎么验证产出、怎么管住 AI 生成的系统。 |
| 速度与效率 | 需求明确、结构规整时效率不错，遇到大量重复或模板任务就慢。 | 提速明显，尤其在样板代码、重复逻辑和原型阶段。 |
| 质量与可维护性 | 结构清楚，逻辑可追溯，维护责任明确。 | 出得快，但大项目里容易出现可读性差、结构重复、隐藏缺陷或安全风险。 |
| 学习门槛 | 语言、算法、工程思维都要花时间，新手起步慢。 | 新手能更快拿到能跑的代码，门槛降下来；可以在 AI 编程里边做边学。 |
| 适用场景 | 高复杂度、需求模糊、需要创新、质量要求高的项目。 | 重复任务、快速原型、标准模块、初稿撰写、提效场合。 |
| 工具与生态 | 传统 IDE 加手写或模板代码。 | 代码生成、补全、语义搜索、错误检测、自动测试等 AI coding 工具越来越普及。 |

![](img/4d49429355050ff555a3a01439d7b112.png)

4. 安装 Claude Code 时常见的概念

动手安装之前，先把几个会反复撞见的核心名词弄明白。名字看着陌生，角色其实很清楚；搞懂它们，也就摸到了 Claude Code 运转的底子。

**⚠️提醒：下面只是名词扫盲，安装时碰到不至于发懵，不必当成重点内容死磕。**

3.1 Git 是什么

Git 是一套**代码版本管理工具**，你每改一次代码，它都记一笔，像一台时光机。写过的内容能查、能退、能对比；不管是多人协作还是自己单干，都不至于手一抖改崩，或者想不起昨天动了哪里。

放到 Claude Code 的场景里，Git 的分量更重：你让它改代码、生成代码或重构时，改动历史会被自动留下，AI 动手前后的版本随时能对照。它甚至能直接读 Git 的提交记录，帮你理清项目这一路是怎么变的。一句话，Git 管记，Claude Code 管想，两个搭在一起，开发才又稳又快。

![](img/d97bc650d728af3f68b0d71c67c76412.png)

想先补补 Git 的入门知识，下面这个视频对新手挺友好，可以看看。

https://www.douyin.com/video/7459207071368629516

3.2 VS Code 是什么

VS Code 是微软做的轻量级免费代码编辑器，也是眼下全球最流行的开发工具之一，主流语言几乎都认，插件生态以万计。

它的好处是简单却不弱：界面干净、打开迅速，调试、预览、运行都能直接在里头完成。Claude Code 写出来的代码，都可以放进 VS Code 里看、改、跑。

打个比方，VS Code 像一款写作软件，只是稿子换成了程序；Claude Code 是替你起草的 AI，VS Code 则是你改稿用的那个编辑器。

下图是 VS Code 刚打开时的样子。和普通软件没多大差别，无非菜单和按钮多几个。

![](img/9f0590869d56353e5506e9d548781322.png)

3.3 MiniMax2.7 是什么

MiniMax 2.7 是一款编程能力相当扎实的模型，背后的公司叫稀宇科技——名气可能不如智谱、月之暗面那么响。

把 Claude Code 想成一件工具，工具要动起来得靠脑子，这个脑子就是模型；这次登场的是 MiniMax 2.7。

对国内用户来说，它最讨喜的地方是稳定可用，不被海外网络卡住。Claude Code 支持换“驱动模型”，用 MiniMax 2.7 顶替 Claude 官方模型，编程能力照样在线。

**Claude Code：外壳不变，模型可换**

先给结论：Claude Code 主要负责外层操作与调度，真正负责推理的“脑子”可以是 MiniMax2.7。Claude 服务连不上时，换成国产模型，代码生成与思考仍能继续。

![](img/90d6a699cee7eac3ea5bf64998b9c6c0.png)

可选模型不只 MiniMax。智谱推出的 GLM5、月之暗面面向编程场景的 Kimi for Code，也能接入这套流程。就现阶段适配 Claude Code 的稳定度和完成度而言，上述三家表现相对更好。

3.4 终端（Terminal）指什么

终端可以理解为操作系统提供的文字入口。人们平时习惯点鼠标开软件，开发者则更愿意在终端里敲命令，比如建目录、装程序、跑项目。它比图形界面诞生得更早，是接触系统底层的一条通道。

学 Claude Code 时，终端就是人与 AI 协作的场地。由于 Claude Code 属于命令行工具，没有图形面板，所以安装、启动、登录，甚至向它提问，都得通过终端输入命令完成。你可以把它当成“AI 的传声管道”：这边下指令，那边给回应。

macOS 自带 Terminal，Windows 自带 PowerShell 或 CMD。掌握少量基础命令，就能开始操作编程世界。

**终端（Terminal）**

它本质是命令行界面（Command Line Interface，简称 CLI），用来直接和操作系统交互。输入命令后，可以完成：

- 建立文件夹
- 启动服务器
- 安装软件
- 查看系统信息

它不靠鼠标点击图形界面（GUI），而是由文字命令驱动系统。

**常见终端：**

| 系统 | 常见终端软件 |
| --- | --- |
| macOS | Terminal、iTerm2、Warp |
| Windows | PowerShell、Windows Terminal、CMD |
| Linux | GNOME Terminal、Konsole、Alacritty |

例如 Windows 的 PowerShell，界面大致如下：

![](img/c2f2667f46f3cea04eb962caa800e465.png)

![](img/69d963f6b9facc313167aff566f5c266.png)

3.5 命令行（Command Line）到底意味着什么

命令行并非某个具体软件，而是一种用文字指挥电脑的操作方法。例如输入 node -v 可查看 Node.js 版本，输入 cd project 会进入指定文件夹。

它最大的优点是精准、迅速、可自动化，尤其适合开发场景中的批量任务。

Claude Code 的每一步都依赖命令行：安装、登录、调用 AI、运行项目，乃至新建文件，都绕不开它。刚上手可能觉得这种方式有点“原始”，但熟悉几个常用命令后，你会发现它比图形界面更自由、更高效。

换个说法：终端是场地，命令行是你在这个场地里使用的沟通方式。掌握这门“语言”，Claude Code 才能理解你的请求。

3.6 GitHub 是干什么的

GitHub 依托 Git，提供云端代码仓库服务，同时也是全球规模最大的开发者社区。Git 更像本地保存系统，GitHub 则承担云端备份库的角色。

它除了远程存放代码，还支持全球开发者协作、开源与复用。Claude Code 能直接读取 GitHub 仓库中的内容，例如“分析某个开源项目的结构”“帮我改某个仓库里的文件”。

使用 Claude Code 时，若想保存、共享或部署代码，GitHub 是更稳妥、更规范的选择。可以这样打比方：Git 像随身记录本，GitHub 像远程档案柜。

详细说明可访问：https://docs.github.com/zh

![](img/c5557aa2e0ce29ea4c2e0c61353604a3.png)

**Git 与 GitHub 的关系**

简单说，Git 是工具，GitHub 是网站。

Git 在本地执行版本控制；GitHub 把代码放到云端，供多人协作。Claude Code 既能在本地与 Git 配合，也能和 GitHub 上的远程仓库交互。

二者类似 Word 与百度网盘：一个管编辑，一个管存储；配合起来，才形成现代开发的完整流程。

GitHub 的通俗理解：
https://www.douyin.com/video/7460057392470887699

3.7 Node.js 起什么作用

Node.js 为电脑提供运行 JavaScript 代码的环境。过去 JavaScript 主要活跃在浏览器中，Node.js 把它带到电脑端，使 JavaScript 可以用于服务器、桌面程序、命令行工具等场景。

Claude Code 正是基于 Node.js 构建、并且要在命令行中运行的开发工具。电脑上若缺少 Node.js，Claude Code 就像机器少了动力源，无法启动。

![](img/14976741161f885d3e2fc247dafce5c6.png)

💡Claude Code 的运转，可以视作一次分工明确的演出：终端提供舞台，命令行是你给出的指令；Node.js 提供动力，让 Claude Code 得以上路；Claude Code 登台执行，理解需求、生成并修改代码；VS Code 是后台工作间，用来查看、编辑和测试代码；Git / GitHub 负责留档，把每次改动保存下来，让项目可追溯、可协作；MiniMax2.5/GLM 5 / Claude 模型则贡献思考与编程能力。

整条链路可以概括为：终端发出命令 → Claude Code 借 Node.js 启动 → 调用 AI 模型产出代码 → 在 VS Code 中查看和调整 → 由 Git/GitHub 保存与协作。

### 02.搭好开发环境，安装 Claude Code

0. 安装之前先了解：电脑基础常识

这一部分补充电脑常识，例如如何判断自己的 CPU 型号，以及操作系统的基本概念。

**电脑分类**

电脑大体分为家用电脑和服务器。家用电脑包括常用的笔记本、家中台式机，以及公司配发的笔记本，归个人使用。服务器通常置于机房机柜内，普通人一般接触不到；做过运维、进过机房的人会更熟悉。服务器要求全天候运行，对能耗与稳定性都有很高要求。

**操作系统**

电脑有了硬件后，还要装🛰️、🐧、浏览器等日常应用。硬件与这些应用之间，存在一层软件，通常称为操作系统。

操作系统种类很多：日常最常见的是 Windows，其次是 Mac 苹果系统；服务器上则多采用 Linux。

通常来说，购买的台式机、联想电脑多为 Windows；苹果电脑运行 macOS；若使用虚拟机，例如 Ubuntu，或者服务器上常见的 SUSE，则都属于 Linux 系统。

**Linux 系统**

Linux 是一个较复杂的分支，源头是 UNIX。UNIX 属于商业收费系统，Linus Torvalds 出于开源理念写出了 Linux。日常所说的 Linux，往往指 Linux 内核，可视为基础 SDK 工具。为了承载🛰️、🐧 等上层软件，还需要图形化界面等组件，于是逐渐出现 Ubuntu、CentOS、Red Hat Linux 等分支。

**CPU**

这里要重点关注电脑硬件中的“大脑”——CPU。CPU 是硬件，其发展过程中形成两大指令体系：x86 与 ARM。上层软件要先与操作系统配合，再同底层 CPU 交互。CPU 负责计算与指挥，因此它的指令类型会影响软件安装包的选择。

常见的 Intel 处理器属于 x86 指令体系，这类 CPU 通常对应 x86_64 安装包。如今 macOS 使用的 M 芯片属于 ARM 指令系列，鸿蒙操作系统所用芯片也属于 ARM，因此需要选择 ARM 安装包。

怎么判断自己的 CPU 类型？

💡分清电脑 CPU 是 ARM 芯片还是 X86_64 芯片很关键，因为这关系到安装包选择。此处没看懂也无妨，后面真要选安装包时，再回来确认即可。

**Windows 电脑**

在“我的电脑”上点右键，进入“属性”，即可查看电脑基本信息。

![](img/1a7b144bd1dda1198070a0e96e4e7c32.png)

界面中会显示处理器名称。例如我这里的机器是在 Mac M 芯片上装的虚拟机，因此属于 ARM 类型处理器。

若显示 intel 等字样，则属于 x86_64 机器。

![](img/e3f868ca4bbc1d050ec89f824a80be53.png)

**Mac 电脑**

点左上角苹果图标，找到“关于本机”或“About this Mac”，点击进入。

![](img/89fc7f2db81b35dc14126fe270dba3e7.png)

接着查看“芯片”一栏。若显示 M4 一类型号，就是 ARM 芯片；若出现 intel 字样，则为 X86_64 型号。

![](img/40c65c9438c4af88f5273109da072003.png)

![](img/035568fb2e7d8210c8ff3af33ed300d2.png)

1. 开发环境搭建

使用 Claude Code 之前，要把开发环境准备好，包括开发工具、基础环境 Git，以及 Claude Code 的相关配置。

1.1 Git 环境部署

Git 是代码版本管理体系，会记录你对代码做过的每次修改，相当于一台可回溯的“时间机器”。每段代码都能被追溯、回退或比较；不管是团队项目还是个人项目，都能避免“手滑改崩”或忘记昨天改了什么。

1.1.1 Windows 平台

💡Q：为什么要装 Git？

A：

1. Claude Code 在各系统上都要识别、管理并保存代码项目的版本记录，而这项能力来自 Git。Windows 默认不带 Git，必须手动安装，否则 Claude Code 读不到项目的版本信息。
2. 后续代码存档管理也要依赖 Git，它是开发基础环境中的必备项。装好 Git，Claude Code 才能更安全、完整地理解并管理项目。

PS：安装 Git 时请使用默认路径，不要自行更换安装目录，否则后面容易报错。

**零：视频教程**

视频学习链接：安装 Git 环境-Windows 版本

视频位置如下方截图

![](img/22db047f953e9df5be11d6c07a0f1dd2.png)

**第一步：获取安装包**

打开官网下载地址：https://git-scm.com/

在网页中间找到红色“Install for windows”按钮并点击。

![](img/b6098a87e48db7676be5307b7c2490d7.png)

⚠️注意：安装包虽然不到 64 兆，但官网下载速度偏慢，需要耐心等待。也可以改为网盘获取：

夸克网盘：https://pan.quark.cn/s/7f9f6e363612 提取码：FVCm

百度网盘：https://pan.baidu.com/s/1cRFbfyA-D1wdJX-KMvirdQ?pwd=xg8w#list/path=%2F 提取码：xg8w

随后会进入下载页面，点击“Click here to download”即可开始。

![](img/5497ead46e127cda7a82201573f28666.png)

打开浏览器下载按钮，就能看到下载进度。

![](img/2dc189a4628917710ae010204f585624.png)

**第二步：执行安装**

打开安装包，点继续。

![](img/d88b7d13d72f8a32932c32f5d0684cf7.png)

安装目录选择：

💡这里建议保留默认目录。后面会涉及环境变量识别，还需额外设置；而且 Git 并不会占用 C 盘太多空间。

![](img/d985e1b54428bf3771f4fc1049e61781.png)

保持默认。

![](img/3485dc4612176d927a9d965816dcb3e4.png)

继续。

![](img/37ddd5f6cbffa44b75bb68a5905ba727.png)

保持默认。

![](img/d242bfe3b3568732771d1b8aa8af5d15.png)

随后按安装程序预设连续继续：

![](img/e77d27a2a53d45f590d0e7e5cc7454f9.png)

![](img/ddf0d4a9a0436d856b8a786c432e84c0.png)

![](img/2b7b06314e7366ac1192998b15d7bf1e.png)

![](img/ac3b7ebf80e329f1585409fc5fabcf75.png)

![](img/6e1e20016dd5fbd49729bfd3fec393a4.png)

![](img/b1fe56af8c3d5796c52814bd48f81692.png)

![](img/c8369fbf563eb84e9cea9824ca8ee127.png)

开始安装：

![](img/32f17aaba7de35e29694adc7b53542cb.png)

等待安装结束：

![](img/bec8c3b9b7fda95ff160a70abb51b2b7.png)

完成即可：

![](img/e7958ec678ea1ecad543191cbbb62ab5.png)

![](img/8892c18892c633c0b63503b66e4afb16.png)

之后会弹出如下界面，说明安装成功。

注意：不同电脑型号显示的紫色字样会不同，按自己的机型判断；拿不准可以截图问 AI 是否成功。

下图对应 ARM 处理器，会显示 CLANGARM64～

![](img/331aba6e53cf624d086bf52b330aa9b3.png)

若电脑使用 Intel 或 AMD 处理器，紫色字样会显示 MINGW64～

![](img/70748a7ba45e8de11d9c8eede2a672f5.png)

![](img/21a6123193475997a7a760cd5016d1bb.png)

1.1.2 Mac 平台

这里采用 brew 安装方式，因为 brew 装好后，Git 也会一并就绪，省去额外操作。

💡为什么需要安装 brew / git？

1. Mac 上不少软件都能借助 brew 安装。
2. 安装 brew 时，Git 默认会一起装好，无需再单独处理。

**第零步：视频教程入口**

视频学习链接：安装 Git 环境（Mac 版本）

视频位置如下方截图

![](img/cb08df4aa93c2eb4a21ed7e28586785e.png)

**第一步：启动终端**

从 Launchpad（启动台）或 Spotlight（聚焦搜索）中找到“终端”应用。

通过启动台找到“终端”：

![](img/97482bcb4d07fdf36885f7ed8668d4a3.png)

打开后，默认终端界面如下：黑色竖线所在处，就是输入命令的位置。

![](img/c3fdbcf9b046b4965e730ad19ba78a90.png)

接下来开始安装 brew。若对 brew 不熟，可以询问豆包、GPT，先了解它的用途。

**第二步：安装 Homebrew**

参考链接：https://gitee.com/iamzhihuix/HomebrewCN

将下面整条命令复制到终端并执行。

Shell

```
/bin/zsh -c &quot;$(curl -fsSL https://gitee.com/happyaicoder/HomebrewCN/raw/master/Homebrew.sh)&quot;
```

执行效果如下图所示。

某些环节出现 Password：提示时，输入电脑登录密码即可，注意不要输错。

注意：输入密码时，终端不会显示密码内容，输完直接回车。

![](img/df8c625f0f7454fdfcbaad53af9ba719.png)

选择 1 后，会出现新的提示，仍需继续输入电脑密码。

![](img/62d126513519200f72aad6737ba2d630.png)

输入 Y。

![](img/5c5955dc59fb16d2807d96fc8aa5c4fb.png)

直接回车。

![](img/e8566cbe916daff7200caf4454972df5.png)

输入电脑密码。

![](img/f7715843c77d7f4b989b49abfcaeea3f.png)

选择 2。

**装完了？先验一验再走**

![](img/b8d4dd4818bfaf4cb6c6d587b21bed45.png)

屏幕上出现这一幕，说明刚才那一步已经跑通了。

![](img/e137fe304013c2acf971a0a56375637c.png)

接下来照着命令行给出的指引操作。由于每台机器环境各异，要敲的命令也各不相同——别手打，直接从终端窗口里把那串内容复制出来。终端会告诉你当前该运行哪一条，图示中加了方框的那一段，正是需要你取走的。

![](img/8766f5cda88d2dcabc05f00f4274baed.png)

![](img/9e1ca8e7e81aa03e6158810c99e8af5f.png)

**收个尾：确认 brew 与 git 都装妥了**

先在命令行里跑一遍，验证 brew 已经就位：

```
brew -v
```

![](img/50befa777bff17222e38a4c6f314f799.png)

再核对 git 的情况：

```
git --version
```

![](img/8df30bbef7cdd99ab3f98d38a32e43e1.png)

![](img/958ed644711b0fef0cf0a07ad3c07b42.png)

**1.2 把 Node.js 运行环境搭起来**

💡**问：装它的理由是什么？**
答：像网页、H5 这类最终要落到浏览器里运行的复杂前端项目，其开发依托于 Node.js；比如用 ReactJS、Next.js 做东西时，缺了它根本转不起来。

**版本要求：** 至少要 18，比 18 大的都行，20、22 之类没问题。

**1.2.1 Windows 用户看这里**

动手之前，建议先刷一遍视频：Windows 版 Node.js 环境搭建，入口在下面的图示里。

![](img/87a745734e3498fac046bcaf40aef41e.png)

**① 拿到安装文件**

官网入口：https://nodejs.org/

进站后直接下载，挑安装程序那一项：

![](img/fc68f7f70a01d63a86703ce00e05b808.png)

![](img/a43a0416a265ce52fb2cbc1b2e506c5c.png)

下好之后，文件大致长这样：

![](img/daa3c1e7d692bf5ef8a6777788f85c31.png)

懒得等官网也行，可以直接拿走这里备好的那份。需要提醒一句：你拿到的多半跟我这份不同，毕竟官网版本一直在升级。

![](img/1d4d08197a829073653d1f8b55ab4839.png)

[node-v24.14.0-x64.msi](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/DlPbbuChmonpzKxc5CNcURslnXJ?response-content-disposition=attachment%3B%20filename%3D%22node-v24.14.0-x64.msi%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260526%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260526T134056Z&x-oss-expires=86400&x-oss-signature=2cd4ed55a9c3517d802c294f4c5f221e44690f9a00856f3e8608c8bd1dc8faf1&x-oss-signature-version=OSS4-HMAC-SHA256)

双击它就能启动安装。

**② 走一遍安装流程**

打开这个文件：

![](img/b587591801fe9bae0bcb5a938aa454ca.png)

界面上点「下一步」继续。

把许可协议勾上同意：

![](img/b26fb020cf21b638803da4983faacd0b.png)

安装位置想换就换：

![](img/f19819cce0a604c8cddd564a0461360c.png)

然后直接往下走：

![](img/5fcbae2352cd15f3e6e5909074dae67d.png)

再一次确认：

![](img/2a27e91cb970b484626cd305954ef67a.png)

点「安装」：

![](img/f072cc78ff0fee373362b39a088d8a42.png)

系统若弹出是否允许改动设备的询问，选「是」：

![](img/1985ffc83052f18e46b28bb8f44a3037.png)

耐心等它跑完：

![](img/403c9865e81b957e45c5296367c6d78d.png)

收工：

![](img/e901933c58c49b7a04891f6ffa8bd24c.png)

**③ 试一下能不能用**

唤起 PowerShell 或者命令提示符，把下面这条敲进去：

```
node -v
```

![](img/56a456fc1ee0e853c8041a21a510c033.png)

再跑一条：

```
npm -v
```

![](img/5da95ecb60076685de56b3e1ddb43198.png)

只要返回了正常的版本数字，就说明环境没问题了。截图里记录的时间是 2025-06-13，你看到的数字可能更大、也可能跟我这边对不上，这都无所谓，有数字打出来就算过关。

万一碰上这个错误提示：

![](img/e6a8fd53f61d049872bca1278cb084ed.png)

那就补充执行：

```
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

弹出来问你，敲 Y：

![](img/7b5ebd7059a8371a91ff2ea799956edc.png)

回头再跑一次 `npm -v`，就能正常出结果了。

```
npm -v
```

![](img/2da6a8ac4b13239f49185f4e9d5c2a40.png)

**1.2.2 Mac 用户看这里**

同样先看视频：Mac 版 Node.js 环境搭建，入口在下面的图示里。

![](img/27f772dc06af288bac56607cdbdc45f6.png)

**① 开始装**

教程页面：https://gitee.com/iamzhihuix/nvm-install-cn

把下面这串命令原样拿走，千万别手敲，复制粘贴才靠谱：

```
/bin/bash -c &quot;$(curl -fsSL https://gitee.com/iamzhihuix/nvm-install-cn/raw/main/install.sh)&quot;
```

接着在启动台里搜到「终端」，打开它：

![](img/df9fd2af68a5a740b6db409af9fe6d12.png)

![](img/fdba2bb3d4bdfd4b163dca7234ca3e91.png)

等它下载结束：

![](img/7e7a09c65e676020fb98419f61c7f5ea.png)

出现下面这段提示，说明已经装好了：

![](img/8c032ca030fca4712813c68ffa8820c1.png)

**② 检查结果**

依次跑这几条：

```
node -v
```

```text
npm -v
```

```可以看到版本号就表示安装成功了

你的版本号不一定要和我的保持一模一样

只要是显示版本号了就可以

![](img/f525a0cbadaad09f8daf6f60a1f8ffa1.png)

![](img/430217d3652e45928a34b96aa995cf62.png)

1.3 安装 VS Code 环境

VS Code 是一款轻量、免费的代码编辑器。它的优势是“既简单又强大”：界面清晰，启动快，还能直接调试、预览、运行代码。**Claude Code 生成的代码你都可以在 VS Code 里查看、修改、运行。**

💡Q：为什么需要安装 VS Code

A：就像你写文档的时候在 word 里，那么我们 AI 编程也需要个编辑器环境，我们也叫 IDE，那么 VSCode 是首选

PS：如果你已经具备一定的编程基础，可以自行安装 Cursor 工具，Cursor 编辑器只不过加了 AI 编程功能

1.3.1 Windows 版本

**第零步：视频版教程**

**视频学习链接：**

[安装 VS Code 环境（Windows 版本）](https://shengcaiyoushu01.feishu.cn/docx/Coxxd3mfZoz9CVxEfucc2L4pnJb)

视频位置如下方截图

![](img/bb6e72d335807a6e4e65a021faf522ac.png)

**第一步：下载**

地址：https://code.visualstudio.com/

**点击下载即可**

![](img/a2087c62983e6eb71fb8c5c1ec386114.png)

**第二步：安装**

**我同意**

![](img/60879172a01d203c741219a488df5bc3.png)

**选择安装目录**

![](img/3a3b8260ca780c5349cab4013f426400.png)

**默认**

![](img/09342dc7e737912ed9cf3bc73d0cf897.png)

**全部勾选**

![](img/2c248f624b37832de4ab36a00c4b24d2.png)

**安装即可**

![](img/03563dcfe52d46bb64fd6d0aa51a97f9.png)

**完成就可以**

![](img/35bbd3d460d642ce17f052cf954bcd79.png)

**可以右击直接通过 VSCode 打开项目**

![](img/3136a0e0d6185fd5ed43fe2f7e59e841.png)

![](img/3dc1fcb53eee5859ba2a5aec3d192d7a.png)

1.3.2 Mac 版本

**视频学习链接：**

[安装 VS Code 环境（Mac 版本）](https://shengcaiyoushu01.feishu.cn/wiki/Ixr5wOxeGiuKvik2mQqc4dg2nfg)

视频位置如下方截图

![](img/d23fa0626e97ad7f55951c5382d6fba5.png)

**第一步：下载**

打开网站（https://code.visualstudio.com/download）地址后

选择 Mac 的图标就开始下载了

![](img/41dc0762df8b291b2dc60f1a5610a384.png)

就会跳针到这个页面，打开下载已经开始下载了。

默认下载的是一个 zip 的压缩包

![](img/1a7588e63f3f95e8c644df1f13f9f6d9.png)

**第二步：解压缩**

![](img/64b8f4e7318f720173a4e37bf4d91a6c.png)

**第三步：安装**

安装很简单

直接讲解压缩完后的文件，直接拖拽到左侧栏目的「应用程序」里面就可以。

![](img/2311a6f86d5025adc76858ff349dfffd.png)

打开应用程序，就可以看到 Visual Studio Code 的软件了

就是表示已经安装成功了。

![](img/9f493f3a59ed1a922b86524b59f19111.png)

![](img/bcd98553db26d89cb833e7f2806575ae.png)

2.**安装 Claude code**

这里只是给大家演示不同电脑版本如何安装 Claude code，**并没有启动 Claude code 部分**，等到下一部分，会和大家说如何配置 MiniMax2.7，然后 在 VS code 中使用 Claude code

2.1 Windows 版本安装

**视频版教程**

**视频学习链接：**

[安装 Claude code（Windows 版本）](https://shengcaiyoushu01.feishu.cn/docx/AVAldXzUmoVc8nxNX0dc2LVinWf)

视频位置如下方截图

![](img/e171a7be3586aca95511c833b9e82585.png)

**图文教程：**

我们在开始中搜索**「powershell」**
```

```
powershell
```

启动时记得提权（管理员模式）：

![](img/807b00b02db66fdaed2de8de5dfff260.png)

然后敲：

```
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned
```

![](img/62ad2745ca5cfcd087c41ad0b372aa9b.png)

提醒：部分机器会跳出策略限制相关的询问，得按后面的步骤处理掉，否则接下来会卡住走不动。

处理方式：敲 Y 再回车，如果界面回到可以继续输入的状态，那就成了。

![](img/ff956ea81722b9a3462dc1350104cfb6.png)

核对：把下一条命令复制出来，粘进 PowerShell 里回车。

```
Get-ExecutionPolicy -List
```

只要 `CurrentUser` 那一栏写着 `RemoteSigned` 就过关，其余项是什么值不必在意。

![](img/33f68e59dcd0939825535d234bcd2484.png)

接着跑安装指令：

```
npm install -g @anthropic-ai/claude-code  --registry=https://registry.npmmirror.com
```

![](img/defdd96ee1a319f88252d4222acd4176.png)

屏幕上冒出几行 `notic` 开头的提示，那只是警告，不代表 Claude Code 装坏了：

![](img/42172b1230c4f89d1794b53d6c8e17f3.png)

核对：

```
claude -v
```

能看见版本数字打印出来，就大功告成。

![](img/d89d697d96d8fbc970564fdd9cd7100b.png)

![](img/d48aca86f64b333f536480220181b9bc.png)

**2.2 Mac 上的 Claude Code 安装**

视频入口：Mac 版 Claude Code 安装，位置在下面的图示里。

![](img/f07aac0646ed55be356ce63fb13979e9.png)

**① 装起来**

把这条命令复制好，直接往终端里贴：

```
npm install -g @anthropic-ai/claude-code  --registry=https://registry.npmmirror.com
```

你终端里刷出来的内容未必和我一模一样，只要不是红色字就没事。通常还会带出别的信息，看不懂就截个图丢给 AI，让它帮你翻译。

![](img/4e987cf2c4d654d65bb5f8e7c0e07772.png)

**② 看是否装好了**

```
claude -v
```

苹果机器上的画面如下：

![](img/521365db7674089ddef072a681f0fbec.png)

![](img/54d6ad3e853c3872d430a9899ee019e0.png)

**2.3 装的时候容易碰上的几个坎**

**坎一：终端出错了，怎么把错的内容抠出来？**
用鼠标选中那几行，点右键即可拷贝。

**坎二：跑 `npm -v` 或者 `claude` 时报错**
Windows 上要是撞见下面这个错误，先跑一条：

![](img/c68af2242527f958f6109c84f0eb27c7.png)

再补一条：

```text
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

```
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

![](img/f2cbbed271b8c647e21a4a9f6689f01d.png)

**坎三：出错信息里带 git 字样**

![](img/953801c9216933b05ba9747aa9c8045c.png)

两种解法：
1. 把 git 卸掉重装，路径保持默认；
2. 给 `CLAUDE_CODE_GIT_BASH_PATH` 赋上值，值填 git 的实际位置（在 Windows 的环境变量窗口里设置）。

**坎四：Mac 上冒出红色错误**

```
sudo npm install -g @anthropic-ai/claude-code
```

💡**⚠️ 提醒：** 安装过程中若弹出下图这个错误，说明当前操作得靠管理员权限。在前面补一个 `sudo` 重跑就好。把这条命令粘进终端：

```text
sudo npm install -g @anthropic-ai/claude-code
```

之后终端会索要开机密码。这里要注意，密码输入时屏幕上不会有任何回显，照常打进去按回车即可。比方说密码是 1234，就在钥匙🔑图标后面敲 1234 再回车。图示如下：

**⚠️Claude Code 连不上网？先看这里**

![](img/1b4c94be5f6cf360336e0a2b4492445c.png)

![](img/673091eefc6e2f8273f617cd1a90ebd5.png)

本地若未开启全局代理，大概率会看到 **Unable to connect to Anthropic services，please check your internet connection and network setting** 一类的报错。要是后续打算用智谱、MiniMax 等国产模型来跑 cc，这条提示暂时可以无视；但如果你用的是官网原版 Claude Code，那就按下面的方法来处理。

**报错修复思路**

![](img/158e76a61dbe0b984e4a3760138d6c0a.png)

核心操作只有一个：动 Claude Code 的配置文件。

Mac 端位置：`/Users/[电脑用户名]/.claude/settings.json`  
Windows 端位置：`C:\Users\[电脑用户名]\.claude\settings.json`

举个例子，Mac 用户名若为 limo，对应文件即 `/Users/limo/.claude/settings.json`；文件不存在的话，同名新建一个就行。

![](img/e5d36a3d56a9b80d50ff451357978e5a.png)

双击打开 `settings.json`，按 JSON 格式把代理参数补写进去：

```
{&quot;env&quot;: {
    &quot;HTTP_PROXY&quot;: &quot;http://127.0.0.1:7890&quot;,
    &quot;HTTPS_PROXY&quot;: &quot;http://127.0.0.1:7890&quot;
}}
```

![](img/d2d11ac419b940cc308cb24a75331eb0.png)

请务必核对端口：代理软件 HTTP 端口写的是 7890，这里就填 7890；写的是 7897，就改成 7897。

**3. 另一条路：MiniMax2.7 驱动 Claude Code**

Claude Code 的用法分两类——官方版，以及用 MiniMax2.7 等国产模型来驱动。官方版得先去 Claude.ai 订阅，套餐分 Pro、5x MAX、20x MAX，标价依次为 20 刀、100 刀、200 刀。再加上 Claude 对国内长期封锁，走官方路线要同时搞定网络与海外信用卡支付两道难关，门槛确实偏高。

本次实操，我们更建议大家走国产模型 **MiniMax2.7** 驱动 Claude Code 这条路。

💡先花一分钟科普几个高频词：

1. **cc-switch**：一款能在 Claude Code 里快速切换不同模型 API 配置的辅助工具。  
2. **MiniMax2.7**：MiniMax 公司训练的大模型。  
3. **Claude Code**：一个编程工具。平时大家聊的“官方使用”“封号”“需要网络环境”，背后其实对应 Claude 模型——Anthropic 这家公司既产出 Claude 模型，也提供 Claude Code 编程工具。

后面动手时，它们之间的关系会更直观。

**3.1 视频版教程**

cc-switch 在 Mac 上涉及安全设置，因此以 Mac 为演示环境；Windows 端操作逻辑与之完全一致。

视频学习链接：[安装 cc-switch](https://shengcaiyoushu01.feishu.cn/docx/Qr2NdoezHo87gIxcMy9c1vs6nIf)

视频位置如下方截图。

![](img/e3b72ed90198ff52e006f0c1d8a58d64.png)

**3.2 配置 MiniMax2.7（cc-switch 篇）**

**3.2.0 学习资料先备好**

套餐购买入口：

https://platform.minimaxi.com/subscribe/coding-plan?code=G4YsAHUVMT&source=link

通过该链接下单可享 9 折优惠。

这个入口用于 MiniMax2.7 注册账号与充值。该模型由 MiniMax 公司运营，属于付费服务。进去后先完成注册，再购入 Token 额度或会员套餐，才具备调用资格。

![](img/bfe77697c28bacc0446066e6921e741e.png)

API-KEY 设置入口：

https://platform.minimaxi.com/user-center/basic-information/interface-key

这里是获取 MiniMax Token Plan Key 的页面。账号有余额并不等于能直接拿账号密码登录软件（cc-switch）——你需要在此页生成一串 API Key，也就是那串较长的字符密钥。它相当于给软件开的“专用通行证”，填入配置后软件才能代表你调用 AI 模型。

💡重点是选“Token Plan Key”，而不是上方那个普通 API Key，切勿搞混。

![](img/13ac5c7178ea47fd70d0c42bb35f403b.png)

MiniMax2.7 官方配置文档：

https://platform.minimaxi.com/docs/coding-plan/claude-code

可以把它当成官方说明书，里面会逐一交代 cc-switch 中各参数的填法，例如 API 地址写什么、模型名称怎么写。建议先打开自行过一遍。

![](img/577820c66751610efac0ed43f5dff4ca.png)

**3.2.1 选购套餐**

MiniMax2.7 由 MiniMax（国内 AI 模型企业）提供，是一款商用大语言模型。模型跑起来要靠 GPU、显存这类算力资源，算力服务本身收费，所以用户得先买套餐、拿到调用额度。

（1）点开链接进入大模型官网：

https://platform.minimaxi.com/subscribe/coding-plan?code=G4YsAHUVMT&source=link

首次访问需登录，手机号注册即可。登录后会看到对应页面，点击特惠套餐就能跳到付费套餐选择页。已经注册过大模型官网的，直接点上方链接也会出现类似的套餐界面。

![](img/e29d57fde047c0b3c2c08ee6243ddc13.png)

（2）按需求挑套餐：

- 新手观望、只想体验 Claude Code 功能：先选 29/月试水，推荐 49 套餐。  
- 确定后续高频使用、或要上线产品功能：选 119/月。  
- 在意生成速度（3 倍速）：选对应额度的极速版。

💡提醒：默认会按月自动续订。下个月不打算继续用的话，记得去支付宝取消订阅；取消后本月仍可正常使用。

**3.2.2 提取 API KEY**

API Key 相当于一份独属的“身份凭证”，也是工具替你登录系统的“钥匙”——系统凭它辨认你是谁、买了哪档套餐、还剩多少额度。每次调用 MiniMax 模型（写代码、答问题等），你的电脑或工具（如 cc-switch）都会附带这个 Key 发给服务器。

打开上面给出的 MiniMax 地址，界面如下。

![](img/7a525b7f14a9edf4705bb09d09e6183e.png)

复制 API key。我这边已配置过，所以能看到一个「复制」按钮。

💡请务必妥善保存 Key，防止泄露带来不必要的安全隐患。

![](img/ce0ea80e3e71ace7f53ef1adb68dfb58.png)

**3.2.3 用 cc-switch 填入 API Key**

AI 模型本身不带聊天窗口，得借助 cc-switch 这类软件填入 API Key 才能对话。这款工具的优势在于界面直观，能在 ChatGPT、MiniMax2.7 等多个模型间一键切换。本次我们就用 cc-switch 配 api-key 并选用 MiniMax2.7 模型，对新手比较友好。

注意：若你已有官方 Claude 账号，就绕开 CC-Switch，直接进 Claude Code 终端，在对话框里执行 `/login` 登录。

第一步：下载 cc-switch。

这里选用的是一款轻量模型切换工具 cc-switch，GitHub 开源项目，能帮我们更便捷地切换不同模型来驱动 Claude Code。原地址：

https://github.com/farion1231/cc-switch

下面是 Windows 版与 Mac 版，开箱即用。

Windows 版下载：

![](img/6fd875464dc7f048121278d2bc55d619.png)

[CC-Switch-v3.12.3-Windows.msi](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/UxmTbcWTQoR19FxZMCkcw0HJndh?response-content-disposition=attachment%3B%20filename%3D%22CC-Switch-v3.12.3-Windows.msi%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260526%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260526T134056Z&x-oss-expires=86400&x-oss-signature=8cd2adefaa862a13e11240b77379c6f25908630517e99f2c6df940580afab7f9&x-oss-signature-version=OSS4-HMAC-SHA256)

Mac 版下载：

![](img/81eada940d20530688f7ebd8c0d30e16.png)

[CC-Switch-v3.12.3-macOS.dmg](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/LxWqb0wRJotGMLxJ0hhcULDGnwc?response-content-disposition=attachment%3B%20filename%3D%22CC-Switch-v3.12.3-macOS.dmg%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260526%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260526T134056Z&x-oss-expires=86400&x-oss-signature=a1c74d9cce5f9b55c99749f9253a762226e5c3631de70df625f56d5f5a55203b&x-oss-signature-version=OSS4-HMAC-SHA256)

或者从这里直达：

https://github.com/farion1231/cc-switch/releases

网速不给力的话，优先用上方提供的直链安装包；访问超时的话，可转到国内 gitee 镜像仓库：

https://gitee.com/iamzhihuix/cc-switch-mirror

Windows 端安装若碰到类似报错，换成下面的免安装版即可：

![](img/0486a89fe7cd81c7a5f3422a0446e2c8.png)

免安装包在此：

![](img/b732ce0c8999a9ccd03b2832004bc6e6.png)

[CC-Switch-v3.12.3-Windows-Portable.zip](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/XvYKbUJIco4LBVx04PecsX8Lnxb?response-content-disposition=attachment%3B%20filename%3D%22CC-Switch-v3.12.3-Windows-Portable.zip%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260526%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260526T134056Z&x-oss-expires=86400&x-oss-signature=66864f124e6eb666df9bfefe3be2c4754cc95fc6c4ed0aa303800e37c3b4edd5&x-oss-signature-version=OSS4-HMAC-SHA256)

1. 解压到某个目录，别把这个目录删掉。  
2. 建议右键以管理员身份启动。  
3. 可右键发送到桌面，建个快捷方式。

💡⚠️提示：CCswitch 迭代较勤。若从 GitHub 拉下来的版本跟本文档中的对不上，可以直接下最新版，整体安装步骤大同小异；也可以直接用本文档提供的安装包。

上述链接点击后，Windows 电脑会展示对应页面——点进第一个 3.12.3 标题，把页面拖到底部找到 Assets，那里就是下载安装包的位置，挑一个下方包下载即可。

⚠️提示：加载速度偏慢属于正常现象。

![](img/7a36835b1093ad6130d678ec21b724e8.png)

页面继续下滑会看到 Assets，那里就有安装包下载入口。

![](img/5e38d28e9be3a456d0f1f5bd266705fc.png)

若找不到想要的包，试试点页面上的「Show all 17 assets」链接，所有包都会列出来。

![](img/3288646ee21b4675e6ca7c9cd0c9fc24.png)

Windows 安装包如下：

![](img/31ad22052e804dd8ba2042dfcf4b6c55.png)

Mac 安装包如下，下载下来是压缩包。安装方式：双击解压，再拖进「应用程序」目录即可。

![](img/71568c4f319f74af45213702dcca6682.png)

⚠️提示：Mac 若打不开，出现「移到废纸篓」或者「文件已损坏」等提示，请参照 3.3 常见问题处理。

第二步：安装 cc-switch。

Windows 安装流程：出现此类弹窗时，点「运行」。

![](img/7cdcc74008c5917f6dfc9c7b118a3b35.png)

随后进入如下界面。

![](img/9592203b1db3cbe29518a4978e113c43.png)

选定安装路径。

![](img/816fa2b3d4a00bdcf98a20aac7089de6.png)

点击安装，等它走完即可。

![](img/d02e232d804ff462ddfdc98531022397.png)

![](img/c44d1d896846e1200d763dd1fd65d01b.png)

![](img/dc7f40755d0973ad35ce640548a145c7.png)

**3.2.4 配置 MiniMax2.7**

接上 MiniMax2.7 接口，就等于让工具与模型正式对话——指令能送达模型，回应也能拿回来。

装好 cc-switch 后打开，界面如图。首次安装进入就是这一页，点右上角【添加供应商】。

![](img/61f4c506e769bc2686bb4b0eaa036337.png)

把此前在 MiniMax 页复制的 Coding Plan Key 粘贴到下面输入框。若忘了位置，可以回看截图，或重新打开：

https://platform.minimaxi.com/user-center/basic-information/interface-key

![](img/9ad89bdfd7edadd3655f7db18070fb01.png)

最后点一下添加。

![](img/3d2996f03da55d4bc3577ba3797bb1d8.png)

如下图，鼠标悬停到已配好的 MiniMax 模型上，若显示“使用中”，就代表配置成功。

![](img/49217f4171766f65e5e33ffa06b7189c.png)

若出现如下界面，别忘了最后点一下「启用」。

![](img/0c944d4dae65681ecef6f97c8f4c920e.png)

**3.3 cc-switch 安装常见问题**

Q1：VSCode 插件怎样使用自定义 API key？  
A：进入 CC-switch 的设置页即可。

![](img/06d832fa6d4c7bfd87cb90a0ec72c23b.png)
勾选完成，按下保存，这一步就收尾了。

![](img/65c040fc6f359645e9aefbbaace881c6.png)
若按上面的方法设置后依旧没效果，再继续看后面的调整。

![](img/9fa4c4246ca25671414072c35608e59a.png)

![](img/ff328deaa15e4dc27fadd9df32e0e385.png)

**Q2：套餐额度不够用怎么办？**
A：直接续费或充值套餐就好。

![](img/9c288f80c202cedec415c4cc0538120f.png)

**Q3：Mac 上装 cc-switch 的安全拦截如何处理？**
3.12.4 版已经修复了这个现象。
在苹果电脑启动 cc-switch 时，系统仍可能弹出下面这样的提醒：

![](img/41da9498a4beb1563a2230ada5bf99b0.png)

别紧张，进入系统设置，定位到隐私安全相关面板，滑到页面底部，点选允许继续打开的那一项。

![](img/0216dae1a418724d730b52dc0ce69e3a.png)

第二次弹出同样窗口时，记得仍然选允许打开，别点偏；随后会跳出密码输入框。

![](img/1e413958933719b4131f0b62688fdce4.png)

![](img/8065b99c502d0871573349893b558ac4.png)

完成后就能顺利进入了。

![](img/96aef687bb68bdae8d67793fe8977d38.png)

环境配置到此结束。下面我们认识一下 Claude Code 的界面。

**Q4：从终端启动，或连接官方接口时遇到网络报错**
建议优先看配套视频。需要改的文件和参数其实一致，只是操作系统不同，路径会略有差别。

**Mac 版视频：**

![](img/bd88f6eee3884d7876140367a6fc1198.png)

claudecode-network-mac-12月19日.mp4【在线播放】

![](img/8c179ad8041b4f53ecebd6e0cdc2d59e.png)

**Windows 版视频：**

![](img/dc1cd91cdd64b2991b7ad29f933b992f.png)

claudecode-network-windows-12月19日.mp4【在线播放】

![](img/1f585f0ebf331f3c8a7879692893d318.png)

如果 CC Switch 已经配好，却还看到下图这类错误，

![](img/91841b12358cb5ae64944d381f2f6802.png)

先检查 settings.json 里有没有写入 KEY、URL。Windows 下路径为 C:\Users\用户名.claude，记得让系统显示隐藏项目。确认该文件存在后，用记事本打开编辑。

![](img/196f8f738763408583b3c83a7b00a121.png)

至少要能看到 ANTHROPIC_AUTH_TOKEN 与 ANTHROPIC_BASE_URL 这两项；缺少的话，回 cc-switch 再配一次。

![](img/d8661ede7346d4afa09d638043b08521.png)

两项都齐全，却依旧进不去 Claude 终端，那就要改 .claude.json。它位于用户目录中，见下图。

![](img/e2788365287c160d57fa0bc3276e0c15.png)

同样用记事本打开，搜索 hasCompletedOnboarding 这个字段。其余内容不用管，有差异也无妨。

![](img/02e0c8fbf5ae0d00b31a0b0d2066b4d3.png)

若找不到该字段，就把它补进这个 JSON 文件，注意字段后面的半角逗号。全程使用英文符号，别混入中文标点。整个文件必须保持合法 JSON 结构；一旦语法出错，配置就不会生效。改完可以到 json.cn 这类站点格式化并校验格式。

Plain Text

```
{// ... 其他配置
  &quot;hasCompletedOnboarding&quot;: true,
}
```

### 03.Claude Code 使用界面与常见操作

1. 怎样把 Claude Code 跑起来

初次上手推荐第一种，功能更齐全；第二种可以按需了解。

**配套视频**

**视频入口：**
Claude Code 启动演示
视频在下方截图中的位置。

![](img/a44b30836ae9b1042b1a333b7c50cb2a.png)

**1.1 第一种：在 VS Code 的终端里运行 Claude Code**

1.1.1 启动 VS Code，点界面左上方的文件夹按钮，然后选取打开文件。

![](img/6db2b27589ddf1a31e7b512cdb317567.png)

1.1.2 建一个新文件夹，载入项目，并在提示中选择信任。

![](img/45031a33ec65519245c098b4c6f7cdd4.png)

![](img/e89e8cd50d9ab7f4ecdd783e402db1de.png)

1.1.3 调出终端。在 VS Code 里点右上角那个相近的按钮。

![](img/b972f0715cc3ba3f6fea93800cb32548.png)

即中间位置那枚。

![](img/e03efacfa9c39f1359b606b5d319ba2c.png)

点下去后，下方会出现一块绿色区域，那便是默认开启的终端。

![](img/9d8a1c68c952f4ab7930af40c2b22b9d.png)

此时终端已能运行 Claude Code，敲入 claude 即可。

```
Plain Text

```text
claude

```

![](img/a367a49b4aabf1b0d7e7d6a7cf97950f.png)

下面就可以愉快的和 Claude Code 沟通交流了

![](img/22752b58281f7dec97a7f53579ceca9c.png)

**1.2方式**二**： VSCode 使用 Claude Code 插件形式**

💡官方对这个插件在 2.0 版本后进行了大升级

native 方式的插件支持

体验更友好

前提操作：

! ! ! 在 CC-switch 设置里面，一定要打开下面的配置！！！

![](img/2563ab0da6af4ff81b616a18459d3a72.png)

1.2.1 打开**VSCode**，点击左上角文件夹图标，选择打开文件

![](img/9f7c0f8d1c411d3f1a71d87b5a053fe7.png)

1.2.2 新建文件夹，打开项目，选择信任项目

![](img/fbc00cf0541d6cbf0e22931ef113946f.png)

![](img/5ece9ac12f41538d5edd356a1366ca76.png)

1.2.3 安装插件

如下图：

1、需要打开 VSCode 的插件市场

2、搜索 Claude Code

3、认准是 Anthropic 公司的插件

4、 点击安装就可以

![](img/58f2ad0a8773e096e8a866ecc873acd6.png)

会有弹框提示，选择相信就可以

![](img/cc9910aef0fe37f38785359fdd26dd8c.png)

可以看到在编辑器的右上部分，可以看到一个 Claude Code 的图标

就表示已经安装成功了。点击那个图标就可以使用了

![](img/c95b57badcaee9268d3b032d279ec6cc.png)

下面是使用的几个截图

![](img/59cef3aa6beca8d5422810a7473f2f6a.png)

![](img/6bfff8b066066d98d563a74c10601c8a.png)

如果大家打开的是下面的画面：请一定要看下面的注意事项

![](img/b4a58b3f1b12119dbeb71364fdf1f404.png)

💡

**注意事项 1**

右侧有个 vscode 的自己的 chat 框，那不是我们要用的，也不要在这里发消息，关闭掉

💡

**注意事项 2**

如果 Claude Code 对话框出现订阅画面

那是 cc-switch 的配置没有成功

回到 cc-switch 的设置里打开“应用到 Claude Code 插件”

如下图所示，然后重新打开 VSCode，重新打开 Claude Code 对话框

![](img/81bef8ce03a18a5a5305f42086b12912.png)

![](img/79837659b67652958d6212090bcbcf26.png)

![](img/ab2d15488c38d7b0ad7937023c6cde38.png)

2.使用 Claude code 基础操作

这里给大家介绍关于使用 Claude code 的一些常用操作，如果之前从来没有使用过 Claude code，这个板块可以仅做了解学习，看看即可，不需要马上掌握就可以用，具体等到第二章的案例，就会在实操中使用这些操作的

2.1 基础入门操作

| 操作名称 | 功能是什么 | 什么时候用 | 如何操作 |
| --- | --- | --- | --- |
| 自动编辑模式 | 让 Claude 自动修改代码，不用每次确认 | 写代码、修 bug、调逻辑时 | Mac： Shift + Tab 一次 Windows： Alt + M 切换模式 |
| @ 指定文件 | 告诉 Claude 只处理某个文件 | 修改单个文件或定位错误 | 在对话里输入 @文件名 即可 |
| 粘贴图片 | 让 Claude 看图帮你调界面或排查错误 | 前端调界面、查页面错误 | Mac： Ctrl + V （ 不是 Cmd + V） Windows: Alt + V |
| 常用命令 | 管理 Claude 的状态和上下文 | 清空对话、切换模型、诊断问题 | /clear 清空上下文，重新开始； /compact 清理但保留记忆； /status 查看当前 Claude 状态； /doctor 检测安装问题； /model 切换不同模型 |

2.2 日常高频操作

| 操作名称 | 功能是什么 | 什么时候用 | 如何操作 |
| --- | --- | --- | --- |
| Plan 模式 | Claude 先帮你想清楚方案，再写代码 | 项目刚开始、做方案设计或复杂功能时 | Shift + Tab 连按两次（Windows：优先使用 Shift + Tab ，不好使就用 Alt + M 按两次） |
| 记忆文件（ CLAUDE.md ） | 让 Claude 记住你的使用习惯和项目环境 | 希望长期保持同一风格或配置时 | 全局：～/。claude/ CLAUDE.md ; 项目：项目目录下创建 CLAUDE.md |
| 打开思考模式 | 普通思考模式 或者会使用思考模型 | 基本常开 | tab 打开，右下角会提示 |
| 深度思考（ultrathink） | 让 Claude 进入“高强度思考模式” | 遇到复杂问题、性能优化或大规划时 | 提示词中加入 “ultrathink” 或 “深度思考” |

2.3 进阶操作 YOLO 模式

**P**S：YOLO 模式属于进阶内容，如果是第一次操作使用Claude code，对此仅仅做了解即可，可以进入到下一步的实操学习中

视频学习资料：

[YOLO 模式视频学习链接](https://shengcaiyoushu01.feishu.cn/wiki/EUxewYXXGiPViyk3iPwcx43Inyf)

视频位置如下方截图

![](img/3ea45d535f747eb871423a14540c61a3.png)

我们在使用 cc 的过程中经常会出现要求我们手动确认文件修改的场景，这种频繁的人工干预会打断我们的思路。

这种情况下我们就可以使用 yolo 模式（狂飙模式）了，它可以解放我们的双手，让 cc 进行入到自动工作模式。

YOLO 模式通过一行启动命令开启：

claude --dangerously-skip-permissions

Plain Text

```
claude --dangerously-skip-permissions

```

如果我们发现 cc 左下角提示了一个“bypass permissions on"，代表我们的 YOLO 模式已经启动成功了

![](img/44b38f368502b2013a2be1511ad985f6.png)

yolo 模式非常适合我们从 0-1 新建项目，这种模式下我们不需要频繁地去接受变动，让我们写代码像德芙一样丝滑。

那我们发现每次输入这么长的一堆很麻烦，那我们能不能默认使用 claude 就是 yolo 模式呢？解决方案很简单，就是配置终端别名。

当然了无需自己实现，我们只需向 cc 发出这样的指令：

Plain Text

```
麻烦给终端加个别名：以后敲 claude，就自动带上 --dangerously-skip-permissions 参数执行。

```

这样我们发现执行 claude 进入中断后左下角也有 YOLO 模式的提醒了

相信到这里，你已经安装上 Claude code，并且可以在 VS code 中运行啦，现在也对 Claude code 的基本内容有了简单了解，让我们在下一章开启实操学习吧

```

### 04.实战：拿 Claude Code 做一个早读小工具

1. 配套视频

📕上有一批卖得挺火的 AI 虚拟商品，下面这个早读工具就是典型例子。它靠产品解决用户需求，同时带一点技术门槛，能帮你在虚拟商品领域建立壁垒。一旦你能独立做出这种产品，收获的不只是技能，更是一件能在📕直接卖货的商品。

说明：本节案例重在帮你快速上手，借助 Claude Code 做出产品，并对它有初步认识；更多编程案例见 2025 年 12 月的 Claude Code 航海（https://scys.com/course/detail/98）。

**视频入口**：[用 Claude Code 做一个早读工具](https://shengcaiyoushu01.feishu.cn/wiki/SEtTwjUuBiIcGkktTcFchFAEnvf)

视频在下方截图中的位置：

建议先过一遍视频，再对照图文动手。

![](img/60f01e426a882e1b64c3caef00b45ee2.png)

2. 产品需求怎么找

逛一逛📕就能发现，教育类小工具可做的方向不少。

![](img/650025e139b6d34bfa9a406089f5bf37.png)

本次挑中的案例叫「早读动物园」。玩法很简单：先设一个分贝阈值，学生朗读声超过它，屏幕便蹦出许多动物形象；声音持续达标，动物数量还会不断增加。

在📕搜索「早读动物园」，能刷到不少同类型早读工具。

不妨先跟着案例把这款产品复刻出来，再去开发你感兴趣的其他早读工具。

![](img/8c3c336f18f56c01b8f638040a51a685.png)

3. 动手实操流程

**3.1 先截屏，再由 AI 代写指令文案**

到📕找到目标产品的展示图，截屏保存。

![](img/f56a05d0bb3f7f1be6bd4a7186468ac6.png)

没找到的读者，直接拿下面两张截图也行。

![](img/ec757a528b26e7016643ac5fe1d48521.png)

![](img/b5f9b24aebc5e41b5f34acac2fc85fda.png)

**3.2 把截图发给 AI 并说明需求**

把指令文案和截图一起丢进 AI 对话窗口，把想要的效果讲明白。手头没有 GPT 或 Claude 客户端（它们需要特定网络环境）的话，可以用国内豆包替代。也可以直接复制下一步备好的指令，粘贴给 Claude Code 或其他 AI 对话框。

Markdown

```text
这张图里面是什么内容，我想使用 html 复刻的话怎么弄了？先不写代码，我去 claude code 里面实现，请给我具体的提示词就行.
```

![](img/a7df0a45d4e76c4e90f91686d055ff7a.png)

![](img/1865644bbfd1b256c1a87d70886fa54d.png)

3.3 交给 Claude Code 来开发

3.3.1 在 VS Code 里载入新目录

从菜单栏进入目录：
1. 运行 VS Code；
2. 在顶部菜单点「文件」（File）；
3. 选「打开文件夹...」（Open Folder...）；
4. 弹窗出现后，找到目标目录并选中，按「打开」。

![](img/b0d4771a33f8bdf19b1fc1e1dae5e215.png)

3.3.2 在 VS Code 里跑起 Claude Code

在 VS Code 终端敲入 claude 并回车，程序就会跑起来。

Markdown

```
claude --dangerously-skip-permissions
```

![](img/ec611effff19524ce4b11df3aa6efe9a.png)

3.3.3 让 Claude Code 开始写代码

# 早读神器实战记：Claude Code 与 Skills 一起拿下

打开 VS Code，创建一个名为 `prd.md` 的空白文件。先把之前向 AI 要来的那段 prompt 粘贴进去，然后切回 Claude Code 的对话框，输入 `@prd.md` 引用这个文件，功能就能直接跑通。

这里提醒一下：文件记得保存。

- Windows 快捷键：`Ctrl + S`
- Mac 快捷键：`Cmd + S`

放进 `prd.md` 的完整 prompt 如下：

Markdown

```
请用 HTML + CSS + JavaScript 创建一个&quot;早读动物园&quot;应用，具体需求：

1. **主界面布局**：
   - 顶部：标题&quot;早读动物园&quot;和副标题
   - 中间：大的天蓝色动物展示区（带浅绿色地面），动物图标随机散落分布
   - 底部三栏：左边显示当前分贝和阈值调节，中间显示计时，右边是设置和暂停按钮

2. **核心功能**：
   - 使用 Web Audio API 获取麦克风音量分贝值
   - 当音量超过设定阈值时，每隔一定时间生成一个随机动物emoji
   - 动物以随机位置、随机大小出现在展示区，带淡入动画
   - 计时器记录累计朗读时间

3. **设置面板**（点击设置按钮弹出）：
   - 动物生成速度滑块（1-60秒）
   - 动物种类选择（多选，用emoji表示）：🐶🐱🐰🐻🐨🦊🦁🐐🐷🐸🐔🐧🦆等
   - 全选/全不选按钮
   - 保存和重置按钮

4. **视觉效果**：
   - 使用渐变色背景
   - 动物emoji大小在30-60px间随机
   - 卡片式设计，圆角阴影
   - 按钮用蓝色和红色区分功能

5. **技术要点**：
   - 请求麦克风权限
   - 实时计算音量分贝
   - 动态生成和移除DOM元素
   - localStorage保存用户设置
```

这份就是交给 Claude Code 的开发指令，让它照着实现。

搭建细节建议跟着视频走一遍，会更直观。

Markdown

```
@prd.md 实现这个功能
```

![](img/030405969c5713d5ca3fc869ed047615.png)

![](img/4eb426c89d05e74da4541e3cf8cf8506.png)

### 3.3.4 成品展示

开发收尾后，回到项目根目录，右键选择「Reveal in File Explorer」，找到 `index.html`，用 Chrome 浏览器打开它。

![](img/0ef84ace7bc864893475e628d3ae8f3c.png)

首次进入页面会弹出麦克风授权请求，点允许继续。

![](img/ee44d66feba313d81ff56551c48bc29e.png)

声音测试开始前，先把阈值调到合适位置。然后随便说几句话试试，屏幕上会蹦出卡通小动物。只要声音不停，小动物就会持续冒出来、越积越多。

![](img/40a811e75a0c59eeddef140531c49b9a.png)

**这个小工具的主要用途：**

1. 支持自由调整触发发声的分贝线。
2. 当声音超过分贝线且持续不断时，页面里的小动物数量会一直累加。
3. 做它的初衷很简单，就是让早读课不那么无聊，鼓励学生放开嗓子大声念课文。

### 4. 总结

这次做的是一个早读好帮手，动手部分的重点：

1. 从📕这类内容平台里发现真实需求
2. 用 Claude Code 落地一个基础网页案例，技术组合是 HTML、CSS 与 JavaScript
3. 练熟 Claude Code 的提示词对话方式，别看到终端工具就打怵

💡本期航海内容排得比较密，Claude Code 这边只演示了一个项目。想多看实际案例的话，可以去翻上一期航海，那边的内容更丰富，选择也更多。

---

## 二、Claude Skills 的入门和实战

### 01. 入门：快速认识 Claude Skills

#### 0. 本章导读

从这一章开始，正式进入 Claude Skills 的入门和实战。目标不只是让你知道 Skills 大概是什么，而是真正上手：会装、会挑、懂得避开风险，还能亲手做出第一款能落地的 Skill。

先记住一个底层认知：所谓 Skills，就是写给 Claude 的操作手册。它的价值不在于让 AI 变聪明，而在于让 Claude 在做特定事情时，输出更稳定、表现更专业、结果更贴近你的验收标准。

后面会讲具体的安装和管理方法，包括怎么从 GitHub 快速拉取现成 Skill 到 Claude Code 项目里、安装时有哪些原则要注意。

在此基础上，本章安排了两条实战路线。

其中一个方向是自媒体自动发布 Skills，具体拆成👸号和📕两种场景，二选一完成就行。新手更推荐从👸号全自动搭建入手，📕那条线难度会高一些。

另一个方向是 AI 视频制作 Skills，进阶篇同样是双选项，挑一个完成即可。新手建议从小说改编漫剧剧本的 Skill 开始，另一个选项门槛略高。

当这章学完，你得到的不仅是几个能用的 Skill，更是一种全新工作方式：把经验、流程、判断标准，沉淀成 Claude 能反复调用的自动化能力。

💡

**本章航线图**

完成本章的学习和动手操作，航线图第一阶段就收尾了。

- 第二阶段：Claude Skills 的入门和实战（约 7 天）
- 安装部署 Claude Skills（约 1 天）
- 完成一个基础实战案例（约 3 天）
- 完成一个进阶实战案例（约 3 天）

#### 1. 认识 Skills

💡⚠️先提个醒：第二章的内容都要在 Claude Code 环境里跑。如果还没装好 Claude Code，请先回到第一章完成部署，再回来看 skills。

Skills 是 Claude Code 在 2.0.20 版本里引入的一项能力。准确讲，这是 Claude 整个产品线的通用能力，Anthropic 自家的产品都带，Claude Desktop 也一样。到了现在，Skills 几乎成了行业标配，各家厂商陆续跟上，这股势头跟当年的 MCP 有点像。

一句话概括：**Claude 眼中的 SOP，就是 Skills。**

别急着划走，下面用大白话解释。如果这一段觉得绕，直接跳过去也没关系，后面实战会帮你建立起体感。

SOP——标准作业程序，这个词你应该见过。麦当劳在全球开了数万家门店，为什么每家做出来的巨无霸味道都差不多？不是因为每家店都请了大厨，而是后厨标准被写到了极致：肉饼煎几秒、酱料挤多少克、生菜放几片，全部有明文规定。换上任何一位新店员，按着这套流程走，出品都不会跑偏。

Skills 放到 Claude 身上，就是同一套逻辑。

没有 Skills 的 Claude 是什么状态？就像一个聪明但没受过培训的新人。你让它做一份年度汇报 PPT，它凭自己的感觉来，做出来也许能用，但字号混乱、配色随意、排版简陋——因为没人告诉它标准长什么样。

有了 Skills，情况完全不同。等于你递给它一本《PPT 制作标准手册》，从字体、字号、每页文字量到图表配色，规范写得一清二楚。它照着执行，出来的成果自然稳当、专业。

从技术底层看，Skills 本质是一份 Markdown 指令文档，相当于数字化的 SOP 文件，里面打包了三类信息：

• **操作步骤**：第一步做什么、第二步做什么、执行顺序如何
• **工具配置**：会用到哪些工具、具体怎么调用
• **质量标准**：交付物达到什么水准算合格、哪些雷区不能碰

这跟现实世界的 SOP 完全同构——把专家的经验转译成可执行的流程，执行者不需要自己从头摸索。

**Skills 的价值**

看懂「Skills = SOP」，价值感就出来了。

想想那些连锁品牌：海底捞的待客方式、星巴克的咖啡出品、胖东来的货架陈列，它们的核心能力并不是运气好招到了能人，而是把最优做法写进流程里，确保任何员工都能持续输出同一水平。

Skills 干的就是这件事，核心三个字：**稳、准、专**。

💡

• **稳**：结果不赌运气。没有 SOP 的餐厅，菜好不好吃全看厨师当天状态；没有 Skills 的 Claude 也一样，同一个任务今天的输出和明天可能差很远。一旦有了标准化流程，每次产出的质量都能保住下限。

• **准**：不用反复交代需求。以前你交代任务要写一大段：“用这个字体、标题加粗、表格带边框、结尾放个目录……”现在这些约定全都收进 Skill 里，你只需要说“做个 PPT”。就像你不需要每次提醒麦当劳店员“肉饼要煎熟、生菜要放两片”，SOP 里都写好了。

• **专**：装载的是经过反复验证的打法。Anthropic 官方出的 Skills 都经历了多轮测试和迭代，比如 Word 处理那个 Skill，里面连页眉页脚怎么安排、目录怎么自动生成、段落间距怎么控制都设定好了，全是前人踩坑换来的经验。自己研究可能要浪费大半天，用 Skill 直接省掉这段摸索时间。

更关键的一点：**你自己的 SOP，也可以写成 Skill。**

这是整套机制里最有想象力的一环。官方提供的是通用版本的 SOP，可每个团队、每个人都有各自的干活习惯：

• 公司周报有固定模板——可以做一个「周报 Skill」
• 前端项目有一套命名规范——可以做一个「代码规范 Skill」
• 👸号文章有专属排版风格——可以做一个「排版 Skill」

把这些写好之后，以后每次只需一句话，Claude 就会遵照你定下的规则行动。相当于你把手头多年的工作习惯，直接传授给了 Claude。

就像连锁品牌的加盟手册：把自己的方法沉淀为标准流程，Claude 就变成了一个完全听你指挥的虚拟员工。

**把 Skills 放进 AI 时代来理解，它就是新一代 SOP——让 Claude 不只会做，还能按最高标准稳定地做。**

**它的目录结构长这样**：

• `SKILL.md`：负责记录技能的元数据、触发条件以及核心逻辑（相当于大脑）
• `scripts/`：可选项，放一些能自动执行的小脚本
• `templates/`：放领域相关的代码模板或文档模板。理论上任何目录都可以，叫 `references/` 或 `api/` 都行，只要 SKILL.md 里把引用路径说明白

**Skills 和 MCP/Hooks 的区别**

💡说实话，光靠读定义，你可能还没完全吃透 Skills 到底是什么。

没关系，继续往下走就好。像做数学题一样——老师在黑板上推公式的时候，你记不住也不明白那些推导有什么用。那怎么办？刷题呗。

接下来的内容，就是不断动手、反复练习的过程。

![](img/3d84df49f152283f7f9f6229c01cd51d.png)

#### 2. 动手装一个 skills

其实每套 skills 的 README 里都自带安装指引。不过这一节着重聊一个被大家称作“神级”的安装利器！

💡它的定位很纯粹：专门解决 skills 的安装问题。

眼下主流编程工具很多：Claude Code、Codex、Gemini-CLI、Cursor……各家虽然都开始支持 skills，但安装路径并不统一，学习成本一下子就上去了。有没有一个工具，可以同时管理所有场景下的 skills 安装？vercel 给出了答案。

项目地址：https://github.com/vercel-labs/skills

Plain Text

```
https://github.com/vercel-labs/skills
```

vercel 刚推出的 skills 安装器，走命令行就能完成一键部署，兼容 30 多种 coding agent，claudecode、opencode、codex、gemini-cli、codebuddy、cursor、antigravity、kilo、droid 这些全部覆盖。

vercel 是专门做部署产品的一家公司，你没听过也没关系，把它当作靠谱的出品方就行。

教练碎碎念：这工具一出来，我花了两个小时截了一堆图的教程直接报废！惊不惊喜？意不意外？哈哈哈哈哈哈呜呜呜呜呜～

这个安装器的上手难度极低，先扫一眼 README 就明白了。里面列了各种各样的装法，你先大致浏览一遍，有个印象就好，现在不需要全部跑一遍。

需要留意的是，里面涉及的都是在终端执行的命令。苹果电脑用系统自带的「终端」，Windows 电脑用 PowerShell。

![](img/162bdafd534e23bb834d217f79115a09.png)

假设你看中了一套 skills，就用宝玉老师的这套来举例：

https://github.com/JimLiu/baoyu-skills

![](img/7d8d65d949ce143764a526e204744047.png)

这套包里收纳了不少 skill，完整的目录可以点下面的链接浏览：

https://github.com/JimLiu/baoyu-skills/blob/main/README.zh.md

![](img/36be362b322b3c22584dec8f019ae278.png)

现在创建一个新项目目录。比如我想做📕家装方向，先把文件夹命名为 `xiaohongshu-jiazhuang`。

![](img/114f1249e3eb2b53cf2843653abe4553.png)

进入目录后，在空白区域点右键，选择「在终端中打开」。

![](img/1b32c95a68ff05705f135c8976e4c416.png)

按工具说明，在终端输入下面这条命令：

Plain Text

```
npx skills add jimliu/baoyu-skills
```

回车

![](img/1ca40833281f17e8f31f66974cdbb505.png)

工具会自动爬取整个仓库，把里面包含的所有 skills 全部列出来。中途遇到报错或卡住，直接把截图丢给 Claude Code 帮你排查。

![](img/ab8b17ea659e49aed06c938165b67274.png)

包内每个 skill 都附了使用文档。比如目标是小🍠家装博主，通常会用到这几个：

• `baoyu-xhs-images`：生成📕封面图
• `baoyu-infographic`：信息图制作
• `baoyu-url-to-markdown`：抓取网页并转换成 Markdown

操作方式不复杂：上下方向键移动光标，**按空格勾选需要的项，最后回车确认**。

![](img/119abd84d6df5068c7596284c388db44.png)

回车之后进入 agent 选择页。这里建议手动指定目标，不要一股脑全选。比如我写文章的主力工具是 gemini-cli，那就只勾它。

界面上会出现三种选择：第一项是沿用上一次的选择，如果你是第一次使用这个工具，看不到这项；第二项是给电脑里所有 agents 都装一遍；第三项是自己挑。演示就用第三项。

![](img/7c4ead932e69edc476dd2a9ab0b89286.png)

同样用上下键导航，空格打勾，回车进入下一步。

![](img/85543a97f9a30d05fa336a612d2a7bb0.png)

我这边勾选 gemini-cli，回车。接着会让你选安装位置，这里最推荐选第一个 project，也就是装进当前项目目录。回车。

![](img/f68dc96acc2c44c312586b61dea0e76a.png)

安装方式采用默认的 symlink 就行。

![](img/ab64f26afebacc2398119213a3448259.png)

再按一次回车，它会列出实际的安装路径，目前可以看到是在根目录下面。最后一步是安装确认，选 yes，再回车。

![](img/f660bc9c433810ac4bb41929e1a92154.png)

到这儿就装好了。

![](img/bb0f878cde0836718f0eff93a3d645bd.png)

是不是比想的还简单？

💡最后补充几条安装纪律，建议牢牢记住：

1. 尽量别做全局安装，尤其是那些绑定特定业务场景的 skill，免得模型在处理无关任务时乱激活
2. 同一个项目里安装的 skills 最好别超过 10 个，装多了容易互相干扰
3. 不要设计“skill 调 skill”的套娃链路，推荐做法是在 AGENT.md 或 CLAUDE.md 里写清已装 skills 的使用场景和调用流程

**!! 风险提醒 !!**

另外，现在 skills 生态有些泛滥，OpenClaw 火了之后尤其明显，市面上冒出来不少留后门的恶意 skills，安全事故也不是头一回出现。装任何 skills 之前，一定先确认来源。

**来路不明的 skills 坚决不碰**，别拿自己的电脑和账号 token 去冒险。

![](img/57c84d63532ac183b498bdf89f601402.png)

#### 3. 好用的 skills 去哪找

## Skills 资源清单与自动配图实战

想找好用的 Skills，不妨先逛几个入口和 GitHub 热门仓库。下面这些资源适合当索引来了解，没必要一次全装；如果你已经装过 Skills，那可以直接跳到 1.4 的实操环节。

**Vercel 官方的 Skills 站**  
地址：https://skills.sh/  
![](img/c202f47696d85fddbfeae05d4a74dfd8.png)  
首推 Vercel 的 skills 市场。原因很直接：页面会统计通过 npx skills 安装的次数，某个 skill 被装得越多，通常说明用的人越多。不过有个坑要留意：find-skills 在每次执行 npx skills add 时都会被推荐，有人没细看就顺手装了，因此它的数字不能当真。判断热度时，主要看下方各 skills 的安装量。  
![](img/8c4f622a16ba0751b6cdbfc6bb4caa4e.png)  
在 skills.sh 的搜索框里输入 skill 名称即可。但它本身不具备语义识别能力，所以不适合当作“找想要技能”的搜索引擎，更适合看看最近哪些 skill 火了。  
![](img/4c34d8d9d98508671668c692eb62dec9.png)  
页面里还能看到排名，像 azure 系列 skills 的名次上升就很快。  
![](img/ca5852ff2d6c49c2798970b09a48b56a.png)  
挑一个感兴趣的，比如做网页动画的 remotion-best-practices。点进去后，按右侧复制按钮，再打开 CLI 就能安装，具体操作可回看 1.2 节。  
![](img/1935313fef7da10b122ca46ca1226202.png)

**韩国小哥搭的 Skills 站**  
地址：skillsmp.com  
![](img/5ba08bc39d64916239a46ec670797435.png)  
这个站几乎什么 skill 都能搜到，收录面很广，但没有官方背书，质量得自己把关。  
![](img/bc2252404b8acbc296dba02656cb13a1.png)  
进去后直接搜就行，它支持语义搜索。比如想找自动写作类，输入“写作”即可。  
![](img/5a1e0e2fb3ed2449617e4508e085282a.png)  
结果出来以后点进去查看详情。  
![](img/e11b6c745b3cd427c86fdfd14e23e12b.png)  
在右侧找到 skills.sh 的安装指令，复制到终端执行即可，具体见 02 部分。  
![](img/27c2cf8cc17c77916b406f6c1e3820c5.png)  
页面下方通常还有不少说明和相关内容，可以按兴趣翻看。  
![](img/40a8e5b475e7a920b09d6cedef0882a3.png)

**GitHub 上的仓库**  
GitHub 才是 Skills 的一手资料源。下面列几个仓库，大家可自行学习和安装。安装套路不复杂：看中某个 skill 后，到 skills.sh 搜它，再用 npx skills add 安装。

- **Anthropic 官方仓库**  
  地址：https://github.com/anthropics/skills  
  这是 Anthropic 官方的 skills 案例集，日常高频 skills 基本都收进去了。想研究 skill 怎么写，建议 clone 这个仓库，然后追着 claudecode 问到底，往往能挖到制作 skills 的关键技巧。  
  ![](img/64678eaeaaf0c3bbb769de3ecdc7b72b.png)

- **官方 plugin**  
  地址：https://github.com/anthropics/claude-plugins-official  
  plugin 属于 claudecode 专属插件，眼下也只有 claudecode 能跑，覆盖面没有 skills 那么广。差别在于它通常把 skills、mcp、subagents、hooks 等一并打包，装一次就等于拿到一套组合能力。  
  ![](img/51de9412470bbe1596d1642b012367f9.png)  
  以 ralph loop plugin 为例，它内含 command、hooks、scripts，形成一套相当能打的功能开发闭环。它并不是普通 skill，而是由自定义提示词、hooks 与自动化脚本拼成的完整插件。

- **Awesome-skills**  
  地址：https://github.com/ComposioHQ/awesome-claude-skills  
  ![](img/9af3aca7ea76504d62e7fe9aa5373aff.png)  
  这是个高星 GitHub 仓库。我最早做 skills 指北时，丢进 notebookLM 的材料就是从这儿提取的。八成以上的用户场景都能在里面找到对应内容，只是作者近期更新不勤。

- **Marketing-skills**  
  地址：https://github.com/coreyhaines31/marketingskills  
  这套 skills 面向独立站营销，做网站的人会很喜欢。从 SEO、定价到社媒运营都有涉及，建议去 skills.sh 逐个翻看。  
  ![](img/29c0bb4f853ccd892123c489a68007eb.png)

- **superpowers**  
  地址：https://github.com/obra/superpowers  
  这也是网站场景常用的 skills 集合。我尤其偏爱其中的 brainstorming，很多选题和点子都靠它打开思路。  
  ![](img/3fccc1a13bf2a2542fc84ee72335b2bd.png)

**全平台常用 Skills**  
需要提醒的是，高星或高安装量的 skills，大多偏向 AI 编程。搞 vibe coding 的人往往用得勤、写得也勤，并乐意开源。我常驻的几项如下：

- **Brainstorming**：来自 superpowers，属于脑暴类技能，擅长蹦出不少可用的创意；当你灵感不足时可以派上用场。  
```
npx skills add https://github.com/obra/superpowers --skill brainstorming
```
- **Doc-coauthoring**：来自 Anthropic 官方，文档撰写类 skills。它会先搭大纲，再逐章落笔，成稿质量相当能打，而且整体节奏基本由你掌控。  
```
npx skills add https://github.com/anthropics/skills --skill doc-coauthoring
```
- **Web-design-guidelines**：来自 Vercel，网页设计阶段调用，能帮你打开布局思路。  
```
npx skills add https://github.com/vercel-labs/agent-skills --skill web-design-guidelines
```
- **Frontend-design**：来自 Anthropic 官方，偏前端设计，和 web-design-guidelines 搭配效果更顺。  
```
npx skills add https://github.com/anthropics/skills --skill frontend-design
```
- **Shadcn-ui**：如果你的网站用了 shadcn/UI，可以装这个 skill。它会依据网页布局自动编写 shadcn 组件并嵌入页面，而不是把内容直接硬写死在页面里。  
```
npx skills add https://github.com/giuseppe-trisciuoglio/developer-kit --skill shadcn-ui
```
- **Vercel-react-best-practices**：网站完成后用它检查，能发现不少结构、布局和样式问题，效果不错，推荐用 codex 跑这个 skill。  
```
npx skills add https://github.com/vercel-labs/agent-skills --skill vercel-react-best-practices
```
- **seo-audit**：SEO 审查 skill。整站收尾后跑一遍，能审到 metadata、robots.txt、sitemap，还能看内页 keywords 与标题等。建议连跑两轮，把该修的都修掉。  
```
npx skills add https://github.com/coreyhaines31/marketingskills --skill seo-audit
```

如果你不做 AI 应用出海，也可以按自己的业务挑其他 skills。比如大家熟悉的 baoyu-skills（https://github.com/JimLiu/baoyu-skills），里面内容生成、自媒体相关的能力比较多。

- **baoyu-post-to-wechat**：👸号内容创作者的必备项，用来发布🛰️👸号文章。  
```
npx skills add JimLiu/baoyu-skills --skill baoyu-post-to-wechat
```
- **baoyu-xhs-images**：可产出 1—10 张📕信息图，内置 11 种视觉样式与 8 种布局。  
```
npx skills add JimLiu/baoyu-skills --skill baoyu-xhs-images
```
- **baoyu-post-to-x**：把内容发到 X（Twitter），支持文章以及带图或视频的推文。  
```
npx skills add JimLiu/baoyu-skills --skill baoyu-post-to-x
```
- **baoyu-cover-image**：用于文章封面，可输出 2.35:1、16:9、1:1 等比例。  
```
npx skills add JimLiu/baoyu-skills --skill baoyu-cover-image
```
- **baoyu-comic**：做知识漫画，能切换多种艺术风格，例如 Logicomix 和 Ohmsha 风。  
```
npx skills add JimLiu/baoyu-skills --skill baoyu-comic
```
![](img/24d04d4597a350f5ae75ba3b0dcd31c3.png)

**1. 自动配图 Skill 小试牛刀**  
写内容时，配图常常是最费手的一环：不找不行，找起来又琐碎。👸号、博客乃至其他文稿，都逃不过搜图、挑图、下图这一套动作，思路很容易被切碎，效率也跟着下降。

不妨自己搭一个配图 Skill：把文章交给 Claude Code，让它按内容产出风格契合的插画图。整个流程高度自动，喂进正文即可得到图片，适用范围覆盖👸号、博客和文档等多种文本。成本这块也能捏在手里：限制出图张数就能压住 API 开销，预设画风则能让整组图保持统一调性。

做完这个练习，你会练到：怎样把带接口调用的 Skill 需求讲明白；怎样拿到并填入第三方 AI 生图服务的密钥；怎样在需求里框定张数、画风等边界；以及怎样让 Claude Code 自己把 Skill 建好并配好。预计 5—10 分钟就能收工。

**4.1 和 Claude Code 对齐需求**  
在让 Claude Code 创建 Skill 前，先想清楚几个关键点：这个 Skill 做什么（自动为文章配图）；用哪个 API 服务（gemini-3-pro-image-preview，经 APImart 平台调用）；有哪些限制（图片数量、风格要求）；Skill 叫什么名字（方便后续管理和调用）。

操作步骤：  
步骤 1：启动终端或 IDE 里的 Claude Code，并进入你准备放 Skill 的目录再开聊。这样生成的文件不会跑到别处。  
![](img/39c2e7c3be48a0835b4772227aa7fc78.png)

步骤 2：输入需求描述。向 Claude Code 输入以下内容，可按实际情况调整：由于需要走 API，nanobanana pro 出图成本不算低，因此把数量卡在 3 张；配图希望带插画感，所以会补充画风限制；另外给 skill 起一个明确的名字，避免 cc 自动命名过于相似、后续分不清。  
```
我需要你帮我设计一个skill，这个skill主要是用来帮我实现文章配图。当我写完一篇文章之后，就可以调用这个skill，帮我文章配图。我的api是apimart，调用模型选择gemini-3-pro-image-preview（Nano Banana 2），这是模型调用的文档：https://docs.apimart.ai/

然后我的要求是：
每篇文章只要生成3张图片，前30%、中间30%、最后30%各一张图片。

图片中如果有文字的话，都需要使用中文；
图片风格固定成手绘漫画风格，温暖、亲和、有故事感，不偏写实、不偏赛博朋克，适合内容平台配图（横向或方形构图，画面干净，主体清晰）

这个skill的名字叫&quot;插画风格配图生成skill&quot;。
```  
PS：这时 Claude Code 可能读不到网站文档，可以把文档页面直接一键复制后发给 CC。  
```
https://docs.apimart.ai/
```![](img/55d369fc477d583723d2872a98ef8990.png)![](img/184deb12a94ff2ba6eab9d13fb751f12.png)

步骤 3：按 Enter 提交需求。输入完成后按下 Enter，让 Claude Code 开始理解需求并准备创建 skill。

注意：到这一步，Skill 已经创建好，但还没配置 APImart 的 API 密钥，需要继续下一步配置 API。  
![](img/d52bc69f10c72a8eaaaf9cc4b671ae3f.png)

**4.2 拿到 APImart API 密钥**  
APImart 是一个专业的 AI 模型 API 聚合平台，提供包括 gemini-3-pro-image-preview（Nano Banana 2）在内的多种 AI 图像生成模型。

选择 APImart 的原因：它的优势在于调用成功率有保障、接口稳定；计费按实际用量走，每张约 0.05 美元，成本一眼能算清；兼容多个主流图像模型；文档齐全，接入门槛低；还能做 4K 输出、图像编辑，并配有专业工具，商用也合适。

API 密钥获取步骤：  
步骤 1：注册并登录 APImart。先打开浏览器访问 https://apimart.ai/zh/model/nano-banana-2-api，进入 APImart 的注册登录页面。  
```
https://apimart.ai/zh/model/nano-banana-2-api
```  
点击页面右上角的【注册】或【登录】按钮。首次使用需要先注册，可用邮箱或第三方账号（如 Google、GitHub）注册；注册完成后用账号密码登录。这样就创建了 APImart 账户，后续所有 API 调用都会关联到这个账户。

注册成功后，系统可能会向你的邮箱发送验证邮件。打开邮箱找到邮件，点击其中的验证链接完成邮箱验证，以确认邮箱地址真实有效。

验证完成后，用账号密码登录 APImart，进入管理后台。  
![](img/8bba23b14e3e16283fe5155efdae926d.png)![](img/96dbb253e27ecbc3cca263b178b24b50.png)![](img/821e336e964c1bc5570cd8bc4c1ae8f6.png)

**步骤 2：进入密钥管理入口**

登录后，在界面找到【API 密钥】并点开，就能进入密钥管理区。这里集中处理 API Key 的新建、查看与维护。

![](img/24f3be9137ed6a5d4609aca7584081f5.png)

想新增一条密钥，点【创建 API 密钥】，弹窗出现后填一个容易辨认的别名（如“Claude-skill”），再按【确定】或【创建】。系统会即时生成新的 API Key 并显示出来，点【复制】把它收好。

![](img/7567061ba6404630f9b80e46fa87f270.png)

**重要提醒：**

API Key 相当于你在 APImart 的通行证，务必妥善保管。不可转交他人，也不要把含密钥的文件提交到 GitHub 等公开代码托管平台。若发生外泄，他人可能冒用你的账号发起调用，从而消耗账户余额。

**步骤 3：给账户存入余额**

到个人中心或账户管理区，点【账单】进入充值界面。APImart 要求先有余额、后使用服务，属于预付费机制。页面会列出若干金额档位，如 5、10、20、50 美元等；初次使用建议选 5 至 10 美元，足以跑通测试和早期调用。

![](img/5374e16c340f7dcbc8d51c4e96bcdae9.png)

选好金额后，点【充值】或【支付】，跳转到付款页，按提示选择信用卡、PayPal、支付宝等渠道完成付款。若用信用卡，需确认卡片支持 VISA、MasterCard 等国际支付通道；没有国际信用卡时，可改用 PayPal 或其他可用方式。

付款完成后，页面会展示最新余额，例如“账户余额：$10.00”，代表款项已入账，可以开始调用 API。

**为什么账户里要先有钱？**

预付费是 APImart 的使用前提。gemini-3-pro-image-preview 模型按调用次数收费，每次产出 3 张图，费用为 0.05 美元。系统会依据实际用量逐次扣款，未消耗的金额留在账户里，余额与消费明细都能随时查询。

**步骤 4：让 Claude Code 获取调用凭据**

拿到 API Key 后，可直接在 Claude Code 的对话窗口里粘贴。等它询问密钥时，把复制好的 token 发过去，它就会写入 Skill 配置，保证后续能正常请求 APImart 的图片生成能力。

```
我已经获取了APImart的API密钥，现在需要配置到刚才创建的&quot;插画风格配图生成skill&quot;中。

我的APImart API Key是：[粘贴你的API Key]

同时请确保skill能够正确调用https://apimart.ai/zh/model/nano-banana-2-api这个模型

请帮我：
1. 将API密钥配置到skill的配置文件中
2. 确保skill能够正确调用gemini-3-pro-image-preview模型
3. 配置完成后测试一下skill是否可用
```

若想更稳妥，也可手动写入。待 Claude Code 把 Skill 建好，打开其配置文件（一般在 .claude/skills/插画风格配图生成 skill/ 目录），找到存放 API Key 的字段，填入密钥并保存。这样可减少密钥留在聊天记录里的风险。

同时，把官方调用页面 https://apimart.ai/zh/model/nano-banana-2-api 一并发给 Claude Code，能帮助它理解接口参数与请求方式，缩短排查时间，提高搭建成功率。

```
https://apimart.ai/zh/model/nano-banana-2-api
```

该页面是 gemini-3-pro-image-preview 模型的官方说明，涵盖 API 文档、参数设置与示例代码。让它参考这份资料，有助于正确编写请求与响应处理，降低出错概率。

**注意事项**

- API 密钥安全：不对外分享，不把含密钥的文件公开上传；若怀疑外泄，立即到 APImart 后台删除旧 Key 并新建一条。
- 余额监控：定期进入账户管理页查看余额与消费记录，防止余额不足造成调用中断。
- 成本控制：gemini-3-pro-image-preview 每生成 3 张图收 0.05 美元，按次计费而非按张计费。建议限制生成数量，测试期先小批量跑，确认效果后再扩大。

![](img/8eec542cd4aa207f627d6ae9cef01897.png)

**4.3 静候 Skill 构建完毕**

需求描述和密钥配置完成后，Claude Code 会自动进入 Skill 构建流程。通常耗时 3 到 5 分钟，具体取决于 Skill 复杂度、API 文档解析速度以及网络状况。

![](img/4299c13af64ff56f82b03be74bc8300e.png)

后台里，它会先拆解你的需求，弄清功能边界与限制；再规划 Skill 结构，设计输入、输出与处理链路；随后编写核心代码，接入 gemini-3-pro-image-preview 的调用逻辑；接着生成配置文件；最后做基础语法检查与逻辑核验。几分钟后，配图 Skill 就建好了。

看到类似下面的提示，就说明构建已经成功：

```
✓ Skill &quot;插画风格配图生成skill&quot; 创建成功
✓ 配置文件已生成
✓ API调用已配置
```

**4.4 检验 Skill 能否正常使用**

**步骤 1：查看 Skill 列表**

在 Claude Code 里输入 /skills list，列表中出现刚建好的“插画风格配图生成 skill”，就表示注册成功。

```
/skills list
```

若你在 VS Code 插件里使用 Claude Code，该命令可能没有回显，可直接用提示词问：“列举下现在可以用的skills列表”。

**步骤 2：测试 Skill 功能**

调用这个 Skill 做一次测试，例如输入：
/插画风格配图生成skill "这是一篇关于春天的文章，描述了花开的美景和温暖的阳光。"

若流程正常，它会读取文章内容，请求 gemini-3-pro-image-preview API，并按照预设产出 3 张插画风配图，从而验证整条链路是否打通。

```
/article-image-generator &quot;这是一篇关于春天的文章，描述了花开的美景和温暖的阳光。&quot;
```

```
手绘漫画风格插画，展现传统编程与Vibe Coding的对比。左边是程序员对着满屏代码抓狂，头发凌乱，桌上堆满技术书籍，标注&#x27;传统编程:痛苦敲代码&#x27;。右边是轻松的人在和AI聊天，屏幕显示&#x27;我想要一个网站’，AI回复&#x27;马上为您生成&#x27;，标注&quot;VibeCoding:动口不动手’。温暖的色调，简洁明了的中文标注。
```

```
手绘漫画风格插画，展现&#x27;点菜式编程&quot;的概念。画面中央是一个友善的AI厨师机器人，戴着厨师帽，面前有一个菜单显示&quot;软件菜单:网站、APP、小程序&#x27;。旁边站着一个普通人指着菜单说&#x27;我要一个蓝色风格的登录网站，要简洁的&#x27;。AI厨师回答好的，马上为您制作’，手里端着一个发光的网页模型。背景是温馨的厨房环境，中文标注清晰。
```

**步骤 3：检查生成结果**

最后看图片是否达到预期：风格是否偏手绘漫画？画面是否扣住文章主题？清晰度是否够用？若效果不理想，可把需求里的风格说明写得更细，或修改 Skill 配置参数，也可以重新构建 Skill。

![](img/23567a0698e2c345afc2c8e2b3ef007e.png)

![](img/b7326df943d00b510a63e564e2184fa6.png)

**回顾与拓展**

做完这个 Skill，你已学会：如何向 Claude Code 讲清一个带 API 调用的 Skill 需求；如何取得第三方服务密钥并写入 Skill；如何用限制条件控制调用开销；以及如何命名、测试和验证自己搭建的 Skill。

它的使用面很宽：🛰️图文写完后可一键配图，提升发布速度；博客与社交媒体内容能快速补图；PPT、Keynote 可加入插画；技术文档、产品文档也能增加视觉元素。若想继续升级，可加入多种画风（写实、抽象、卡通等）、按文章长短自动决定出图数量、支持自定义尺寸、批量处理多篇文章，或把图片自动存到指定目录。

**4.5 高频疑问速答**

Q1：密钥填错了怎么处理？
打开 .claude/skills/插画风格配图生成 skill/ 目录下的配置文件，找到密钥字段，改成正确值并保存，然后重新测试。

Q2：出图不符合预期怎么办？
调用时把文章描述写得更具体，或调整 Skill 配置中的风格参数、修改 prompt 模板。若多轮调整仍不理想，可考虑换用其他图像生成模型。

Q3：APImart 余额用完会怎样？
调用会中断，Skill 无法出图，Claude Code 会给出错误提示。登录 APImart 后台充值后即可继续。

Q4：能换别的图像生成服务吗？
可以。选择 Replicate、DALL-E、Midjourney API 等支持 API 调用的服务，在需求中写明服务与接口，并按对应文档获取密钥，再让 Claude Code 重新创建 Skill。

Q5：碰到网络错误怎么办？
开启 TUN 模式（增强模式）。目前推荐 clash.verge 客户端，旧版 clashx 不再建议使用。英文常称 TUN 模式，中文叫增强模式或虚拟网卡模式。

![](img/2acdc7a93286ff7fb8c658b3e09a6f70.png)

### 02. 实战：用 Skills 打通自媒体自动发布

1. 👸号内容自动生成与发布 Skills

💡凡是流程化的工作，都值得交给 Skills。推荐大家动手学起来：用 Skills 发推文、发🛰️图文、发📕，能力边界很宽，而且能并行推进，比如同时产出👸号文章、📕笔记和视频脚本。

以前做👸号很费时间：定选题、写正文、找配图、点发布，一套走完可能半天就过去了。有了 Skill，找选题、写文章、配图、发布可以串成一条自动化链路。

完成这个 Skill 后，你会掌握：让 Claude Code 自动搜集 AI 热点、生成文章、调用 API 出图、把图片传到🛰️服务器、再送进👸号草稿箱。这个 Skill 比较复杂，会串联多个 API，但跟着步骤走，大约 30 到 60 分钟能完成。

**重点必看：**实战篇只需完成一个 Skills 案例即可，我们通过案例来掌握 Skills 用法。👸号的难度低于📕，新手建议先做出👸号 Skill，再进入进阶篇的 AI 视频创作 Skills。实操中遇到任何问题，都可以截图发给 Claude Code，让它帮你排查。

**1.1 先掌握这些要点**

**（一）👸号全自动 Skill 的运转全流程**

先看清整体链路，后面每一步才不会迷路：

第一步：搜索采集 AI 热点资料
借助 Exa 或 Tavily 两个 AI 搜索工具，查找 24 小时内指定主题（例如“open claw”）的最新消息，涵盖技术进展、市场反应、行业影响等，再结构化整理，作为写作素材。

第二步：撰写文章
根据搜到的资料，让 AI 写出一篇 Markdown 格式的文章。正文会遵循你设定的风格（技术深度、通俗易懂、行业分析等），并在需要插图的位置插入图片标记。

第三步：生成配图
解析文中的图片标记，提取每张图的描述（prompt），再请求 APImart 的 gemini-3-pro-image-preview 模型产出插画风配图，整体保持手绘漫画感、温暖、亲和、有故事性。

第四步：上传图片到🛰️服务器
把图片传到🛰️👸号素材库，取得每张图的 media_id，方便文章引用。

第五步：转换为 HTML 并发布到草稿箱
将 Markdown 文章转成🛰️👸号支持的 HTML 格式，把图片占位符替换成🛰️服务器上的图片 URL，再调用🛰️👸号 API，将文章送入草稿箱。

第六步：提示用户检查
Skill 会返回预览链接，提醒你到👸号后台查看文章。满意就发布，需要调整就在后台改完再发。

**（二）涉及的技术和工具**

这个 Skill 需要多个工具配合，先弄清各自职责：

Claude Code：核心开发工具，负责创建和管理 Skill。它能理解自然语言需求，自动写代码、配置 API 调用，是整个 Skill 的中枢。

Skill Creator：辅助工具，帮助快速搭出 Skill 的基础结构，自动生成配置文件、代码模板、文档结构，省去从零起步。

🛰️👸号 API：官方接口，允许用程序管理内容。它是整个 Skill 的关键，因为最终目标是把文章送进👸号。通过它，可以上传图片、创建草稿、发布文章、管理素材。

APImart：AI 模型 API 聚合平台，提供 gemini-3-pro-image-preview（Nano Banana 2）图像生成服务，用于出配图。相比手动搜图、筛图、下载，AI 生图能根据文章内容自动匹配风格、尺寸与画面。

Exa MCP：专业 AI 搜索工具，擅长深度检索与内容理解，用于采集 AI 热点资讯。

Tavily MCP：另一个 AI 搜索工具，擅长实时热点追踪，用来补足搜索结果，扩大资讯覆盖面。

**（三）学习目标**

完成这个 Skill 后，你会掌握：搭建复杂的多步骤自动化工作流 Skill；集成🛰️👸号 API、APImart API、Exa MCP、Tavily MCP 等多个第三方服务；处理数据采集、转换、上传、发布等完整链路；配置和管理 API 密钥；调试并优化 Skill 性能。

**1.2 安装 Skill Creator 与两个配套工具**

在创建👸号自动发布 Skill 之前，需要先安装 Skill Creator。它是辅助工具，能自动生成 Skill 的基础结构、配置文件和代码模板，让搭建过程更省力。

（一）Skill Creator 是什么？

# Skill Creator 从部署到需求规划

Skill Creator 本身也是一种 Skill，只不过它致力于帮你生成其他 Skill。你可以将其视为“Skill 作坊”：它熟悉标准 Skill 的骨架搭建、参数调整、API 对接等全套流程。

把它用起来的好处包括：
- 目录与配置文件全自动创建，无需手工整理
- 代码模板按需生成，不用从零敲代码
- 配置工作遵循最佳实践，省去纠错烦恼
- 支持增量更新和版本管理，后续改动很轻松

（二）Skill Creator 与两个工具的部署操作（见图）

步骤 1：启动 Claude Code

在终端或 IDE 中打开 Claude Code，确认它已经就绪，这样才能顺利进入 Skill 创建流程。

![](img/8b19f7c7eb43e1fd5b48aee550f2a32d.png)

这里提前部署 Exa 和 Tavily 两个 MCP

这两个 MCP 是 Skill 获取外部信息的重要通道，后续运行 skills 时会频繁使用，因此优先装好。核心思路是：先去官网注册并拿到 API Key，再把配置指引发给 Claude Code，由它自动修改配置文件。

**背景知识**

**什么是 MCP？**

MCP 即模型上下文协议（Model Context Protocol），它是一套标准协议，允许 AI 模型连接外部工具与数据源。你可以类比浏览器的插件系统，Claude Code 借助 MCP 也能扩展自身能力。

默认情况下，Claude Code 只能消费你直接投喂的信息，不会主动上网搜索。接入 MCP 后，它就能调用外部搜索、数据库、API 等，从而获取实时资讯。

在我们的 Skill 场景里，MCP 让 Claude Code 可以搜索 24 小时内的 AI 热点。没有它，Claude Code 只能依靠训练数据写文章，无法触及最新动态；有了它，Claude Code 能实时检索互联网，文章内容自然更新鲜、更贴合当下。

如果放弃 MCP，你只能手动检索资料，再复制粘贴给 Claude Code，让它基于这些资料写作。这不仅费时，也无法自动化。而接入 MCP 后，这一切都能自动完成：给 Skill 一个主题关键词，它就会自己搜索、筛选、整理并生成文章，全程无需操心。

**Exa 与 Tavily 各有什么本事？**

两者都是专业的 AI 搜索工具，但侧重点不同。

Exa 在深度搜索和内容理解上更强。它不是做简单的关键词匹配，而是能理解搜索意图，找到真正有价值的内容。同时，Exa 还具备质量评估能力，会过滤广告、垃圾、重复等低质信息，只留下可靠的高质量内容，确保后续文章建立在可信信息源上。

Tavily 则偏向实时热点追踪。它面向新闻和热点做了专门优化，能很快找到 24 小时内的最新消息。比如你搜“AI 最新新闻”，它会优先呈现几小时内或几天内的报道，而不是过时内容。此外，Tavily 还擅长多源整合，能从新闻站点、社交媒体、技术博客等渠道汇总信息，拼出完整全貌，不放过重要动态。

**为什么两个都要？**

因为两者优势互补。Exa 能挖到高价值和深度的内容，但实时性弱一些；Tavily 能快速捕捉最新动态，但深度有所欠缺。同时使用，可以先让 Tavily 找到当日热点，再让 Exa 提供深度解读，这样生成的文章既有新闻性，又有分析价值。

**只用其中一个行不行？**

没问题。预算有限或不想配置两个 MCP 时，只用一个也是可以的。真要选，优先考虑 Tavily，因为它更贴近 AI 热点追踪。不过，单一来源会让文章质量略有波动，因为信息面变窄了。

**部署 Tavily MCP**

步骤 1：访问官网并注册

打开浏览器，输入 https://tavily.com 并回车，进入 Tavily 的注册页。

Plain Text

```
https://tavily.com
```

页面加载后，点击右上角的【Sign up】或【Get Started】按钮，开始注册。

你可以使用 Google 账号快速注册（推荐）：点【Sign up with Google】，在弹出窗口选择账号并授权即可。没有 Google 账号时，也可以用邮箱注册，填写邮箱和密码，点【Sign up】即可。

注册完成后，系统可能发送验证邮件。去邮箱打开邮件，点击验证链接完成验证，以激活账号。

![](img/cdbcba526f0128d31956a2199790258e.png)

**步骤 2：获取 API Key**

完成验证后返回 Tavily 并登录，页面会自动进入 Dashboard（仪表板）。在 Dashboard 中找到【API Key】或【API Keys】，一般位于左侧菜单或顶部导航。点击进入密钥管理页。

页面上会显示一个默认的 API Key（注册时自动生成），以“tvly-”开头，形如“tvly-abc123def456”。点击旁边的【Copy】按钮复制，再妥善保存。

**注意：**

Tavily 有免费额度，通常每月可调用约 1000 次（以官方最新政策为准）。免费额度耗尽后需升级付费方案，测试或初期使用通常够用。

![](img/fbf8ade47adf4590e8e59895a4c853e6.png)

步骤 3：让 Claude Code 接入 Tavily MCP

拿到 API Key 后，回到 Claude Code 对话界面，发送如下内容：

请安装 Tavily MCP，我的 API Key 是 tvly-xxxxxx（替换为刚才复制的 Key）

Plain Text

```
请帮我安装Tavily MCP。我的API Key是tvly-xxxxxx
```

这样 Claude Code 就会帮你完成 Tavily MCP 的配置，写入 Key 并激活。它会做这些事：检查是否已装，未装则下载安装；找到 MCP 配置文件（通常位于 .claude/mcp/ 目录）；把 Key 写进配置；重启 MCP 服务使配置生效；最后测试运行。

正常情况下 1~2 分钟就能搞定，界面会显示进度。看到“Tavily MCP 安装成功”的提示，即表示完成。

![](img/51b9ed246c9be31716375a77527679dd.png)

**部署 Exa MCP**

步骤 1：访问官网并注册

打开浏览器，进入 https://exa.ai ，回车后到达 Exa 的注册页面。

Plain Text

```
https://exa.ai
```

页面加载后，点击右上角的【Sign up】或【Get Started】开始注册。这里可以用 Google 账号或 GitHub 账号快速登录，点对应按钮并在弹出的窗口授权即可。

**步骤 2：获取 API Key**

注册并登录后，会自动跳转至 Dashboard。在 Dashboard 中找到【API Keys】或【Developer】选项并点击，进入密钥管理页。

![](img/17952fd08c311cf64c6c0068b92e1cc9.png)

在密钥管理页，点【Create API Key】或【Generate Key】生成新 Key，再点【Copy】复制并保存。

**注意：**

Exa 同样提供免费额度，每月有一定的免费调用次数（以官方为准）。超过免费额度后需升级付费方案。

步骤 3：让 Claude Code 接入 Exa MCP

拿到 API Key 后，回到 Claude Code 对话界面，发送下面的内容：

请安装 Exa MCP，我的 API Key 是 xxxxxx（替换为刚才复制的 Key）

Plain Text

```
请帮我安装Exa MCP。我的API Key是xxxxxx
```

Claude Code 会自动配置 Exa MCP，写入 Key 并激活。流程与 Tavily 类似，通常 1~2 分钟完成。看到“Exa MCP 安装成功”的提示即代表就绪。

![](img/d03bb468201e1e6ea00815e7a75e9c49.png)

**步骤 2：请求安装 Skill Creator**

另外再开一个窗口，在 Claude Code 对话界面输入：

Plain Text

```
请帮我安装Skill Creator这个工具。我需要用它来创建一个复杂的公众号自动发布Skill。
```

这会让 Claude Code 明白你要安装 Skill Creator，它会从官方仓库或推荐源拉取并部署。

![](img/669e6254388ad971bdf0cf5f9830c641.png)

**步骤 3：等待部署完成**

Claude Code 会下载并安装 Skill Creator，视网络情况约需 1~2 分钟。期间它会显示下载文件、创建目录、配置环境等进度信息。看到类似“Skill Creator 安装成功”的提示时，就说明装好了。

Plain Text

```
✓ Skill Creator 安装成功
✓ 配置文件已生成
✓ 工具已就绪
```

![](img/df85380470bcb938a4335f895198cffc.png)

步骤 4：验证是否可用

装完后，有必要确认一下。在 Claude Code 中执行命令：

Plain Text

```
/skills list
```

如果是在 VS Code 插件中用 Claude Code，这条命令可能没有输出，可以直接用下面的提示词：

列出当前可用的 skills 列表

后面即可查看已安装的 Skill 清单，确定 Skill Creator 在不在其中。

![](img/1b302baf18025bb4ba44f3dc2af6248f.png)

如果列表里有【Skill Creator】或近似名称，说明它已成功注册到系统。若没有，可能是安装有问题，那就重新装一次。

步骤 5：测试 Skill Creator

想确认它能正常工作，可以做个快速测试。在 Claude Code 中输入：

Plain Text

```
@skill-creator 帮我创建一个测试Skill
```

![](img/2adf341658a69b793bf5cfa0cede1e73.png)

如果一切正常，Skill Creator 会向你询问测试 Skill 的名称、功能说明、需要哪些 API 等信息。这说明它可以正式使用了。不需要真的创建测试 Skill，输入“取消”即可退出。

**（三）常见安装问题与对策**

问题 1：装好了却找不到 Skill 入口
原因可能是安装路径不对，或 Claude Code 没刷新 Skill 列表。解决：重启 Claude Code 触发重新扫描；输入 /skills refresh 手动刷新；检查配置文件里的安装路径是否正确。

问题 2：提示“权限不足”
当前用户可能没有系统目录的写入权限。解决办法：Mac/Linux 下用 sudo 提升权限；Windows 下以管理员身份运行 Claude Code；或者把 Skill 装到用户目录，避开系统目录。

![](img/d08d620d5583f44a37e0da8842480d72.png)

1.3 和 Claude Code 把思路捋明白

动手创建 Skill 前，要先把自己的需求讲给 Claude Code，让它认真思考怎么落地。这一步很关键，尤其是复杂需求，不梳理清楚就开工，很容易出现功能残缺、逻辑混乱，甚至完全跑不起来的情况。

**（一）为什么要先梳理？**

你可能会问：直接说“给我做个👸号自动发布 Skill”不就行了？干嘛费劲先梳理？

因为“👸号自动发布”这个需求背后藏着很多子任务：热点挖掘、文章生成、配图、上传、发布等等。如果跳过梳理，Claude Code 可能会给出一个过度设计、塞满无关功能的方案，导致开发难、调试久；也可能方案太简陋，缺了关键能力，没法真正用起来；还可能没考虑技术或成本约束，方案根本不可行或调用 API 太贵。

所以，先和 Claude Code 一起厘清需求边界，确认技术方案是否靠谱，再动手开发。这就像盖房子之前先画图纸，前期多花点时间，后面能少走很多弯路。

**（二）需求沟通操作（见图）**

步骤 1：向 Claude Code 说出初步想法

在 Claude Code 对话界面里，描述你想实现的功能。这里有个技巧：需求描述后面加上“ultrathink”，这会促使 Claude Code 进入深度思考，产出更详尽周全的方案。

可以这样输入：

Plain Text

```
我要做一个全网自动做AI热点，自动写文章，自动配图，自动上传发布的skill，先不要直接写这个skill，我们先梳理一下思路，怎么样才能高质量的实现这个功能，ultrathink
```

这样做的目的是让 Claude Code 先给出整体实现思路，而不是立刻动手写码。“先不要直接写这个 skill”这句提示很关键，它强调了当前是规划阶段，而非执行阶段。

![](img/a1963767bdc4e20f01307b567dbefc65.png)

步骤 2：查看初步方案

Claude Code 会进入深度思考模式，分析你的需求并给出详细方案，可能包含多个模块和复杂架构。

比如它可能会给出：

**核心架构设计**

四大核心模块：

热点发现引擎：多源数据采集 + 智能评估
内容生成引擎：结构化写作 + 质量控制
配图生成引擎：AI 图片生成 + 风格统一
多平台发布引擎：差异化适配 + 自动发布

关键质量保证点

热点筛选质量：多维度评估（热度走势、时效性、受众匹配）；内容过滤（拒绝低俗、重复、过时内容）；智能去重（避免同质化热点反复处理）。

内容生成质量：结构化模板（标题优化、逻辑框架、SEO 布局）；深度控制（背景补充、多角度分析、数据支撑）；原创性保证（事实核查、语言润色、重复度检测）。

系统可靠性：微服务架构 + 事件驱动；多层审核机制（AI 初审 + 人工抽检）；风险控制（法律、平台、技术风险管理）。

实施路径建议

MVP 阶段：单源抓取 → 基础生成 → 简单配图 → 单平台发布
优化阶段：多源整合 → 质量提升 → 高质量配图 → 多平台适配
高级阶段：智能预测 → 个性化生成 → 互动功能 → 商业化

# 先跑通 MVP，再谈自动化

技术选型上，Python + FastAPI 负责应用后端，Redis 做缓存，PostgreSQL 存数据，Docker 管部署，这套组合就够用了。不过这个系统的成败，重点不在于“自动”到哪一步，而在于质量把关和风险控制。更稳的路径是：先做一个最小可行产品（MVP）来验证核心逻辑，之后再有针对性地优化每个环节。

乍看之下，完整方案确实写得很专业、很完备，可放到我们实际场景里，还是太复杂。像这种高复杂度需求，最好拆成多个 skill 分工去跑，硬塞进一个 skill 里，出错的概率会高很多。而且整套系统从零搭起来，可能要几天甚至几周，涉及的技术面又宽，新手很容易卡在半路。

所以，思路得调整：砍掉非必要功能，锁定核心需求，先交付一个能用的 MVP，再根据真实使用反馈逐步迭代扩展。

## 步骤 3：让 Claude Code 给方案瘦身

在向 Claude Code 提需求时，要把实际边界和限制条件一次性讲清楚。需要发送的提示如下：

指令内容：

```
我感觉这个操作流程太复杂了，我们的热点来自x，24小时内容热AI内容，发布平台暂时就限制在公众号，使用公众号的API进行发布，你简化一下这个方案，整体的逻辑实现按照这个逻辑来实现&quot;1. Exa/Tavily 搜索采集 AI 热点资料 → 2. 撰写文章（Markdown 格式）  →  3. 调用 nanobanana API 生成配图 → 4. 上传图片到微信服务器  → 5. 转换为 HTML 并发布到公众号草稿箱  → 6. 提示用户去微信公众号后台检查文章&quot;
```

![](img/07e1058a9decacafc5da9e2839db2763.png)

这么做是为了让它明确我们到底要什么、不要什么，别把方案设计得又大又全，把精力集中在能落地的部分。具体来说，我们加了这么几条硬约束：

- 热点来源：只从 x（Twitter）搜，不搞多源采集；
- 内容范围：只看 24 小时内的 AI 热点，其他领域不碰；
- 发布平台：只发🛰️👸号，不做多平台适配；
- 发布方式：先放草稿箱，人工最终确认，不自动发布。

这些限制能大幅削减系统复杂度，让可用的版本更早出来。

## 步骤 4：确认精简后的方案

接到简化需求后，Claude Code 会给出一个更务实、更易执行的方案。它的内容大致如下：

方案输出：

```
基于你提供的内容链路，我重新梳理了实现逻辑。这个方案更加实用和可操作：
核心实现逻辑
用户配置收集
输入: &quot;写一篇DeepSeek的文章&quot;
系统询问:
文章风格 (技术深度/通俗易懂/行业分析)
配图数量 (1-5张)
目标受众 (开发者/普通用户/投资人)
智能搜索采集

Exa/Tavily搜索 → &quot;DeepSeek AI 最新动态&quot; (24小时内)
提取关键信息 → 技术突破、市场反应、行业影响
结构化整理 → 为内容生成提供素材
内容生成引擎
基于风格指南生成文章 → 避免AI味
插入图片标记 → &lt;!-- IMAGE_1: DeepSeek logo科技感背景 --&gt;
Markdown格式输出 → 便于后续处理
配图生成流程
解析图片标记 → 提取prompt描述
调用nanobanana API → 生成高质量配图
中文prompt优化 → 添加&quot;simplified chinese&quot;标签
微信集成发布
上传图片到微信服务器 → 获取media_id
Markdown转HTML → 适配微信格式要求
替换图片占位符 → 使用微信mmbiz URL
创建草稿箱文章 → 调用微信API
用户确认环节
返回预览链接 → 用户可在微信后台查看
提供修改建议 → 基于用户反馈优化
一键发布选项 → 确认后直接发布
技术架构设计
Skill结构:
ai-wechat-publisher/
├── skill.md (工作流定义)
├── style-guide.md (写作风格)
├── wechat-api.sh (API封装)
├── image-gen.py (配图脚本)
└── config.json (配置管理)
关键优势:
一键操作: 用户只需提供主题关键词
质量保证: 风格指南 + 多轮优化
平台适配: 专门针对微信公众号优化
模块化: 便于维护和功能扩展
实施建议
MVP阶段 (1周):
基础搜索 + 内容生成 + 简单发布
完善阶段 (1周):
配图集成 + 微信API + 风格优化
优化阶段 (持续):
用户体验 + 错误处理 + 功能扩展
这个方案的核心是简化操作流程，让用户真正实现&quot;一句话生成公众号文章&quot;的体验。你觉得这个实现逻辑如何？
```

和初版相比，这个简化版明显靠谱多了：功能聚焦，多余设计被砍掉，技术实现也更直白。接下来就让 Claude Code 按这个方案动手实现。

### 数据流转示意

用一张简易流程图，可以更直观地看到数据在模块间是怎么走的：

流程示意图：

```
用户输入主题 → Exa/Tavily搜索 → 获取热点资讯 →
AI生成文章（Markdown） → 解析图片标记 →
APImart生成配图 → 上传到微信服务器 →
获取media_id → Markdown转HTML →
替换图片URL → 发布到草稿箱 →
返回预览链接 → 用户检查 → 发布
```

每条箭头都代表一次数据传递，各个步骤的输入、输出都写得很清楚。这样的设计让流程足够透明，哪个环节出了毛病，马上就能定位和修复。

![](img/322eb04527f1b8690a099cd3e7afb8e3.png)

## 1.4 备齐 Claude Code 需要的 API 资料

skill 的执行逻辑确定后，下一步是向 Claude Code 确认它需要哪些资料，然后再去收集。如果不知道操作流程，可以叫它输出分步说明，照着走就行。

### （一）先问清资料清单

先向 Claude Code 询问准备清单：

询问提示：

```
ok，这个逻辑没问题，接下来我们要进行实现了，你看看我需要你给哪些资料，比如API等。
```

这一步的目的是提前把 API 密钥、配置项等摸清楚，避免在创建 Skill 过程中缺这少那，导致中断。

![](img/f6b22a2d99057ffcb053d036900b957b.png)

Claude Code 会告诉我们，需要准备以下材料：

- 🛰️👸号的 AppID 和 AppSecret：用于调用👸号 API，是身份认证凭证；
- APImart API Key：用于调用 gemini-3-pro-image-preview 生成配图，属于付费服务凭证。

### （二）获取🛰️👸号 AppID 与 AppSecret

编程方式操作👸号，离不开 AppID 和 AppSecret 这两个凭证，它们的地位就相当于账号和密码。没有这两样，程序就无法调用👸号 API。

**AppID（应用 ID）**

AppID 是👸号在🛰️开放平台上的唯一标识，好比身份证号。每个👸号都有一个专属的 AppID，🛰️服务器靠它来识别请求来自哪个👸号。AppID 本身是公开的，可以直接写进代码。

**AppSecret（应用密钥）**

AppSecret 就是👸号的密码，得当成机密来保管，不能透露给任何人，也不能放进公开仓库。一旦泄露，别人就能冒用你的👸号身份调用 API，可能导致内容被改、数据被偷等严重问题。

**AppID 和 AppSecret 的关系**

两者需要配套使用，就像用户名配密码。调用 API 时，两个值要一起提交，🛰️服务器校验它们是否匹配，匹配通过后才会允许访问。

接下来是获取凭证的具体操作：

#### 步骤 1：进入开发者平台

浏览器访问 https://developers.weixin.qq.com/platform 并回车，进入🛰️公众平台的开发者后台，API 凭证就在这里拿。

```
https://developers.weixin.qq.com/platform
```

页面打开后是一个登录页，用🛰️扫二维码登录。这是为了确认操作者是👸号管理员，只有管理员才能拿 API 凭证。手机端确认后，页面会自动跳转到开发者平台主页。

#### 步骤 2：进入👸号管理页

登录完成，在页面顶部找到【我的业务】菜单，展开后点【👸号】，即可进入👸号管理页面，相关的开发配置都在这个页面里处理。

![](img/e663f4482ce406c13f262c03b06ea8b9.png)

#### 步骤 3：获取开发密钥

在👸号管理页，从左侧或下方找到【开发密钥】或【开发设置】入口并点击，进入密钥管理页，在这里可以查看或生成 AppID、AppSecret。

![](img/36f20b82994d2b646cdaf2b2b4876602.png)

这个页面会展示两项关键内容：

**AppID（开发者 ID）**

AppID 通常直接列出，是一串以“wx”开头的字符串，例如“wx1234567890abcdef”。点右侧的【复制】按钮，粘到文本文件里，后续配置 Skill 会用到。

**AppSecret（开发者密钥）**

AppSecret 不会明文显示，页面上只有一串星号（**）。要重新生成，需点击旁边的【重置】或【生成】按钮，这时系统会弹窗提示：“重置密钥后，旧密钥将立即失效，使用旧密钥的应用将无法调用 API，是否确认重置？”点【确定】继续。

接着系统会要求身份验证，一般是扫码或输入验证码。验证完成后，页面展示新生成的 AppSecret，它是一段随机字符，例如“a1b2c3d4e5f6g7h8i9j0k1l2m3n4o5p6”。这个验证环节保证只有👸号管理员本人能拿到密钥。

**特别提醒：**

AppSecret 只在生成时完整显示这一次，页面一关就再也看不到。所以最好马上点【复制】并保存到安全位置（密码管理器、加密文本等）。要是忘记保存，只能重新生成，旧的 AppSecret 会立刻失效。

#### 步骤 4：配置 API IP 白名单

IP 白名单是👸号 API 的一个安全机制，用来限定哪些 IP 能调用接口。即便 AppID 和 AppSecret 被别人拿到，只要 IP 不在白名单里，请求照样被挡在外面。这就像门锁：有钥匙（凭证）是第一步，名字还得在门禁名单（IP 白名单）里，门才会开。

如果跳过这步，Skill 调用 API 时会收到“IP 地址不在白名单中”的错误，整个流程跑不通，所以配置白名单是必要的前置动作。

具体操作：在开发密钥页往下翻，找到【API IP 白名单】或【IP 白名单】，点旁边的【修改】或【添加】，把允许调用 API 的 IP 填进去。

**怎么查自己的公网 IP？**

配置之前，得先拿到自己设备的公网 IP。这里有三种方法：

**方法一：在线查询（最省事）**

打开浏览器，访问 https://ip.cn 或 https://www.ip.cn，页面会直接显示你当前的公网 IP，比如“36.112.123.45”。

```
https://ip.cn
https://www.ip.cn
```

**方法二：搜索引擎**

在百度或 Google 里搜“我的 IP”或“my ip”，一般第一条结果就会给出公网 IP。

**方法三：命令行（适合技术人员）**

Mac 或 Linux 用户，打开终端输入 `curl ifconfig.me`，回车即可看到公网 IP。Windows 用户则在命令提示符（cmd）里执行同样命令（需要先装 curl）。

**注意：**这里要的是公网 IP，不是局域网 IP。像 192.168.x.x、10.x.x.x 这类内网地址无法从外网访问，填进白名单没有意义。

**添加 IP 到白名单**

在【API IP 白名单】旁点击【修改】或【添加】，在输入框里填上刚才查到的公网 IP（如“36.112.123.45”），保存即可。系统可能会再次要求验证身份（扫码或验证码），验证通过后 IP 才算真正加入白名单，以防非管理员乱改安全设置。

**另一个提醒：**👸号 IP 白名单最多加 5 个地址。如果你的公网 IP 常变（比如家庭宽带的地址由运营商动态分配），建议把 Skill 放到云服务器上运行（阿里云、腾讯云等），云服务器 IP 固定，配置一次就能长期使用。

**动态 IP 的应对思路**

家庭宽带或移动网络下，公网 IP 可能隔段时间就变。等 IP 变了，需要重新登录开发者平台更新白名单，否则 API 就调不通。针对这种情况，有四个可选方向：

- **方案一：定期手动更新** —— 如果 IP 不常变（几周甚至几个月才动），每次变更后手动改下白名单即可。成本最低，就是有点麻烦。
- **方案二：动态域名解析（DDNS）** —— 有一定技术基础的话，可以用花生壳、Cloudflare DDNS 等，把固定域名绑到动态 IP 上。IP 虽然会变，但域名不变，不过👸号白名单不认域名，这个方案还得配其他技术一起用。
- **方案三：使用云服务器** —— 买一台阿里云、腾讯云或 AWS 的云主机，把 Skill 部署上去。云主机 IP 固定，一次配置长期有效，且成本不高，入门配置每月只要几十块。
- **方案四：固定 IP 代理** —— 租一个固定 IP 的代理服务器，让 Skill 通过代理访问👸号 API。本地 IP 怎么变都无所谓，代理 IP 是稳的，不用总去更新白名单。

### （三）获取 APImart API Key

之前 1.5 节在搭建自动配图 skill 时，已经详细说明过怎么获取 APImart API Key，这里直接复用即可。如果没有的话，可以回到 1.5 节按步骤重新生成。

补充一句：用其他平台提供的 API 也可以，只要支持 nanobanana pro 就行。拿到 API 密钥后交给你 Claude Code 即可。

## 开始创建 Skill

所有材料到位后（👸号 AppID、AppSecret、APImart API Key、Exa MCP、Tavily MCP 都配置完毕），就可以正式创建 Skill。

向 Claude Code 发送创建指令：

指令内容：

```
我感觉这个操作流程太复杂了，我们的热点来自x，24小时内容热AI内容，发布平台暂时就限制在公众号，使用公众号的API进行发布，你简化一下这个方案，整体的逻辑实现按照这个逻辑来实现“1. Exa/Tavily 搜索采集 AI 热点资料 → 2. 撰写文章（Markdown 格式）  →  3. 调用 nanobanana API 生成配图 → 4. 上传图片到微信微信服务器  → 5. 转换为 HTML 并发布到公众号草稿箱  → 6. 提示用户去微信公众号后台检查文章”
```

这一步让 Claude Code 按我们确定的简化方案开始搭建 Skill，并理清每个步骤的执行顺序和逻辑。

![](img/a80a6e24cf62651a2046939489ffd9e1.png)

Claude Code 会开始创建，整个过程通常需要 5–10 分钟，具体看 Skill 的复杂度和网络速度。

![](img/cb2e42755634364e2cf481b661328cc7.png)

![](img/135e4a14f9c16a8f739cda598ef33bf6.png)

![](img/34e9784c0dae6b86ac52e99d13f9d70d.png)

![](img/50ef2351804635318c1b97912ddf2326.png)

## 1.5 收尾：配置白名单并测试调用

Skill 创建完成后，还要做最后的配置和测试，保证它能正常工作。

**依赖检查**

先确保系统已安装 jq 和 curl。如果没装，可用下面的命令安装：

Mac 下：brew install jq curl

```
brew install jq curl
```

# 👸号与📕发布自动化实战

正式动手前，先补齐 Skill 依赖的两个命令行工具。

Ubuntu 或 Debian 环境执行：

`sudo apt-get install jq curl`

```
sudo apt-get install jq curl
```

Windows 系统则要先装 Chocolatey，再运行：

`choco install jq curl`

```
choco install jq curl
```

这两个工具分工明确：jq 负责 JSON 解析，curl 承担网络请求发送，缺一不可。

**完整验证 Skill 链路**

下面把 Skill 从头到尾跑一遍，确认搜索、成文、配图、投递这几个环节都能衔接上。

环节 1：下一条测试指令

在 Claude Code 里输入：

`@ai-wechat-publisher 写一篇关于 open claw 的文章`

这条指令用来检验基础能力：它会围绕 open claw 抓取近期热点，完成写作与配图，再把结果送进👸号草稿区。默认采用技术深度路线，配 3 张图，资讯范围限定在一天内。

```
@ai-wechat-publisher 写一篇关于open claw的文章
```

环节 2：盯住执行反馈

Skill 启动后，界面会陆续出现进度信息，顺着提示观察即可。

环节 3：核对产出结果

执行结束后，登录🛰️公众平台后台（https://mp.weixin.qq.com），依次点开【素材管理】→【草稿箱】，找到刚产出的那篇稿子，确认内容与图片是否符合预期。

![](img/f0a161b835b3d9c1186c5854a7f2ac01.png)

草稿箱里应能看到完整成品：标题、正文、配图都在。点开预览，重点核对四件事——标题是否有吸引力、内容是否准确、图片是否清晰、版式是否整齐。确认无误后点【发布】即可推送；若想调整，先在后台编辑再发布。

**进阶玩法**

不想用默认配置，可以在指令里写清风格、配图数量、目标读者等条件：

`@ai-wechat-publisher 帮我搜一下最新的 GPT-5 资讯，写一篇深度分析，目标受众是开发者，生成 5 张配图，发到👸号`

```
@ai-wechat-publisher 帮我搜一下最新的GPT-5资讯，写一篇深度分析，目标受众是开发者，生成5张配图，发到公众号
```

这样 Skill 会从这句话中提取搜索对象、写作路线、读者画像和配图数量，再按这些条件产出内容。

**1.6 常见疑问速查**

Q1：成稿效果不理想，如何优化？

可以从以下方向调整：

• **关键词再具体些：** 调用时别用“写一篇 AI 文章”这类宽泛说法，换成“围绕 DeepSeek 技术突破写一篇深度分析”更有效。关键词越明确，搜索结果越匹配，成稿更稳。

• **完善风格指南：** 打开 style-guide.md，写清写作口吻、语言风格、内容深度。例如补充“少用‘当下这个时代’‘科技日新月异’之类空话”“每个观点都要有数据或案例支撑”。

• **增加结果数量：** 在配置里把 max_results 从 10 调到 20 或 30，让 Skill 有更多素材可选。不过结果变多，成本和耗时也会上升。

• **接入更优质的搜索源：** 若 Exa 和 Tavily 的结果不够理想，可增加 Google Scholar（学术搜索）、Hacker News（技术社区）、Reddit（讨论社区）等渠道。

• **保留人工审核：** 即便内容由 AI 产出，发布前也值得通读一遍，检查逻辑、表达和事实，必要时润色修改，确保质量稳定。

Q2：常见报错怎么处理？

• **“IP 地址不在白名单中”：** 先访问 https://ip.cn 查看当前公网 IP，再更新白名单。

• **“APImart API Key 无效”：** 确认复制时没有混入空格或换行，并检查 Key 本身是否有效。

• **“余额不足”：** 登录后台查看账户余额，不够就充值。

• **“文章生成失败”：** 打开日志文件定位原因，然后重新运行 Skill。

• **“图片上传失败”：** 检查图片大小、格式是否正常，再排查网络连接是否稳定。

Q3：API 调用成本

**Exa/Tavily API：** 按搜索次数计费，每次约 0.01 到 0.05 美元。假设每天产出一篇、每篇搜索一次，月成本约 0.30 到 1.50 美元。

**APImart API（gemini-3-pro-image-preview）：** 每次 0.05 美元，可生成 3 张图片。按每天一篇、每篇 3 张图计算，月成本约 1.50 美元。

**🛰️👸号 API：** 不收费，完全免费。

![](img/f524ffc87cf9c5d4201b26d6ab8674fe.png)

**2. 📕内容的自动生成与发布 Skills**

📕是国内活跃度很高的内容社区，也是许多创作者和品牌重点运营的阵地。每天手动写文案、做配图、再发布，工作量确实不小。借助 Claude Code，这条链路可以从创作到发布实现自动化。

完成本案例后，你将掌握一套完整流程：让 Claude Code 自动生成📕风格内容、调用 AI 产出配图，并通过 Cookie 认证把笔记自动发到📕。

该案例需要借助 GitHub 开源项目，涉及 MCP 插件、Skill 安装、Claude SDK 使用以及 Cookie 配置，技术门槛略高；只要跟着步骤走，仍可顺利搭起来。预计耗时 40 到 60 分钟。

**注意：本案例难度偏高。👸号与📕两个案例二选一即可，新手建议先做👸号；21 天内跑通一个 Skills 案例就算有收获。**

**2.1 安装📕 MCP 插件**

💡动手前先装 xiaohongshu-mcp。MCP 相当于 Claude Code 的扩展接口，装上后它才能访问📕、发布笔记。

关于 xiaohongshu-mcp

这是一款专为 Claude Code 打造的📕平台集成插件，让 Claude Code 能与📕直接交互。借助它，可以获取账号信息、发布笔记、上传图片、管理草稿等。项目开源，由社区开发者维护，代码托管在 GitHub。

它的价值在于：内容发布可全自动完成，无需手动登录网页或 APP；支持批量操作和定时发布；还能与其他 MCP、Skill 组合，搭建完整的内容生产链路。

步骤 1：启动 Claude Code

打开 Claude Code 对话界面，确认网络可正常访问 GitHub，以便下载 MCP 插件。

步骤 2：发出安装请求

在对话框输入：

`请帮我安装 xiaohongshu-mcp，项目地址是 https://github.com/xpzouying/xiaohongshu-mcp`

```
请帮我安装xiaohongshu-mcp,项目地址是https://github.com/xpzouying/xiaohongshu-mcp
```

Claude Code 收到指令后，会从 GitHub 克隆项目、解析结构、安装依赖，并把 MCP 注册进系统。

![](img/7bd32ae3adbf0d39c071d880c4e489e8.png)

步骤 3：等待安装完毕

安装通常需要 2 到 5 分钟，快慢取决于网络速度和项目体量。看到成功提示，就说明 xiaohongshu-mcp 已就绪。

![](img/77030fc74b5959b82bfbc6a03815f899.png)

**2.2 安装智能内容创作 Skill**

💡MCP 就位后，再装 smart-content-creator-skill。它专门产出📕风格的标题、正文和话题标签。

关于 smart-content-creator-skill

这是一款为📕内容创作优化的 Skill，内置平台内容规范和风格指南。只要给出主题或关键词，它就能生成符合平台调性的内容——有吸引力的标题、结构清晰的正文、恰当的 emoji、热门话题标签等。

使用它的好处是：内容更贴合📕读者的阅读习惯，标题更容易获得曝光；正文结构清楚、可读性强；还会自动补齐话题标签，提高被发现的机会。

步骤 1：让 Claude Code 协助安装

把这套开源项目直接交给 Claude Code，让它自动完成安装。在对话框输入：

`请帮我安装 smart-content-creator-skill，项目地址是 https://github.com/ginobefun/smart-content-creator-skill`

```
请帮我安装smart-content-creator-skill,项目地址是https://github.com/ginobefun/smart-content-creator-skill
```

Claude Code 会拉取 Skill 代码、解析配置文件，并安装到本地 Skills 目录。

![](img/f4bce84d24b345cd60d059459c76836c.png)

安装时，不同 AI 模型给出的反馈可能略有差异，根据回答多尝试几次即可；遇到不明白的地方，多向 AI 提问。

步骤 2：等待安装完成

通常需要 1 到 3 分钟，Claude Code 会自动完成 Skill 的注册与配置。

![](img/a0eec2ad2c77459ecc9c21040bf266a0.png)

步骤 3：验证安装结果

装完后，可以在 Claude Code 中查看 Skill 列表：

```
/skills list
```

以此确认 smart-content-creator-skill 是否已出现在可用列表中。

若通过 VS Code 插件使用 Claude Code，这条命令可能没有回显，此时直接发提示词即可：

`列举下现在可以用的skills列表`

![](img/586571811e55a3ad8a76028a1f4ef8ca.png)

**2.3 使用 Claude SDK 连接功能**

💡现在 xiaohongshu-mcp 和 smart-content-creator-skill 都已就位，还差 Claude SDK 把它们串起来，才能真正跑通自动化。

关于 Claude Agent SDK

Claude Agent SDK 是 Anthropic 官方提供的 Python 开发工具包，方便开发者调用 Claude 能力，并把多个工具和服务连接起来。借助 SDK，可以编写自动化脚本，让 Claude Code 按既定流程执行任务。

在本案例中，SDK 扮演“中间人”：先调用 smart-content-creator-skill 生成📕内容，再调用 xiaohongshu-mcp 把内容发到平台，整条链路无需人工介入。

步骤一：安装 Claude SDK

第一，确认 Python 环境。

先确保电脑已安装 Python 3.8 或更高版本，在终端执行检查：

```
python --version
```

这样做是为了确认系统环境满足 Claude SDK 的运行要求。如果版本不达标，可以让 Claude Code 代为安装。

第二，向 Claude Code 发送安装指令。

把 GitHub 上的项目交给 Claude Code，让它自动安装 SDK。在 Claude Code 中输入：

```
请帮我安装Claude Agent SDK,项目地址是https://github.com/anthropics/claude-agent-sdk-python
```

![](img/3348563cd739154b44eb08ac5497d1c6.png)

Claude Code 会自动安装 SDK 及其依赖包。

第三，等待安装完成。

过程一般需要 3 到 5 分钟，Claude Code 会下载并配置好必需的 Python 包。

SDK 需要配置 API Key。之前配置 Skill 时若已设置过 API key 和 base url，可以直接对 Claude Code 说“帮我复用当前的 API key 和 base url”。也可以重新申请，获取方式见对应链接。若打算配置其他 API key（比如 kimi），可前往官网（https://platform.moonshot.cn/console/api-keys）领取后交给 Claude Code。

![](img/25afa3f07c0764a8d5860bbbeef16043.png)

步骤二：配置自动化流程

第一，让 Claude Code 创建连接脚本。

在 Claude Code 中输入以下指令：

```
请帮我创建一个自动化脚本,使用Claude SDK连接smart-content-creator-skill和xiaohongshu-mcp,实现从内容生成到发布的完整流程。
```

![](img/3c67eca68808aab6ab3a86fa54041d2c.png)

Claude Code 会编写连接代码，处理两个组件之间的数据传递和流程控制。

![](img/e54055b65c18daffd88855b92d096fc1.png)

第二，查看生成的脚本。

Claude Code 会创建一个 Python 脚本文件，通常存放在当前工作目录。这样做是为了让你了解自动化流程的具体实现逻辑。

![](img/55b4d0e44881e7305e1cb84d33f0d69d.png)

第三，报错就用 AI 解决。

正式使用前，建议先跑一次测试，确保脚本运转正常，把潜在问题提前暴露。

在终端切换到脚本所在目录：

`cd /path/to/your/script`

```
cd /path/to/your/script
```

然后运行测试命令：

`python3 xiaohongshu_auto_publish.py`

```
python3 xiaohongshu_auto_publish.py
```

观察输出。如果看到类似下面的内容，说明脚本一切正常：

✓ 连接 smart-content-creator-skill 成功

✓ 连接 xiaohongshu-mcp 成功

✓ 测试运行完成

![](img/a7904bb93b732e7a4ee496d7e9f39cf4.png)

若出现报错，直接把错误截图发给 AI，多沟通几轮通常就能解决。

常见的调试节奏：

第 1 轮：运行脚本 → 出现报错 → 截图发给 Claude Code；

第 2 轮：Claude Code 修复 → 重新运行 → 若仍有问题 → 再截图发给 Claude Code；

第 3 轮：Claude Code 再次修复 → 重新运行 → 成功。

![](img/6a1eb43d0ca3606c36d31981a277b923.png)

2.4 📕 Cookie 提取法

💡 若打算让 Claude Code 替你往📕发笔记，前提是先把账号的“身份证明”交给它。📕靠 Cookie 判断来者是谁，所以第一步要从浏览器里把这串凭据捞出来，再填进 xiaohongshu-mcp。

**Cookie 认证是怎么回事**

网站分辨访客身份，靠的就是 Cookie 这门技术。你在网页版登录📕之后，平台会往浏览器里塞进一段凭据，此后每次操作都带着它表明“我是谁”。xiaohongshu-mcp 拿着这段凭据，就能模仿真实浏览器的动作，以你的名义把内容发出去。

这里要强调：Cookie 等同于账号钥匙，分量跟密码差不多，必须收好，绝不能外传。它还有时限，一旦失效就得重新走一遍提取流程。

第 1 步：把 Cookie 拿到手

![](img/8244e5453edee1384e2ff2d6e1367636.png)

**先访问📕网页版，完成登录。**

建议用 Chrome、Edge 这类主流浏览器，打开 https://www.xiaohongshu.com ，在页面右上方点【登录】，扫码或手机号都行。这一步的作用是让浏览器先存下登录状态的 Cookie。

**第二步是把开发者工具调出来。**

登录成功后，按【F12】键（Mac 上是【Command + Option + I】）就能唤出它，目的是查看网络请求里带的 Cookie。也可以右键点【检查】，同样能进入。

![](img/38620b4cfe8624a2866feb4a1dad32e2.png)

**随后切到 Network 面板。**

在顶部菜单里找到【Network】（中文界面写作【网络】），点一下，浏览器发出的请求就会列出来。

![](img/1d8f6b5c6a9c3dcd0ccf7baba764c97e.png)

**接着刷新页面，让请求冒出来。**

敲【F5】或者点刷新图标，页面重载后，Network 列表里就会出现新的请求。

在列表中挑任意一条指向 xiaohongshu.com 的请求（通常第一条就行），点开它准备看携带的 Cookie。

![](img/49fbaebb86d80f65ae4e5045ea35dcae.png)

**最后一步，读取并复制 Cookie。**

右侧会展开请求详情，找到【Headers】（请求头）区域，往下滚到【Request Headers】（请求标头），里面有一行【cookie:】。点它后面的值，全选复制。这段字符通常是若干键值对拼在一起，形如 web_session=xxx；xsecappid=xxx; a1=xxx;... 必须整段复制齐全，认证才有效。

![](img/74206da596c5943c197f2b0154ba0f31.png)

第 2 步：把 Cookie 交给 MCP

**这件事同样可以交给 Claude Code 完成。**

先向它下达配置命令。

在对话框里敲入：

Plain Text

```
请帮我配置xiaohongshu-mcp的Cookie。我的Cookie是：[粘贴你刚才复制的完整Cookie字符串]
```

它便会自行定位配置文件，把 Cookie 填进去。

等上片刻，它会依次完成下列动作：

• 找到 xiaohongshu-mcp 对应的配置文件（多半在 ~/.config/claude/mcp_config.json 这类路径下）

• 在文件里锁定 xiaohongshu-mcp 这一项

• 把凭据内容填进去

• 存盘

耗时大约半分钟以内。

**收尾时确认一下结果。**

屏幕上会打出两行提示：

✓ Cookie 配置成功

✓ xiaohongshu-mcp 已更新配置

**安全须知**

就 Cookie 而言：别把它转给任何人；带凭据的配置文件切勿推送到公开仓库；每隔一段时间换一次（一个月左右为宜）；一旦怀疑外泄，立刻在📕 App 里退出账号，所有 Cookie 会随之作废。

就账号而言：拿小号先跑通流程，别拿主号冒险；自动化工具不要用于违规操作；社区规范必须遵守；发帖节奏也要控制，免得被系统当成机器账号。

![](img/4e15c162205cbea35991fb3e692d3729.png)

**2.5 先测后发**

前期铺垫做完，接下来验证整套流程能否顺利产出并发出笔记。

第 1 步：验证内容产出

**先下一条测试命令。**

在 Claude Code 里敲入类似这样的指令：

Plain Text

```
@smart-content-creator-skill 帮我生成一篇关于春季护肤的小红书笔记
```

目的在于检验 smart-content-creator-skill 能否按要求产出📕调性的内容。

**再看它交出的结果。**

正常情况下，它会给出标题、正文、话题标签一应俱全的成品。逐项核对：文风是否对味、标题够不够抓人、标签贴不贴题，以此判断生成环节是否正常。

第 2 步：验证发布链路

**先下达发布命令。**

输入：

Plain Text

```
请使用xiaohongshu-mcp将刚才生成的内容发布到小红书
```

目的是检验 xiaohongshu-mcp 能否顺利调用📕接口把内容送出去。

**随后盯一下执行过程。**

界面会滚动显示进度：上传图片、创建笔记、发布成功等环节，据此判断链路是否顺畅。

**最后回平台核对。**

切到📕 App 或网页版，进入个人主页，确认新笔记是否已经出现，标题、配图、话题标签是否都正确，以此判定内容确实发出去了。

第 3 步：跑一遍全自动流程

前两步分别通过之后，就可以把它们串起来用。

**先发一条一键生成并发布的指令。**

Plain Text

```
请帮我生成一篇关于【你的主题】的小红书笔记并自动发布
```

一条命令就能把“生成内容—发布上线”整条链路串起来跑。

**接着等它跑完。**

一般要 2 到 5 分钟，具体看篇幅长短、配图多少和网速快慢。

**结束时看最终结果。**

跑完后界面会告知发布成功，并附上笔记地址。点开链接就能看到成品，说明整条自动化链路工作正常。

![](img/9d5c7f576643667ca4202a608e5c8532.png)

💡

**进阶玩法**

有余力的话，不妨再往前一步：让 Claude Code 把定时发布也安排上，做到每天到点产出一篇并发出。**定时发布的具体配置流程：**

第 1 步：写一个定时脚本

向 Claude Code 发送这句话：

请帮我创建一个定时发布脚本，每天上午 10 点自动生成一篇📕笔记并发布

它会据此写出一份带定时逻辑的脚本文件。

第 2 步：登记定时任务。**Mac/Linux 走 cron：**终端执行 crontab -e

在编辑器里补一行：0 10 * * * cd /path/to/your/project && python3 xiaohongshu_auto_publish.py 存盘退出（按【Esc】，敲 :wq，回车）。**Windows 用户则走任务计划程序：**按【Win + R】调出运行框，输入 taskschd.msc 回车，任务计划程序就开了

右侧点【创建基本任务】

取名（例如“📕自动发布”），点【下一步】

触发器选【每天】，点【下一步】

起始时间定在上午 10:00，点【下一步】

操作选【启动程序】，点【下一步】

“程序或脚本”一栏填 python3（或 python）

“添加参数”一栏填 xiaohongshu_auto_publish.py “起始于”一栏填项目目录，例如 C:\Users\YourName\xiaohongshu-project

最后点【完成】

**第 3 步：验证定时是否生效。**Mac/Linux：执行后等到次日，观察有没有自动发出。Windows：在任务计划程序里右击刚建好的任务，选【运行】，当场试一遍能否执行。提醒一句：机器得开着，定时任务只在开机状态下才会被触发。

**2.6 常见疑问速答**

Q1：为何走 Cookie 认证，不用账号密码？

📕接口本身不接受账号密码直登，身份校验交由 Cookie 完成。这种做法的好处是：凭据自带时限，万一外泄也会自行过期；代码里也不必留明文密码，风险更小。

Q2：Cookie 有效期多长？失效了如何补救？

一般是 30 到 90 天，看平台怎么定。一旦过期，xiaohongshu-mcp 会报认证失败，此时重新登录网页版，照前面的流程再提一次 Cookie、更新配置文件即可。稳妥起见，每月主动换新一次，免得用着用着突然掉线。

Q3：自动发笔记会不会招来封号？

内容合规、守规矩的前提下，风险并不高。但有几条底线要守：不碰违规题材（广告、虚假信息之类）；控制节奏，别在短时间里连发多篇；内容保持原创，不重复推同样的东西；多账号之间也别发一模一样的内容。正式启用前，用小号跑一阵，稳定了再换主号。

Q4：多个账号能不能一起管？

可以。每个号各自提一份 Cookie，在配置文件里并排写上多组，发布时指明用哪一组。但各号的内容要区分开，否则容易被判定为批量操作。平台规则同样要守，恶意营销、刷量这类动作别碰。

Q5：生成的内容能自己定风格吗？

能。smart-content-creator-skill 允许在调用时附带风格说明，比如要求“专业严谨”或“轻松活泼”的调性。也可以直接改 Skill 的配置文件，把默认风格定下来。产物不满意就多生成几次挑一版，或者生成后自己动手润色再发。

### 03.进阶：AI 视频创作 Skill 实操

1. 小说改编漫剧剧本 Skill 实战

**重点提示：进阶部分不必贪多，吃透一个 Skills 案例就够，用法正是在动手过程中摸清的；**

**这一章的两个案例里，前者门槛低于后者。新手不妨先啃下小说改编漫剧剧本这个 Skills，再转向 Open claw，借这一个案例把 Skills 的用法吃深；**

**动手时碰到任何卡点，截图发给 Claude Code，让它替你排查。**

把网文 IP 改造成短视频漫剧，眼下正是热门赛道。过去这条路依赖专业编剧班底，周期长、成本高。如今借 Claude Code，从小说原文到漫剧剧本可以走自动化：拆剧情、提冲突、标分集、写剧本，一条龙完成。

搭完这个案例，你将学会让 Claude Code 自行读原文、抓核心冲突与情绪钩子、按漫剧节奏切分集数、产出 500 到 800 字可视化剧本的全套方法。案例涉及较复杂的 Skill 配置、多个 Agent 协同、模板与示例文件的调用，整体不算简单，但只要紧跟步骤、善用 AI，依然能把它搭起来。**（版权、二创、人工审核这几关，真要商用，风险不小）**

建议先完成小说二创，再进入生成环节，把风险压下来。

![](img/77bb66f3d849702fef8ca9e776d11de2.png)

剧本.mp4【在线播放】

![](img/bacbfe275302ddd991325763e322b01f.png)

**1.1 整体流程拆解**

**阶段 1：拆解剧情（当前所处环节）**

Plain Text

```
📖 上传小说原文（每5章一批）
↓🔍 输入 /breakdown 开始拆解
↓⚙️ 调用 webnovel-skill 提取剧情点
↓✓  novelsame-agent 自动检查一致
↓💾 保存到 check-down.md
↓📊 标注分集（第X集）+ 状态（未用）
```

产出样例：

Plain Text

```
第1集：
剧情点1：主角被欺辱，激发复仇欲望（冲突强度：8/10）
剧情点2：意外获得神秘玄典（情绪钩子：惊喜+期待）
状态：未用
```

**阶段 2：撰写单集剧本**

Plain Text

```
📋 读取 check-down.md  中&quot;未用&quot;的剧情点
↓🎬 输入 /create 开始创作
↓⚙️ 调用 webnovel-skill 批量创作剧本
↓✓ novelsame-agent 自动检查一致性
↓💾 保存到 scripts/Episode-01.md
↓🔄 更新剧情状态为&quot;已用&quot;
```

![](img/ed981f13edca6cc90fbb1927fbc67299.png)

**1.2 下载项目并完成准备**

💡 动手前，先取一份完整的项目模板。里面配置文件、模板、示例素材都已备齐，下载后略作调整就能用。

**这个项目是做什么的**

**它是一套为网文改漫剧量身打造的工作流项目，**把从原文到剧本的自动化工具打包在一起。核心是一个叫 webnovel-skill 的 Skill，内嵌专业改编方法论，能自动判断小说类型、抓冲突点、标情绪钩子、做分集规划、产出可视化剧本。

最大的便利在于免去从零搭建：改编规则、输出格式、质量标准都已预设妥当，拿来即用。项目还配了两个质量检查 Agent，自动核查拆解质量与剧本一致性，让成品符合漫剧制作要求。

把下方的压缩包解压到好找的地方（桌面或文档目录都行），方便之后在 Claude Code 里直接打开。

[
![](img/2b18a427dc9a4a261ffb09639b42d0e4.png)
test.zip](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/CvKHbuPfroLk1OxTd7bcY2NHndc?response-content-disposition=attachment%3B%20filename%3D%22test.zip%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260526%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260526T190327Z&x-oss-expires=86400&x-oss-signature=ee64990e443e57737f498a0c054d085006b9050437682490d5f1b807c812058a&x-oss-signature-version=OSS4-HMAC-SHA256)

解压完成后，目录大致如下：

一眼看去层级不少，其实日常只需盯两个目录：novel（存放小说原文）与 scripts（查阅产出的剧本），其余文件都在后台自行运转。

Plain Text

```
project/
  ├── novel/                              # 小说源文件目录
  │   ├── chapter-001.txt                 # 第1章
  │   ├── chapter-002.txt                 # 第2章
  │   ├── chapter-003.txt                 # 第3章
  │   ├── chapter-004.txt                 # 第4章
  │   ├── chapter-005.txt                 # 第5章
  │   ├── chapter-006.txt                 # 第6章
  │   └── 《天逆玄典》作者：热乎冰棍儿.txt  # 完整小说
│├── breakdown.md                        # 剧情拆解+分集标注+使用状态
│├── scripts/                            # 单集剧本目录
  │   ├── Episode-1.md
  │   ├── Episode-2.md
  │   ├── Episode-3.md
  │   ├── Episode-4.md
  │   ├── Episode-5.md
  │   └── Episode-6.md
│└── .claude/                            # 配置目录
      ├── CLAUDE.md                       # 项目规则和主Agent配置
      ├── skills/
      │   ├── webnovel-skill/             # 网文改编漫剧skill
      │   │   ├── skill.md                # Skill主配置
      │   │   ├── adapt-method.md         # 改编方法论
      │   │   ├── output-style.md         # 输出风格指南
      │   │   ├── templates/              # 模板目录
      │   │   │   ├── plot-breakdown-template.md
      │   │   │   └── script-template.md
      │   │   └── examples/               # 示例目录
      │   │       ├── plot-breakdown-example.md
      │   │       └── script-example.md
      │   └── webtoon-skill/              # 预留目录
      │       ├── templates/
      │       └── examples/
      └── agents/
          └── novelsame-agent.md          # 单集剧本一致性检查Agent
```

![](img/da5fb7e4c7967f5e4ba7bc6ce378e41f.png)

1.3 先把小说原文备好

项目拉取下来以后，先别急着动手，得把待改编的小说原文备齐。类型方面没什么门槛，玄幻、武侠、都市、言情、悬疑、科幻都吃得下。

文件要求是 txt 纯文本，一章对应一个文件；命名最好排成 chapter-001.txt、chapter-002.txt 这种带顺序号的样子，读取时排错的风险更小。手头已有素材的话直接用自己的也行。当然，这里也放了一份现成的小说，下载解压就能用。

![](img/58e0482e90fc815bba7b8faff5ebc3e1.png)

[novel.zip](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/UNdLb4J4Go01PBxxWqycLTIjn1e?response-content-disposition=attachment%3B%20filename%3D%22novel.zip%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260526%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260526T190327Z&x-oss-expires=86400&x-oss-signature=ced8b1011c6641b313fda4013f61705b5f45ea4c1e3d2898e547d5a21830d1e8&x-oss-signature-version=OSS4-HMAC-SHA256)

![](img/44facc8f2d3a0530b23ac7202058021c.png)

![](img/2a4969d10843d5dcd4dc70ab896ba4f0.png)

1.4 拆剧情：改编的第一道关

原文到位，接下来进入拆解环节。这是整条改编链路的第一环，后面的剧本成色如何，很大程度上看它做得细不细。

拆解到底在做什么？简单说，就是从原文里捞出两类内容：一类是推动故事发展的枢纽事件——主角受辱、金手指觉醒、与对手正面碰撞；另一类是能把观众情绪拽起来的瞬间——打脸爽感、虐心痛感、真相浮出水面。

项目自带的改编方法论会先判断作品属于哪个赛道（玄幻、都市、言情等），再按赛道特征去筛。玄幻方向偏重境界跃迁、越级压制这类内容；言情方向则盯住误会生成、情感拉扯。

筛完之后，系统会把剧情点按漫剧的节奏摊到各集头上，保证每一集都不缺冲突张力与情绪浓度。

步骤 1：把 Claude Code 跑起来

打开终端，或者命令行窗口。

![](img/1fd9992a76f3091a12756a4d561111f9.png)

启动claude code.mp4【在线播放】

![](img/1881da5c6772bc97833de6aa4ee35797.png)

在项目目录里用 cmd 唤起 Claude Code。它会读取 .claude 文件夹下的配置并回显相关提示，顺便确认加载状态正常。

万一弹出报错，把截图丢给 Claude Code，让它替你分析成因。

![](img/e95261dd93c795e7555ae98a40bbcfbf.png)

![](img/52aa630c2e72b62035706a1e18b1bc9a.png)

![](img/3d10ebd085acf8cc43282a02116f5a75.png)

步骤 2：说明作品名与赛道

Claude Code 起来之后，配置也已读完，接着要告知它改编对象是谁、属于什么类型。

这里千万别漏：先把前面那个压缩包解开，把小说文件安置到 novel 目录中。

![](img/f9fa2208d1a01c0b976a5cd3a3a33b8b.png)

在对话框里交代作品信息，比方说：我要改编一部小说，名字是《天逆玄典》，类型是玄幻。目的很明确——让它认出目标作品，并据此挑选对应的改编打法。

Plain Text

```

我要改编一部小说，名字是《天逆玄典》，类型是玄幻
```

它会复述一遍作品信息，再问你是否进入拆解。等于确认前期准备没有遗漏。

**P**S：截图跟下面的图示有出入属正常，出现你需要的内容就往下走；卡住了就把截图发给 Claude Code。

![](img/db9d4d6f811ac1631563cdd18d6462f5.png)

![](img/b3c27b49c48c215bdc229c864ad410b4.png)

![](img/7194544a70959f6131dc3df1d81ded70.png)

步骤 3：下达拆解指令

在 Claude Code 里敲入 /breakdown，用来唤醒拆解流程，webnovel-skill 随即开工。用中文“拆解剧情”同样能触发。

Plain Text

```
breakdown
```

要留意：这里输入的本质是一条 breakdown 提示语，本身就能生效。如果带上斜杠，可能与 Claude Code 的自定义命令机制打架，弹出“命令不存在”的报错。

随后它要你定夺：章节由你点名，还是让它扫 novel 目录。既然文件命名是 chapter-001.txt 这类规范，回一个 scan 让它自己扫过去就行，等于告诉它处理范围。

Plain Text

```
scan
```

再强调一遍：这条提示语直接敲进去就能跑；前缀斜杠有概率与自定义命令设定冲突，到时候跳出找不到命令的提示，别慌。

![](img/2fe4fbd5c8a36ce1b626daa072022c45.png)

系统开始通读原文，捞取冲突点与情绪钩子，并打上分集标记。整轮耗时约 3 到 5 分钟，章节多、篇幅长的话会再久些；这段是 AI 干重活的时间。

步骤 4：验收拆解成果

屏幕上出现“完成！我已经完成了第 1 到 6 章的剧情拆解和分集标注”字样，就意味着这一批处理到位了。

![](img/d9ac0669cad3079d15b6467f1d4aee6f.png)

去项目目录找 breakdown.md，打开后能看到对应内容；借此判断拆得准不准、剧情点是否立得住、分集是否匀称。

接着 novelquality-agent 会接手质检，核对冲突抓取准不准、钩子密度够不够、分集划分合不合理。过关会亮出 PASS；有问题则列出具体修改意见。质量关口由它把关。

步骤 5：剩下的章节接着拆

书还没拆完的话，再发一次 /breakdown，系统会接着处理下一拨章节，直到全书走完。

![](img/8e3d54be0be3f5aa0ceb6e31cb4d8781.png)

1.5 一集一集出剧本

拆解告一段落，就可以动笔写单集剧本了。它是能直接拿去拍漫剧的脚本，场景、动作、台词、特效标注一样不少。

剧本环节的重心，是把拆出来的剧情点翻译成看得见的画面。具体会做这么几件事：从 breakdown.md 里挑出标记为“未用”的剧情点；据此写出一集 500 到 800 字的本子；用画面语言交代场景与动作；补上特效提示和结尾卡黑；落盘到 scripts 文件夹；同时把该剧情点改成“已用”。

产出的剧本贴着漫剧的节奏标准走，每一集冲突够密、爽点够足，契合短视频平台的观看习性。

步骤 1：下达创作指令

在 Claude Code 里输入 create，唤起剧本生成流程，webnovel-skill 开始产出。

Plain Text

```
create
```

注意：这个触发词直接输入即可生效；带斜杠有概率和自定义命令设定冲突，弹出找不到命令的提示。

它会问你要写哪几集，单写第 1 集可以，一口气写到第 6 集也行。等于告诉它产出多少。

系统会逐集读取剧情点、逐集生成本子，平均每集 2 到 3 分钟；重活依旧交给 AI。

![](img/45813630649808abaadd2ef23cd975dc.png)

步骤 2：验收剧本成品

看到“第 1 集剧本已完成”的提示，就说明这一集写好了。

到项目目录的 scripts 文件夹里，能看到 Episode-1.md、Episode-2.md 之类的文件，打开即可查看内容。

![](img/38dd62d348182f4b5b47cb9dd448b110.png)

随手点开一个剧本，看看 AI 写了什么；借此核对格式是否贴合漫剧制作，场景、动作、特效的标注清不清楚。

与此同时，novelsame-agent 会做一致性核验，比对剧本与 breakdown.md 里的剧情点有没有跑偏。质量底线由它守住。

1.6 配置层里藏着什么

走完这一圈，从小说到剧本的全流程你已经跑通了。不过你大概会琢磨：凭什么敲个 /breakdown 就能自动拆？凭什么 Agent 会自己查质量？背后是怎么搭起来的？

**配置文件都在干什么**

.claude/ 目录下躺着几个关键配置，整条改编链路的规则由它们共同写就：

[CLAUDE.md](http://CLAUDE.md)：项目的指挥中枢，主 Agent 演什么角色、按什么次序干活，全由它定，说白了就是“何时做何事”。它给 Claude Code 立了规矩：/breakdown 一到，走拆解流程；/create 一到，走创作流程；拆解收尾，交给 novelquality-agent 质检；剧本收尾，交给 novelsame-agent 查一致性。有了它，Claude Code 清楚自己在这个项目里是编剧身份——调度 webnovel-skill 做专业改编，安排双校验 Agent 把关，整条生产链路都写死在这个文件里。

[skill.md](http://skill.md)：webnovel-skill 的本体，管的是“这个 Skill 能干哪些事”。能力清单列得很明白：类型判别（玄幻、都市还是言情）、剧情拆解（捞冲突点与情绪钩子）、分集标注（按漫剧节奏摊剧情点）、单集创作（500 到 800 字画面化本子）、内容修订（按反馈打磨）。它还规定了各阶段读哪些文件、套什么模板、参照哪些样例，让流程有章可循。

[adapt-method.md](http://adapt-method.md)：改编方法论，只操心一件事——改编本身该按什么章法来。冲突识别（核心、次级、过渡怎么分）、钩子提取（打脸蓄力、碾压爽点、金手指觉醒怎么认）、密度压缩（小说内容怎么压进漫剧节奏）、分集策略（剧情点怎么摊到各集）、节奏公式（每集冲突与爽点怎么保底），整套方法论都写在这里。

[output-style.md](http://output-style.md)：只管 AI 写出来的东西“长什么样”，剧情对不对它不问，只问画面感够不够、节奏快不快、爽点密不密、能不能直接开机拍。场景用※标，动作用△标，特效走【特效】标记，每集收尾必须挂悬念，台词短促有力、单句不超 20 字。有它在，剧本拿来就能投产。

**样例与模板**

examples 目录下有两个参照：plot-breakdown-example.md 演示剧情点怎么写、集数怎么标、情绪钩子怎么挂、状态怎么管，AI 照着这个骨架仿写；script-example.md 演示场景如何落笔、动作如何标注、特效往哪加、悬念怎么卡，是 AI 熟悉画面语言的范本。

templates 目录下有两个骨架：plot-breakdown-template.md 框定拆解的固定版式，让结构不出岔子；script-template.md 框定剧本的固定结构，让每一集都具备可制作性。

**这样拆分的意义何在**

好处是便于你自己动手改。想换改编打法，动 adapt-method.md；想换剧本版式，动 output-style.md；想加新指令，动 CLAUDE.md。彼此独立，改一个不牵连其他，维护和复用都省心。

1.7 高频疑问速答

Q1：小说为什么要切成多个文件？

Claude Code 单文件处理有条数上限，整本书塞进一个文件容易撑爆。切成一章一文件，系统就能分批消化，质量有保障，长度也不再是障碍。切分之后还更好管理，想改哪几章就挑哪几章。

Q2：拆出来的剧情点偏少，怎么补？

# 分镜老跑偏？先用基准锁住画风

遇到“冲突密度不足”的提示，别急着推翻稿子。通常有两种解释：这几章原文本身缺少强核心冲突，或者工具判断偏保守。你既可以回到小说正文人工排查遗漏的冲突点，确认后补写到 breakdown.md；也能在 adapt-method.md 里把核心冲突的识别门槛放宽。

**Q3：成片风格跟预期不一样，怎么调？**

改 output-style.md 里的规则即可。想要对白更密，写明“对白篇幅不低于三成”；想让动作更细，加一条“每个动作至少两句话铺开”。改完再跑一次 /create，新设定就会生效。

**Q4：多本小说能不能一起改？**

能，但更推荐一本书一个独立项目目录。因为 breakdown.md 和 scripts 目录由项目共用，混放容易串内容。操作上复制整份项目，一本一份，分别处理。

**Q5：商用可以吗？**

可以，但四件事要守住：拿到原小说改编授权，不碰版权红线；机器生成的剧本必须人工复核润色，不能原样拿去商拍；商业项目最好在 AI 初稿上继续原创加工；同时遵循各平台内容规范，别踩违规内容。

![](img/a2667674dbf28620f1ad930fa2a6a086.png)

## 1. 从剧本到镜头：分镜生成技能

## 2.1 整条流水线怎么转

**注意：** 该案例难度不低。小说改漫剧、剧本转分镜两个案例，完成其中一个即可；如果你是新手，建议先做完实战篇里的一个案例，再接着学 Open claw。21 天里能完整跑通一个 Skills 案例，就算有收获，不要求全部做完。

💡 **这一节要带你做成什么**

先设想：你有一份不错的剧本，想把它变成可执行的分镜画面。过去要联系分镜师，讲需求、等返稿、反复调整，几周很容易过去。直接让 AI 来，也有坑：角色第一张黑发、第二张金发；这一格向左走、下一格向右走；有画面像新海诚，有画面像皮克斯，整体不统一。

**AI 分镜师**

这个项目就是针对这些痛点设计的。

3.1 节里，我们已经把网络小说改成了漫剧剧本。现在手里的剧本每集都有明确剧情点、冲突设计、情绪钩子。

接着使用 **AI 分镜师** 这个 skills，让三个专业 AI 助手协同，把剧本自动转成可用于 AI 出图和图生视频的提示词。它有一套“渐进式视觉展开”的方法论，专门处理人物一致性、镜头连贯性、风格统一性，实际上是一套完整的智能工作流。

**跑完这个案例，你能拿到什么？**

• 一套完整的 AI 分镜生成 skills，能把剧本片段转成分镜脚本
• 9 格关键画面提示词（叙事锚点图），一眼看清故事发展脉络
• 45 个动态指令（图生视频用），可直接用于 Seaweed Dance 等 AI 视频工具

**首次搭建预计用时：** 90—120 分钟。

动手前先看整体流程，心里有数。

**阶段 1：提炼叙事节点**

```
📖 输入小说文本
↓🤖 视觉叙事师分析剧情
↓📊 识别14个叙事节点
↓🎯 选出9个关键锚点
↓✓ 质量把控审核
↓💾 保存到 narrative-nodes.md
```

这一阶段要从小说里抓出真正推动情节的关键转折。可以理解成看完电影后还记得的重场戏。系统会自行判断哪些情节点重要、哪些可以略去。

**阶段 2：叙事锚点图（9 格）**

```
📋 读取叙事节点分析
↓🎨 视觉叙事师生成9格提示词
↓🖼️ 每格包含：构图+光影+色彩+人物描述
↓✓ 质量把控审核（检查人物一致性、风格统一性）
↓💾 保存到 anchor-prompt.md
```

这一阶段会产出 9 个关键画面的详细描述。这 9 格像故事的主干，把人物外形、场景气质、整体色调先确定。后续画面都拿它们作参照。

**阶段 3：动势展开图（36 格）**

```
📋 读取叙事锚点图
↓🎬 视觉叙事师展开每个锚点
↓📐 每个锚点展开成4格（起承转合）
↓🧬 继承锚点的&quot;视觉DNA&quot;（人物、风格、色调）
↓✓ 质量把控审核（检查连贯性）
↓💾 保存到 unfold-prompt.md
```

这一阶段在 9 个关键画面之间补充过渡画面，让叙事更顺。相当于动画中的“中间帧”，保证动作衔接不突兀。

**阶段 4：动态指令（45 个）**

```
📋 读取锚点图+展开图
↓🎥 动态设计师生成运动指令
↓📝 每格定义：镜头怎么动、人物怎么动、节奏快慢
↓🌍 输出英文指令（AI视频工具支持更好）
↓✓ 质量把控审核
↓💾 保存到 kinetic-prompt.md
```

这一阶段把静止画面变成动态视频。每格画面都会配运动说明，告诉 AI 视频工具：镜头推进、人物转身、云层飘动等。

**为什么不直接让 AI 一次出 36 格，而要分“9 格→36 格”两步？**

因为 AI 分镜常出现三处硬伤：人物长相变来变去、镜头接不上、画风各行其是。

这套流程采用渐进式视觉展开：先把锚点立住，再向细节扩展。像画一面长墙，若从一头直接画到尾，很容易失控；更稳妥的是：

1. 先勾素描草图（叙事节点分析），把主要元素位置定好；
2. 再做 9 张彩色小样（叙事锚点图），确定视觉风格、人物外貌、色调；
3. 最后照小样补足细节（动势展开图），每个区域都以 9 张小样为参照。

**关键机制：视觉 DNA 传递**

例如生成第 3 组展开图（“主角进入游戏”这组）时，系统会把第 3 格锚点图作为参考图片交给 AI。AI 看到参考图后，会继承其中的人物外貌、服装、发型、光影风格。类似让画师画同一角色：第一次需详细描述，第二次直接把第一张图递过去，说“照这个画”。

![](img/0bc415546563611591d28b3a78c4381e.png)

## 2.2 用一个实例跑完整个流程

先不纠结技术细节，跟着一个实例从头到尾跑一次。

**场景设定**

假设你是一名短剧创作者，手里有网文改编剧本，目标做成 9:16 竖屏短剧，画风想要“日漫·新海诚”。

**第一步：准备工作（2 分钟）**

**1️⃣ 确认项目结构**

打开项目目录，先检查结构是否符合预期。

```
AI 分镜师/
├── script/          ← 这是放剧本的地方
├── outputs/         ← 这是生成结果会保存的地方
└── .claude/         ← 这是系统配置（你不用动）
```

**2️⃣ 放入剧本**

剧本保存为 .md 或 .txt 后，放进 script/ 目录。可以新建第一章.md，把正文放进去。这里也备了一份示例：

![](img/4c3940faceb5c3919e4365f934ae447f.png)

[ch01-第一章.md](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/KPUMbz3baoPqrzxYtOjcxpjgnOc?response-content-disposition=attachment%3B%20filename%3D%22ch01-%E7%AC%AC%E4%B8%80%E7%AB%A0.md%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260526%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260526T190327Z&x-oss-expires=86400&x-oss-signature=2b26ed4a313416bc6093107cbc57b0fe8f29fa3f3512351eaa1c00c1bdec97c4&x-oss-signature-version=OSS4-HMAC-SHA256)

**注意：** 文件名没有硬性限制，但带上集数更利于多集管理，比如 ep01-创世.md 或 ch01-开局.md。

**第二步：启动系统（3 分钟）**

**1️⃣ 打开 Claude Code**

在终端进入项目目录，启动 Claude Code。

**2️⃣ 系统初始化**

启动后会自动检查项目状态，屏幕上会出现类似这样的欢迎语：

```
👋 你好！我是一名专业的AI项目统筹，我将负责协调视觉叙事师、
质量把控和动态设计师完成影视分镜工作。

让我们开始吧！

📊 项目进度检测

**剧本文件**：
- 第一章.md [未开始]

**当前集数**：第一章
**当前阶段**：叙事节点分析阶段
```

![](img/2019910d7a6d89cc5fc6392e4eac933c.png)

若发现缺少所需项目目录，它也会补齐。

**3️⃣ 配置项目信息**

系统会连问三项。

**问题 1：视觉风格**

风格库大致分五路：写实类有真人写实、电影胶片、纪录片；3D 类有皮克斯、迪士尼、梦工厂、3D CG；2D 类有日漫、日漫·新海诚、日漫·吉卜力、国漫、国漫·水墨；艺术类有概念艺术、油画、水彩；特殊类有赛博朋克、蒸汽朋克、黑色电影。这里选 **日漫·新海诚**。

**问题 2：目标媒介**

可选电影、短剧、漫剧、MV、广告。这里选 **短剧**。

**问题 3：画幅比例**

可选 16:9 横屏、9:16 竖屏、21:9 超宽、1:1 方形。这里选 **9:16**。

三项答案会被记录，作为后续全部生成工作的基准。

**第三步：输入“继续”，让系统自动工作**

![](img/88c3e77898a1b665021c38c1c5ef9720.png)

从这里起，操作只剩输入“继续”。

**1️⃣ 第一阶段：叙事节点分析**

系统开始分析：

```
现在开始调用视觉叙事师进行叙事节点分析...

[视觉叙事师工作中...]

✅ 叙事节点分析已完成！

已通过质量把控审核并保存：
- outputs/narrative-nodes-ch01.md


下一步 → 输入&quot;继续&quot;生成叙事锚点图提示词
```

你输入：**继续**

![](img/dcb361bd6ed784b9596c560f9c74a3b5.png)

**2️⃣ 第二阶段：叙事锚点图**

继续推进：

```
[视觉叙事师工作中...]
[质量把控审核中...]

✅ 叙事锚点图提示词已完成！

已通过质量把控审核并保存：
- outputs/anchor-prompt-ch01.md

下一步 → 输入&quot;继续&quot;生成动势展开图提示词
```

你输入：**继续**

![](img/3c32ebb921c84a8490b0c33f18bd1059.png)

**3️⃣ 第三阶段：动势展开图**

继续推进：

```
[视觉叙事师工作中...]
[质量把控审核中...]

✅ 动势展开图提示词已完成！

已通过质量把控审核并保存：
- outputs/unfold-prompt-ch01.md

下一步 → 输入&quot;继续&quot;生成动态指令
```

你输入：**继续**

![](img/90ec95b000eb59809863e4bf934fb5b6.png)

**4️⃣ 第四阶段：动态指令**

最后生成动态指令：

```
[动态设计师工作中...]
[质量把控审核中...]

✅ 动态指令已完成！

已通过质量把控审核并保存：
- outputs/kinetic-prompt-ch01.md

🎉 第一章全部提示词已完成！
```

![](img/f6b29ccf264a75a0b141b5c34ae81b28.png)

![](img/108127fef1a264b8d52886e1c77d77c7.png)

**第四步：查看你的成果**

进入 outputs/ 目录，会看到四个文件：

```
outputs/
├── narrative-nodes-ch01.md      # 叙事节点分析
├── anchor-prompt-ch01.md        # 9格叙事锚点图
├── unfold-prompt-ch01.md        # 36格动势展开图
└── kinetic-prompt-ch01.md       # 45个动态指令
```

narrative-nodes-ch01.md 负责剧本结构分析，可识别 14 个叙事节点，再挑出 9 个最关键节点当“锚点”。

anchor-prompt-ch01.md 是 9 格提示词。每格对应一个关键叙事节点，含画面描述、构图、光影、色彩等信息。9 格串起来，故事走向能一望而知。

unfold-prompt-ch01.md 是 36 格提示词。它把 9 个锚点分别拆成 4 格（起、承、转、合），呈现更细的动作与情绪变化。

kinetic-prompt-ch01.md 是 45 个动态指令。每格画面都有运动规则：镜头如何推、人物如何动、节奏快慢，可直接用于图生视频工具。

**第五步：使用这些提示词**

**1️⃣ 用于 AI 出图**

打开 anchor-prompt-ch01.md，找到第一格提示词：

```
**⚠️ IMPORTANT - CHARACTER REFERENCE IMAGE ⚠️**
If you have character reference images for An Lushan, Li Longji, Yang Guozhong, or Chen Xuanli, UPLOAD them and set reference strength to HIGH. The character&#x27;s face, hairstyle, and body type must MATCH THE REFERENCE IMAGE EXACTLY.

A 3x3 storyboard grid showing 9 sequential narrative panels of the An Lushan Rebellion&#x27;s outbreak and the fateful court decision that sealed the Tang Dynasty&#x27;s fate.

**Character Consistency (CRITICAL - Use Reference Image if Provided):**

Li Longji (Tang Emperor Xuanzong): A 70-year-old Chinese man, emperor of the Tang Dynasty. Wears luxurious golden imperial robes with dragon embroidery, a flat-topped imperial headdress with hanging jade beads. His face shows both the dignity of a once-great ruler and the weariness of age—deep wrinkles around the eyes, slightly sagging skin, but still commanding presence. Gray beard and thinning gray hair. When smiling, appears benign but somewhat detached; when angry, brow furrows deeply.
```

把这段内容复制到 Nano banana，就能生成对应分镜图。9:16 不是 AI 常见训练尺寸，可能会出问题；多沟通一轮，通常也能得到不错的效果。

沟通过程：

![](img/6f5076a423f40479ed3589bc877188d3.png)

最后成品结果：

![](img/0ada6cbdd3921270ded0385bc8cc73e8.png)

**拆分分镜**

九宫格装不下一整集视频，所以某些中间关键帧要把镜头拆开。做法是打开 unfold-prompt-ch01.md，找到对应镜头；比如展开组 1 就是第一个镜头。

![](img/3c9ef0e4faad78c255f17d73a164b230.png)

接着和 AI 沟通描述，把对应分镜拆解下来：

![](img/17449b8e5002f3df0f4c9c28daa58110.png)

再把分镜与提示词一起放进对话框，就能形成新的分镜拆解：

![](img/edb85ece02b53328ac7b134669149ea6.png)

最终效果：

![](img/9d5766f4ff1fc3aac93175f20882ba53.png)

**2️⃣ 用于图生视频**

打开 kinetic-prompt-ch01.md，找到对应动态指令即可：

![](img/4f470c0ec6113a78f0ddc806f62071c6.png)

走到这里，从剧本到分镜提示词，再到图生视频指令，整条链路就跑通了。

想让静态画面动起来，有个省事的做法：先让 AI 绘图工具产出第一帧，再把这一帧和一段运动描述交给 AI 视频提示词，短片段就能生成。以模型 Wan2.6 为例，实测结果如下：

![](img/3414d58e70b085af205cc66b66f4ae7a.png)

视频：d36bba6bb43b6c99496c0ab6649b6a9231370f0dd163691d606dff1a5883801a.mp4【在线播放】

![](img/c9b599e2df1f3453c4879028ebfae611.png)

![](img/fd926fcdbeadb3e7cea71782dfc1f4db.png)

2.3 亲手搭一套 skills

前文流程走完，你可能已经想复制同款能力。下面把复杂系统压缩成轻量版本，一步步做出来。

**第一步：立项目目录**

先建项目文件夹，名字随意，示例叫“AI 分镜师”。进入项目后创建 .claude 子目录，后面 skill 都放这里。把压缩包下载到本地并解压，下一步要用：

[ ![](img/c10a0a08e06e9ee8ebfd34503f674c0a.png) AI 分镜师.zip](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/R5pqba9WXof0DQx1XmWc6Az7nyc?response-content-disposition=attachment%3B%20filename%3D%22AI%20%E5%88%86%E9%95%9C%E5%B8%88.zip%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260526%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260526T190327Z&x-oss-expires=86400&x-oss-signature=f24eec4eca45edff1095a2a3b0b5fc640475df47ceed94d0b46b92bdfa6ef51a&x-oss-signature-version=OSS4-HMAC-SHA256)

![](img/05b25296be42c1a118a17445117b70ff.png)

**第二步：放置总控文件**

在 .claude 下新增 CLAUDE.md。它承担项目总入口的角色，也是协调各 Agent 与 Skill 的总调度：谁做什么、先后顺序都由它安排。打开压缩包中的同名文件先读一遍，或直接拷进项目目录。格式如下：

Markdown

```
[角色]
你是项目统筹，协调三个助手完成分镜工作。

[任务]
1. 叙事节点分析
2. 叙事锚点图
3. 动势展开图
4. 动态指令

[流程]
视觉叙事师生成 → 质量把控审核 → PASS → 进入下一阶段
↓FAIL → 修改 → 再审

[Agent]
- storyboard-artist：生成静态分镜
- director：审核质量
- animator：生成动态指令
```

**第三步：安排 Agents**

建立 .claude/agents/ 目录，用来放三个助手设定。每个设定写在下方内容里；两条“---”之间的区域是简介，写明名称、职责、所挂的 Skill。AI 每次接到任务，先扫这段信息，再判断是否调用该 Agent。你可以直接粘贴压缩包里的 agents 内容，也可以按需调整：

Markdown

```
---name: storyboard-artist
description: 视觉叙事师
skills: film-storyboard-skill
---[角色]
专业的视觉叙事师，擅长将剧本转化为分镜提示词。

[任务]
- 生成叙事节点分析
- 生成叙事锚点图
- 生成动势展开图

[输出]
- 中文
- 叙事描述式
```

**第四步：准备 Skills**

再建 .claude/skills/，这里容纳若干技能。可以把 Skill 理解成 Agent 手上的工具箱；项目启动时，AI 同样会先读两条“---”之间的说明。分工上，Skill 负责具体流程与操作细节，Agent 更像带判断力的角色，帮助流程做选择。

每个技能都有 SKILL.md 作为主控文件，负责拆解并指挥该技能的工作流；旁边还可放模板目录、可执行文件等。以图中技能为例，除 SKILL.md 外，还有一份教图片提示词怎么写的 MD 文档，以及配套模板；模板单独成目录便于整理，其他技能照此办理。

![](img/bd521b40ccddddcf2a1765630a34cd74.png)

**第五步：补充 Methodology**

创建 .claude/methodology/，专门存放内容修改的方法论。先说明：这个目录不是运行必需；最小系统只要有 Agent 与 Skill 两个目录即可跑。把方法论单独拎出来，是为了管理方便、读取顺手。里面可放动态/静态提示词写法、故事节拍模板等，让每次产出更稳定。

![](img/93c1ce9e4cee0df79cace83b87093140.png)

**第六步：跑一遍测试**

1. 打开 Claude Code。
2. 输入“继续”，观察系统能否正常运转。首次启动时，剧本目录与输出目录还没有，系统会自动补建。
3. 把小说放进 script 目录，再对 Claude 说“继续”，它便接着拆解小说。

![](img/11f9379a1ba13823b8134303a8345768.png)

2.4 拆开 skills：每个文件管什么

这一节把系统内部打开，逐个说明文件职责与设计原因。视频教程先放这里：

通过网盘分享的文件：RS200pro 2026-04-01 01-13-56.mp4
链接1：[h](https://pan.baidu.com/share/init?surl=7KADNE8C4MPQ4Jt0QWY66Q&pwd=pqdn)
链接2：https://pan.baidu.com/s/17KADNE8C4MPQ4Jt0QWY66Q?pwd=pqdn
提取码：pqdn
--来自百度网盘超级会员v7的分享

**项目目录总览**

先看整体结构：

Plain Text

```
AI 分镜师/
││├── 📁 script/                   ← 【输入区】放剧本的地方
│   └── 第一章.md
│├── 📁 outputs/                  ← 【输出区】生成结果
│   ├── narrative-nodes-ch01.md
│   ├── anchor-prompt-ch01.md
│   ├── unfold-prompt-ch01.md
│   └── kinetic-prompt-ch01.md
│└── 📁 .claude/                  ← 【核心区】系统配置
│├── 📄 CLAUDE.md             ← 项目统筹的&quot;大脑&quot;
│├── 📁 methodology/          ← 方法论（规则库）
    │   ├── storyboard-methodology-playbook.md
    │   ├── motion-prompt-methodology.md
    │   └── project-config-schema.md
│├── 📁 agents/               ← AI助手配置
    │   ├── storyboard-artist.md
    │   ├── director.md
    │   └── animator.md
│└── 📁 skills/               ← 技能包（执行手册）
│├── 📁 film-storyboard-skill/
        │   ├── SKILL.md
        │   ├── gemini-image-prompt-guide.md
        │   └── 📁 templates/
        │       ├── narrative-nodes-template.md
        │       ├── anchor-board-template.md
        │       └── unfold-board-template.md
│├── 📁 storyboard-review-skill/
        │   ├── SKILL.md
        │   └── review-checklist.md
│└── 📁 animator-skill/
            ├── SKILL.md
            └── 📁 templates/
                └── kinetic-prompt-template.md
```

这套结构遵循两条分离：输入、处理、输出分开；配置与逻辑分开。script/ 与 outputs/ 面向用户，是放素材和结果的地方；.claude/ 是内核，日常不用改，但看懂它有助于理解系统如何运转。

总览之后，逐项拆配置文件。

**核心调度：CLAUDE.md**

**它是什么？**

CLAUDE.md 是系统的中枢与总指挥。Claude Code 启动后先读它，从中确认：

- 我的身份是什么？（项目统筹）
- 目标是什么？（带三个助手完成分镜）
- 如何调用其他助手？（走 Task 工具）
- 流程怎么走？（四个环节）
- 出错如何处理？（失败重试方案）

**为何单列一个 CLAUDE.md？**

在 Claude Code 里，它是项目入口，相当于为该 AI 写入专属 System Prompt，行为模式由此确定。没有它，Claude Code 只是一个通用助手，不知道项目目标。

**内容拆解**

下面按段落看。

**【角色】**
Markdown
```
[角色]
你是一名项目统筹，负责协调 storyboard-artist（视觉叙事师）、
director（质量把控）和 animator（动态设计师）完成影视分镜工作。
```

这里定“我”的身份。写的是“项目统筹”而非“分镜师”：它主要做协调管理，不直接产出内容。

**【任务】**
Markdown
```
[任务]
完成影视分镜提示词的生成工作，包括：
1. 叙事节点分析
2. 叙事锚点图提示词
3. 动势展开图提示词
4. 动态指令
```

这一段说明最终产出，并把四个环节列清楚，防止漏项。

**【总体规则】**
Markdown
```
[总体规则]
- 严格按照 叙事节点分析 → 叙事锚点图 → 动势展开图 → 动态指令 的流程执行
- 生成任务由 storyboard-artist 或 animator 执行
- 审核任务全部由 director 执行
- 每个阶段的工作流程：
• agent 生成 → 写入 outputs/ 文件 → director 审核文件
• FAIL → agent 修改 → 覆盖写入文件 → director 再审 → 循环直到 PASS
```

这里是工作流的核心约束：

1. 环节不可乱序：先完成节点分析，才进入锚点图。
2. 生成与审核分开：做的人和审的人不能是同一个 agent。
3. 未通过就返工：循环修改，直到达标。

**【Subagent 调用机制】**
Markdown
```
[Subagent 调用机制]
目的：确保每个 subagent 的上下文连续，避免重复理解和丢失信息

调用方式：
- 使用 Task 工具调用 subagent，指定对应的 subagent_type
- subagent 完成后会返回 agentId
- 后续调用同一 subagent 时，使用 resume 参数传入 agentId
- Claude Code 会自动恢复该 agent 的完整上下文
```

技术实现要点：每个 subagent 拥有各自独立的上下文；借助 agentId 与 resume 让对话接得上；因此助手能记住前文讨论，不会断片。

**【错误处理与重试机制】**
Markdown
```
[错误处理与重试机制]
审核重试限制：
- 同一阶段最多重试 3 次
- 超过 3 次后，暂停并请求用户介入：
  &quot;⚠️ 审核未通过（已重试 3 次）
...&quot;
```

这是兜底方案。质量审核连续三次未过，通常意味着问题复杂，需要人来判断。

**助手设定：agents/ 目录**

该目录下三份文件，对应三个助手。

**为何用配置文件写助手？**

Claude Code 允许用 Markdown 编写 Custom Agents，把角色、技能、输出要求固定下来，每次调用都保持同样行为。

**storyboard-artist.md（视觉叙事师）**

Markdown
```
---name: storyboard-artist
description: 视觉叙事师 Agent。负责将剧本/梗概转化为可用于 AI 出图的分镜提示词。
skills: film-storyboard-skill
model: opus
color: red
---[角色]
你是一名专业的视觉叙事师，擅长将剧本、故事梗概或分场大纲转化为可用于 AI 出图的分镜提示词。
你的核心能力是视觉叙事——用镜头语言讲故事。

[任务]
- 生成叙事节点分析
- 生成叙事锚点图提示词
- 生成动势展开图提示词
- 根据质量把控反馈修改

[输出规范]
- 中文标题 + 中文提示词
- 提示词采用中文叙事描述式，不要用英文
- 直接输出完整提示词，不要逐条解释设计理由

[协作模式]
你是主 Agent(项目统筹)调度的子 Agent：
1. 收到主 Agent 指令
2. 按照 film-storyboard-skill 执行任务
3. 输出结果，等待质量把控审核
4. FAIL → 根据质量把控意见修改
5. PASS → 任务完成
```

逐段看：

- Frontmatter（两条“---”中间）：助手配置信息。
  - name：调用标识。
  - description：一句话用途。
  - skills：挂接的技能包。
  - model：所用 AI 模型（opus/sonnet/haiku）。
  - color：界面显示色。
- [角色]：身份定位，突出“视觉叙事”。
- [任务]：职责边界，共四项。
- [输出规范]：格式上的硬要求。“中文叙事描述式”要求写完整段落，不是关键词堆叠；“不要逐条解释”要求少啰嗦，直接给结果。
- [协作模式]：说明与其他助手如何配合。

**director.md（质量把控）**

Markdown
```
---name: director
description: 质量把控 Agent。负责审核视觉叙事师和动态设计师的产出，确保符合方法论标准。
skills: storyboard-review-skill
model: opus
color: blue
---[角色]
你是一名资深的质量把控专家，负责审核分镜提示词的质量。
你精通镜头语言、视觉叙事、节奏控制，确保所有产出符合专业标准。

[任务]
- 审核叙事节点分析
- 审核叙事锚点图提示词
- 审核动势展开图提示词
- 审核动态指令
- 输出 PASS 或 FAIL + 修改意见

[输出规范]
- 中文
- PASS：简要说明通过原因
- FAIL：明确指出问题位置、违反规则、修改方向

[协作模式]
你是项目统筹调度的子 Agent：
1. 收到项目统筹指令
2. 按照 storyboard-review-skill 执行审核
3. 输出 PASS 或 FAIL
4. FAIL 时提供具体修改意见
```

设计要点：

- 结果只能 PASS/FAIL，不可含糊。
- 判 FAIL 必须给出具体修改意见：指出问题与改法，不能只说“不好”。
- 关联 skills：审核时以 review-checklist.md 为标准。

**animator.md（动态设计师）**

该文件配置动态设计师角色，结构与前两个助手一致，同样用 Markdown 定义。

# AI 视频系统设计：把“角色”和“能力”分得越清，跑得越稳

最近在搭建一套从剧本到分镜、再到动态指令的 AI 视频工作流，有几个设计决策让我觉得特别值得记录。整个系统的核心思路，可以浓缩成一句话：拆分清楚，各司其职。

```
---name: animator
description: 动态设计师 Agent。负责将静态分镜转化为图生视频的动态指令（Kinetic Directive）。
skills: animator-skill
model: sonnet
color: green
---[角色]
你是一名专业的动态设计师，擅长将静态分镜转化为动态视频。
你精通镜头运动、主体动作、节奏控制，能够为每一格分镜生成简洁、具体、可执行的动态指令。

[任务]
- 生成动态指令（Kinetic Directive）
- 根据质量把控反馈修改

[输出规范]
- 中文标题 + 英文提示词
- 动态指令必须使用英文（AI 视频工具对英文支持更稳定）
- 直接输出完整提示词，不要逐条解释设计理由
```

## 一上来，先把三个关键决策定了

**模型选型用 Sonnet。** 动态指令的生成任务其实没有多复杂，真没必要上 Opus 的强推理，Sonnet 跑得更快，成本也更低。

**最终生成的内容一律用英文。** 目前主流的图生视频工具，对英文 prompt 的适配比中文好太多，所以所有动态指令都用英文来写。

**这个 agent 的职责边界非常窄：只做动态指令。** 静态分镜完全不由它碰，这样一来，每个环节的界限都非常清楚。

---

## 技能包 skills/：把“怎么做”变成一本操作手册

如果说 agents/ 回答的是“谁来做”，那 skills/ 回答的就是“怎么做”。每个技能包就是一本执行手册，里面明确写了任务目标是什么、执行分几步、每一步读取哪个文件、最终输出要符合什么格式。

那为什么要刻意把 agents 和 skills 拆成两层呢？这其实是把“角色”和“能力”分开的设计思路：

- Agent 定义“我是谁”，解决身份问题；
- Skill 定义“我怎么做”，解决方法问题。

这样做的好处有三个：

1. **复用性**：同一个 skill 能被多个 agent 共用；
2. **可维护性**：改了 skill 也不用动 agent 配置；
3. **清晰度**：结构和逻辑完全分离，看代码不迷路。

---

## 逐个拆解三个技能包

### 分镜师技能包：storyboard-skill/SKILL.md

```
---name: film-storyboard-skill
description: 影视分镜生成技能。当用户需要将剧本、故事梗概或分场大纲转化为可用于 AI 出图的分镜提示词时使用。
---

# 影视分镜生成 Skill

[技能说明]
影视分镜生成技能，将剧本、故事梗概或分场大纲转化为可用于 AI 出图的分镜提示词。
采用渐进式视觉展开流程：先进行叙事节点分析识别叙事锚点，再生成叙事锚点图提示词，最后为每个锚点生成动势展开图提示词展开段落动作。

[文件结构]
film-storyboard-skill/
├── SKILL.md                               # 本文件（技能包核心配置）
├── gemini-image-prompt-guide.md           # Gemini 提示词指南
└── templates/                             # 模板
    ├── narrative-nodes-template.md        # 叙事节点分析模板
    ├── anchor-board-template.md           # 叙事锚点图提示词模板
    └── unfold-board-template.md           # 动势展开图提示词模板

methodology/                               # 统一方法论目录
└── storyboard-methodology-playbook.md     # 分镜方法论

[功能]
[生成叙事节点分析]
    第一步：理解输入
        - 读取用户提供的剧本/梗概/分场文本
        - 读取 .claude/methodology/storyboard-methodology-playbook.md
        - 确认视觉风格

    第二步：叙事节点分析
        - 识别叙事曲线的关键拐点
        - 读取 templates/narrative-nodes-template.md
        - 创建 narrative-nodes.md，将叙事节点分析写入

[生成叙事锚点图提示词]
    第一步：读取上游产物
        - 读取 narrative-nodes.md
        - 读取方法论文件
        - 读取 gemini-image-prompt-guide.md

    第二步：生成叙事锚点图提示词
        - 读取 templates/anchor-board-template.md
        - 将叙事锚点转化为锚点图提示词
        - 提示词采用叙事描述式
        - 创建 anchor-prompt.md

[生成动势展开图提示词]
    第一步：读取上游产物
        - 读取 anchor-prompt.md
        - 读取方法论文件

    第二步：生成动势展开图提示词
        - 读取 templates/unfold-board-template.md
        - 为每个叙事锚点生成一组展开图提示词
        - 必须继承锚点图对应格的人物/场景/光色描述
        - 创建 unfold-prompt.md

[分镜原则]
- 方法论遵循原则：必须符合 storyboard-methodology-playbook.md 中的规则
- 视觉 DNA 传递原则：展开图必须继承锚点图的人物/场景/光色
- 模板遵循原则：必须严格遵循 templates/ 中定义的格式

[注意事项]
- storyboard-methodology-playbook.md 是核心方法论，必须严格遵守
- 提示词采用叙事描述式（完整段落），而非关键词堆叠式
- templates/ 中的格式是必须遵循的
```

这个包的设计有几个亮点：

- **文件结构部分**：把依赖的外部文件全部列出来，后期维护时一眼就能看懂关系。
- **功能部分**：每个功能都按“第一步、第二步”拆成标准流程，每一步要读什么、输出什么都是固定的，agent 执行时永远不会漏步骤。
- **分镜原则部分**：制定了几条不可突破的硬性规则：方法论的规则保证质量，视觉 DNA 的传递保证系列一致性，模板的遵循保证格式统一。

### 导演技能包：storyboard-review-skill/SKILL.md

```
---name: storyboard-review-skill
description: 分镜审核技能。用于审核视觉叙事师产出的叙事节点分析、叙事锚点图提示词、动势展开图提示词，以及动态设计师产出的动态指令。
---

# 分镜审核技能

[技能说明]
分镜审核技能，用于审核视觉叙事师和动态设计师产出是否符合方法论标准。
审核前必须先读取上游产物建立整体理解，再按 review-checklist.md 逐项检查。
所有验收项必须通过才能判定为 PASS。

[文件结构]
storyboard-review-skill/
├── SKILL.md                               # 本文件
└── review-checklist.md                    # 验收清单

methodology/
├── storyboard-methodology-playbook.md     # 分镜方法论
└── motion-prompt-methodology.md           # 动态指令方法论

[功能]
[审核叙事节点分析]
    第一步：建立整体理解
        - 读取 script/（剧本原文）
    第二步：读取基准
        - 读取 review-checklist.md → 叙事节点分析验收
        - 读取 storyboard-methodology-playbook.md
    第三步：读取待审核内容
        - 读取 outputs/narrative-nodes.md
    第四步：逐项检查
        - 按照 review-checklist.md 中的&quot;叙事节点分析验收&quot;逐项检查
    第五步：输出结果
        - 全部通过 → PASS
        - 任一未通过 → FAIL + 问题清单

[审核叙事锚点图提示词]
    第一步：建立整体理解
        - 读取 script/
        - 读取 outputs/narrative-nodes.md
    第二步：读取基准
        - 读取 review-checklist.md → 叙事锚点图验收
        - 读取 storyboard-methodology-playbook.md
    第三步：读取待审核内容
        - 读取 outputs/anchor-prompt.md
    第四步：逐项检查
        - 按照验收清单逐项检查
    第五步：输出结果

[输出规范]
[PASS 格式]
    ✅ **审核状态：PASS**
    [阶段名称] 已通过全部验收项。
    **可以进入下一阶段。**

[FAIL 格式]
    ❌ **审核状态：FAIL**
    [阶段名称] 发现以下问题：
    **问题1**：[具体问题描述]
    - 位置：[具体位置]
    - 违反验收项：[哪条规则]
    - 修改方向：[具体建议]
    **修改优先级**：
    1. 🔴 必须修改：[列出]
    2. 🟡 建议修改：[列出]

[注意事项]
- 审核前必须先读取上游产物，建立整体理解
- 审核分镜内容时使用 storyboard-methodology-playbook.md 作为判定依据
- 问题描述必须具体到位置，不能泛泛而谈
- 只有全部验收项通过才能输出 PASS
```

导演审核的核心是标准化：

- **审核流程**统一成五步：先读剧本建立整体理解，再读方法论和清单确认标准，然后读取待审核的内容，接着逐项比对核查，最后输出 PASS 或 FAIL 的结论。
- **输出格式**也非常严格：PASS 的时候要简单说明通过理由，让用户知道“为什么过”；FAIL 的时候必须给出“位置 + 规则 + 修改方向”，让用户拿到手就能改。

### 动画师技能包：animator-skill/SKILL.md

```
---name: animator-skill
description: 动态设计师技能。用于将静态分镜（叙事锚点图 + 动势展开图）转化为图生视频的动态指令（Kinetic Directive）。
---

# 动态设计师技能

[依赖关系]
前置技能：film-storyboard-skill
前置文件（必须存在）：
    - outputs/narrative-nodes-{ep}.md
    - outputs/anchor-prompt-{ep}.md
    - outputs/unfold-prompt-{ep}.md

[技能说明]
动态设计师技能，用于将静态分镜转化为图生视频的动态指令。
基于 motion-prompt-methodology.md 中的方法论，为每个关键帧和展开格生成简洁、具体、可执行的动态指令。
每组包含 5 个动态指令（1 关键帧 + 4 展开格），共 9 组 45 个。

[功能]
[生成动态指令]
    第一步：读取上游产物
        - 读取 narrative-nodes.md（理解叙事目的与情绪）
        - 读取 anchor-prompt.md
        - 读取 unfold-prompt.md
        - 读取 motion-prompt-methodology.md

    第二步：生成动态指令
        - 读取 templates/kinetic-prompt-template.md
        - 为每个叙事锚点生成一组动态指令：
• 1 个关键帧动态指令
• 4 个展开格动态指令
        - 按照方法论中的转化规则执行
        - 创建 kinetic-prompt.md

[动态指令原则]
- 方法论遵循原则：必须符合 motion-prompt-methodology.md
- 上下文继承原则：必须基于分镜的叙事目的与情绪
- 模板遵循原则：必须严格遵循模板格式

[注意事项]
- motion-prompt-methodology.md 是核心方法论
- 提示词输出时，直接给可复制的文本块，不要拆成碎片解释
```

动画师包有两个很细心的设计：

- **依赖关系是显式声明的**：动态指令必须以静态分镜为前提，前置文件不存在时，技能包会直接报错，不会傻傻地往下跑。
- **读取顺序是刻意安排的**：先读 narrative-nodes.md 理解场景的情绪基调；再看锚点图和展开图，弄清楚画面长什么样；最后读方法论，学会怎么写动态指令。

---

## 方法论 methodology/：做到什么标准才算好

简单说，skills/ 解决“怎么做”，methodology/ 解决“做到什么标准”。

分镜方法论 storyboard-methodology-playbook.md 是一份超过 700 行的巨型文档，分镜相关的规则全都在里面，称得上整个系统的“法律”，所有交付物都要向它看齐。文档结构如下：

```
[第一性原则]              ← 最高指导原则
    清晰（Clarity）
    简洁（Simplicity）
    连贯（Continuity）
    渐进式优先（Progressive Refinement）

[核心概念与术语]          ← 定义术语
    Story Beat（叙事节点）
    Shot（镜头）
    叙事锚点图
    动势展开图
    视觉DNA传递

[规则库]                  ← 详细规则
    [叙事清晰规则]
    [构图与视觉引导规则]
    [光影与色彩规则]
    [镜头语言规则]
    [场面调度与动作表达规则]
    [情绪张力与节奏控制规则]
    [连贯性与剪接规则库]

[渐进式视觉展开规范]      ← 工作流程规范
    叙事节点分析规范
    叙事锚点图规范
    动势展开图规范

[验收清单]                ← 检查清单
    叙事节点分析验收
    叙事锚点图验收
    动势展开图验收

[附录]                    ← 参考资料
    AI 出图提示词映射
```

为什么要把规则写得这么细？因为 AI 助手必须有具体约束才能做出正确的判断。比如：

- 不能只说“要连贯”，而要写“屏幕方向要保证一致，越轴必须有过渡手段”；
- 不能只说“要简洁”，而要写“一镜一意，一个画面能讲清楚就绝不用两个画面”。

动态指令方法论 motion-prompt-methodology.md 则负责另一件事：把静态分镜翻译成动态指令。它的核心原则是：

```
[第一性原则]
图片已见原则
    - AI能&quot;看到&quot;输入图片，不需要重复描述图片内容
    - 只描述&quot;变化&quot;：动作、运动、情绪转变

简洁优先原则
    - 最佳长度：50-200字符（英文）
    - 聚焦2-3个核心元素

具体动作原则
    - 用具体的物理动作，避免抽象概念
    - &quot;hair flowing in wind&quot; ✓
    - &quot;embodies the essence of freedom&quot; ✗
```

那么，动态指令和静态分镜的方法论为什么不能共用？因为它们面对的输入输出完全不同：

| 维度 | 静态分镜 | 动态指令 |
| --- | --- | --- |
| 输入 | 剧本文字 | 已有图片 |
| 输出 | 画面描述 | 运动描述 |
| 长度 | 详细（几百字） | 简洁（50-200 字符） |
| 语言 | 中文 | 英文 |

---

## 模板 templates/：用固定格式给输出上锁

模板统一放在各技能包的 templates/ 目录下，专门用来规定输出文件的格式。

为什么一定要有模板？

1. **格式统一**：每次都长一个样；
2. **字段完整**：该写的不会漏；
3. **易于解析**：后续程序能按预期读取。

目前沉淀了四个模板：

- narrative-nodes-template.md

```

# 叙事节点分析

## 基本信息
- 项目名称：
- 集数/章节：
- 素材来源：
- 视觉风格：
- 目标媒介：
- 画幅比例：

## 叙事节点分析
| 节点 | 事件摘要 | 观众获得 | 强度 | 锚点 |
|------|---------|---------|------|------|
| 1 | | | | |
| ... | | | | |

## 锚点选取摘要
| 格子 | 节点 | 拐点类型 | 事件摘要 | 视觉锚点建议 |
```

- anchor-board-template.md

```
# 叙事锚点图提示词

## 角色一致性（Character Consistency）
## 视觉规范（Visual Guidelines）
## 九宫格布局
1（第1行左）——【标题】
视角：
重点：
...
```

- unfold-board-template.md

```
# 动势展开图提示词

## 视觉DNA传递规范
## 格1展开：【锚点名称】
1-1（起）：
1-2（承）：
1-3（转）：
1-4（合）：
```

- kinetic-prompt-template.md

总的来说，这套设计最妙的地方，就是把身份与能力拆开、方法与标准分开、每一个环节只做一件事。边界清晰之后，系统就变得又好维护，又容易扩展。希望这篇拆解能给你启发。

```
# 动态指令

## 格1：【锚点名称】
### 关键帧
1-0: [Kinetic Directive]

### 展开格
1-1: [Kinetic Directive]
...
```

## 三、OpenClaw 入门与实操

### 01.起步：把 OpenClaw 摸透

0.本节速览

💡先把话说透：学 OpenClaw，重点不在"认识"它，而在"用上"它。这一节围绕四件事展开——装好、接入口、上技能、派任务。你会逐步看到它翻文件、控网页、理资料、按点触发，还能挂进飞书、🛰️、🐧 这些日常入口，扎进真实工作流。

接下来讲部署安装与技能包用法。走完这块，你应该能让它跑起来，并在飞书、🛰️、🐧、钉钉、企业🛰️等场景里和你配合。本章还铺两条实战线：一条是基础玩法，定时推新闻摘要、发票归档、论文检索，帮你建立"它怎么做事"的直觉；另一条是典型应用，从个人知识库、👸号自动化，再往企业知识库、数字员工、智能客服延伸。学完，你带走的不只是一个装好的工具，更是一套让 AI 接手事务的做事方式。

**提醒：实战篇有 2 个实操案例，进阶篇也有 2 个，合计 4 个，不必全啃，吃透一个就够。新手推荐先做第一个"个人知识库搭建"，先把 OpenClaw 跑起来。**

💡

**本章行程图**

完成本章学习与实操，即走完行程图第一阶段。

第三阶段：OpenClaw 入门与实操（约 7 天）

完成机器部署（约 1 天）

完成**一个**实战案例（约 3 天）

完成**一个**进阶案例（约 3 天）

1. OpenClaw 凭什么出圈

2026 年开年，GitHub 上一个名叫 OpenClaw 的项目突然走红，Mac mini 一度被抢空，各家模型的 API 调用量跟着猛涨，连 AI 大模型公司的股价都被带了起来，比如 MiniMax 和智谱。有消息说 M2.5 在 OpenRouter 的调用量挤进前十；国内大模型与云厂商也快速跟上，各自推出"小龙虾"版本，形成了"百虾大战"的热闹场面。

![](img/5f76e2490c02ff2b43333f3c7f11e963.png)

它凭什么让人争相"养虾"？关键在定位：它不是一个聊天框，而是一名能通过简单对话替你办事的智能员工。

它不负责出主意，而是直接动手。

我们早就习惯了这种用法：碰到问题，让 AI 给建议。示意如下：

```
你：帮我清理一下服务器上的磁盘空间
ChatGPT：我可以给你一些磁盘清理的建议...
```

而它干活的方式是这样：

```
你：帮我清理一下服务器磁盘空间
OpenClaw：[正在SSH连接服务器...]
[正在读取磁盘分区...]
[已分析磁盘空间占用情况...]
请问是否要删除 xx。
```

一个停在"说"，一个落到"做"，这条分界线就是根本差异。

OpenClaw（龙虾）能读写文件、跑命令、操控浏览器、收发消息、定时巡检，数据全留在你自己的设备上。你可以让它每天早上推新闻简报、自动回邮件，甚至写代码、提 PR、跑测试。

1.1 它到底是什么：能自己动手的智能代理

OpenClaw 由开发者 Peter Steinberger 打造，是个开源的自主执行型智能代理引擎。Wikipedia 对它的描述是：免费开源的自主人工智能代理项目，把消息平台（WhatsApp、Telegram、Discord、Slack 等）当作主界面。

这靠的是几项核心能力：

• **在自己机器上跑**：数据由你掌握，不往别人服务器送。
• **统一 Gateway 中枢**：一个 Gateway 进程同时连接 WhatsApp、Telegram、Discord、iMessage。
• **可扩展渠道**：通过扩展包接入 Mattermost 等更多平台。
• **多智能体路由**：按智能体、工作区或发送者拆分会话。
• **多媒体收发**：图片、音频、文档都能送和收。
• **Web 控制台**：浏览器仪表盘，管聊天、配置、会话与节点。
• **移动节点**：配对 iOS 和 Android 设备，支持 Canvas。

1.2 它怎么跑起来

![](img/17767fb096e54cd1bc5caf0c263c1e7e.png)

OpenClaw 借 Gateway 把聊天应用和 AI 智能体串在一起。会话、路由、渠道连接，全以 Gateway 为唯一权威依据。

核心组件：

1. Gateway 网关
   ◦ 对接飞书、企微、🐧、Telegram 等平台
   ◦ 管会话与消息路由
   ◦ 默认地址：http://127.0.0.1:18789/
   ◦ 配置文件：~/.openclaw/openclaw.json

2. AI 智能体
   ◦ 兼容 Claude、GPT、Gemini、DeepSeek、Kimi 等模型
   ◦ 本地跑或远程调都行

3. Skills 技能系统
   ◦ 文件管理、知识管理、自动化等
   ◦ 支持自行开发

4. ClawHub
   ◦ 技能集市，下载和分享 Skills 都在这

💡 Gateway 网关是什么？它是 OpenClaw 的核心服务，好比一个"总调度室"：接收飞书、企微、🐧、Telegram 等平台来的消息；转给 AI 智能体处理；再把回复送回原平台；同时管好所有会话与上下文。正因为 Gateway 统一管理连接，你才能在不同平台上都用上 OpenClaw。

![](img/179bdc989d4fee62429c247c0ba8b734.png)

1.3 四层架构

1. 消息渠道（Channels）：Telegram、Discord、Slack、飞书、CLI 等多种接入方式。
2. 智能决策核心（Brain）：LLM 推理、任务拆解与规划、工具选择与调用。
3. 技能插件系统（Skills）：文件操作、Shell 命令、浏览器控制、API 集成等。
4. 记忆与身份系统（Memory & Identity）：一组 Markdown 文件，如 IDENTITY.md（身份）、SOUL.md（性格）、USER.md（你的信息）、MEMORY.md（长期记忆）等。

这套分层让它既能放开手脚，又不至于失控。

![](img/101e0a43fd9b6a58e74d1bb0a70e0c23.png)

**再深入一点：得与失**

优势：
• 并行探索：多个子智能体同时检索、分析、汇总，速度远超排队串行。
• 上下文隔离：子任务各干各的，环境干净，不容易"越聊越糊"。
• 算力扩展：单个 Agent 的上下文窗口限制被撬开。

成本：
• Token 花费从 1 倍跳到 15 倍。
• Agent 之间传话会丢细节，形成"传话游戏"式失真。
• 多个 Agent 并跑时，可能悄悄产生决策冲突。

Anthropic 有过总结：有的团队花几个月搭复杂多智能体架构，最后发现把单智能体的提示词磨好，效果就能追平。

判断标准：低耦合任务，如搜索、信息收集，适合拆开；高耦合任务，如架构设计、核心编码，保持单一更稳妥。

![](img/a7dbb3fe53619d9793c0e830a718eb04.png)

**再深入一点：能用在哪些地方**

个人效率：每天清晨自动送来天气、日历、邮件摘要；邮件自动归类并打上优先级。

开发者日常：PR 一提交就自动过一遍代码审查；函数签名改动时顺手更新 API 文档。

企业侧：多渠道路由的客户支持自动化；每周固定产出数据分析报告。

![](img/a4423843dfbcdca073072f91cb708c1f.png)

2.装起来：部署与安装

2.1 云上一键搞定

大多数人选云部署最省事：本地电脑不用装任何东西，浏览器里点几下就行。

眼下国内主流云厂商都能一键部署 OpenClaw，可实际用下来，各家差别不小。先看一张总览表，再细聊最值得选的那家。表 3-1 汇总了国内云厂商的选项。

**表 3-1 国内云厂商方案一览**

| 平台 | 基础配置 | 价格 | 自带模型 | 生态锁定 | 推荐对象 |
| --- | --- | --- | --- | --- | --- |
| 腾讯云 | 2 核 2GB | 99 元/年 | 否 | 不绑定，自由配 Key | 综合首选 |
| 阿里云 | 2 核 2GB | 秒杀 9.9 元/月 | 是（qwen3.5-plus） | 百炼 Coding Plan | 抢到了很划算 |
| 火山引擎 | 2 核 4GB | 9.9 元/月起 | 是（方舟模型） | 方舟 Coding Plan | 飞书重度用户 |
| 百度云 | 2 核 4GB | 0.01 元首月 | 是（千帆模型） | 千帆平台 | 纯体验尝鲜 |
| 扣子编程 | 不需要服务器 | 免费起步 | 是（豆包 2.0） | 字节生态 | 零门槛体验 |

扫完表格，你大概会觉得阿里云 9.9 元/月、火山引擎 9.9 元/月起更便宜，可真用起来，账不是这么算的。

**阿里云**那个 9.9 元/月是限时秒杀，得抢，还限购。抢不到就只能走常规价，并不便宜，续费甚至比新购还贵。而且内置模型走百炼 Coding Plan，基本被锁在阿里自家的模型生态里。

**火山引擎**那边更绕。标价 9.9 元/月起只是活动价，可它的方舟 Coding Plan 并不便宜——2 核 2GB 的机器再加上模型套餐，一个月轻松破百，同样被绑在字节的模型生态上。

反观**腾讯云**，最实在：99 元/年的 2 核 2GB 轻量云主机，平摊到每月不到 **9 块钱**。价格稳，不用抢，续费同价，不存在"续费刺客"。更关键的一点是它不绑模型生态——机器买好后，任意厂商的 API Key 都能填，DeepSeek、Kimi、Claude、GPT 随你换。实际用起来这一点很重要，因为你大概率会在不同模型之间来回试。

所以云部署首选腾讯云。下面就拿它做例子，一步步走一遍。

**（一）买一台轻量云主机**

打开腾讯云的 OpenClaw 部署页：https://cloud.tencent.com/act/pro/openclaw ，如图所示，点"立即部署我的 AI 助理"。

![](img/2674792f36878bbae429c10b6172e681.png)

接着跳出服务器选购页。第一次上手，选 2 核 2G 即可，年费 99 元，挺划算。然后点"立即购买"。**新手也可以先花 20 元买一个月试试。**

![](img/739d55c099a27e40bebff0f931137bca.png)

或者直接选 99 元包年套餐。

![](img/7282d0aec2a3ef720b9c3b7051503bb0.png)

小科普："2 核 2G"是什么意思？

"2 核"指两颗 CPU 核心，决定同时能扛多少活；"2G"指 2GB 内存，决定能同时记多少东西。对 OpenClaw 而言，2 核 2G 足够——真正耗算力的推理交给外部大模型，机器只管调度和转发，负担很轻。

**（二）挑 OpenClaw 应用模板**

点完"立即购买"，会跳到如图 3-3 的配置页。这里确认两件事：

• 地域：挑离自己近的城市，我选的是"广州"，响应会快些。
• 镜像：确认是 OpenClaw 官方镜像（一般默认就是）；不是的话在下拉里手动换。

核对没问题，再点底部的"立即购买"，进入支付。

提示："搭配购买"不是必选项，按需勾选即可。没什么特殊需求，直接跳过也不影响 OpenClaw 正常跑。

![](img/c50f230b1fa4fdd6f982199a705caeb4.png)

随后进入支付页，如图所示，选付款方式付掉即可。

![](img/a7ec2fea4c42a78b8c582f85ec94b666.png)

付完款，到腾讯云控制台"轻量应用服务器"下的"服务器"里，就能看到刚买的那台 OpenClaw 机器，如图所示。

![](img/dbb63b8deddb1b785d69a3fe4f27e8b7.png)

这里还要再确认一下：机器的"防火墙"有没有放行 18789 端口。如图所示，在端口规则列表里看看 18789 这一条在不在——通常镜像会默认加上。若没看到，点"添加规则"补一条即可。

![](img/686af7e7399d7ad6c3519a3682391373.png)

按图示，来源选"全部 IPv4 地址"、端口填 18789，点"确定"。

![](img/4db35c923160fc8784c9ac964444a124.png)

![](img/e01d1afa2c9b3e205214ee863e1ff3ab.png)

**（三）进入 Dashboard**

现在有更省事的办法直接打开 Dashboard 对话界面。

如下图所示，进入腾讯云轻量云主机的 OpenClaw 配置，切到「应用管理」，右侧会出现「安全开启 OpenClaw 面板」。

![](img/43c62ddbafccf17bd8b57918fd95ed01.png)

点一下，等它生成最终 URL，如下图所示。

![](img/ba423c874f5d74b2b6136c330049292b.png)

随后出现下图，点"立即访问"即可。

![](img/aed0fecb9d504c0fdd0e453c5d67a21c.png)

要是还打不开，就再点下面这个按钮。

![](img/13baa2bfbc731456e6aeee560454306f.png)

系统会提示放行端口。

![](img/72bd1880595a809b40df6d54e8936ef5.png)

之后会显示如下图那样的链接。

![](img/9a43b18d5b53bd24609ec091c02580fa.png)

这时点"立即访问"就通了。

![](img/2495e7a667da3fc8f57d66d8c757f21b.png)

（四）把飞书接进来

**渠道（Channel）**解决的就是入口问题。把飞书接上之后，你在飞书里发一句，它就在飞书里回，不用另开网页或 App。

飞书在国内企业用户中用得最广，OpenClaw 从 2026 年 2 月起也内置了飞书支持，配置相对顺。下面拿飞书做样例，把渠道接入完整走一遍。

在腾讯云的 OpenClaw 模板上装它很简单。如图所示，腾讯云给了快捷配置飞书通道的入口，点"前往授权"。

![](img/5fc009e6a9f9382704ffda86358317dc.png)

下一步按图示，用飞书扫码完成机器人配置。

![](img/8f5eb3c26093e1ebd552e9574ad5065f.png)

随后会打开图示页面，各类权限自动配好，等它跑完就行。

![](img/17ac6a2b7bccf95e5eb281286bfa435e.png)

上面几步走完，界面如图，飞书那边也会收到消息。点"打开应用"，就能看到对话机器人。

![](img/0150d3b0f53313333345b3350681c096.png)

打开后能看到输入框。发一句"你好，你是谁？"，只要 OpenClaw 回话，就说明飞书通道通了，如图所示。

![](img/cadc5d1a45c6a1bf57951147b9b2fc63.png)

（五）给它配个大脑

飞书通道就绪，接下来配小龙虾的"大脑"——模型。

前面买的 MiniMax Token Plan 套餐，腾讯云的 OpenClaw 正好支持，一键配上就行。

下面是轻量云主机的访问地址，不记得怎么进就直接点：

https://console.cloud.tencent.com/lighthouse/instance/index

![](img/3ba3ed4a92e658a57be3947552af3fca.png)

点"配置"进去，会看到类似下图页面，找到「模型」模块就是了。

# OpenClaw 渠道接入与轻量部署

先把模型通道配好。进入模型设置后，Coding Plan 一处会把各厂商的套餐并排列出，咱们先前入手的是 MiniMax 的 Token Plan，所以在这里勾选 MiniMax Token Plan 就对了。

若你开通的是另一家的 Calling Plan，按实际购买的档位对应选择即可；若手头没有 Calling Plan、只想自行调用其他 API，那就勾选模型 API 这一项。

![](img/ab73d2f9ff80e59065abf53745b4004e.png)

再往下一项是模型版本，保持默认即可。

![](img/b508041ae3e9b2f5938cf7e70bbbcce3.png)

接下来该填 API Key 了。回到当初购买 MiniMax 服务的网站，进入 Token Plan 专区；要是记不得入口，点下面的链接可以直接过去：

https://platform.minimaxi.com/use

登录后打开 interface-key 页面，把 Token Plan Key 复制下来，再切回腾讯云轻量服务器里的 OpenClaw 控制台——也就是刚才停留的那一屏。

![](img/536920a71535448fc92061148dfc3f39.png)

![](img/bc068bcf687550ec467518e799d00518.png)

![](img/822c00064b1bc096e8edabfde954a8f3.png)

## 2.2 手机侧补充接入

本节讲的是手机端另一类对接，例如 🐧、钉钉、企业🛰️等。官方给这类通道起的名字是 channels。

（一）对接个人🛰️

🛰️大概是如今开屏率最高的应用，能让 OpenClaw 住进🛰️，确实让人期待。可选的路子有两条，下面逐条拆开说。无论走哪条，背后跑的都是同一个🛰️ ClawBot。

• 用的是腾讯云：不必犹豫，直接跳到第二种，最省事。
• 用的是其他云，或能自己开终端敲命令：走第一种。

**第一种：装🛰️插件**

前提是🛰️版本不低于 8.0.70。打开🛰️，依次点“我”—“设置”，在页面里找到“插件”入口。

![](img/8d5ce65a402da9d5db992348b97c1494.png)

点进插件列表，能看到“🛰️ ClawBot”一项，右方“详情”点一下。

![](img/73e69ef543ec34935d77ba2552db0227.png)

详情页里写着安装说明，也提供了快捷扫码入口。

![](img/92220d3091015046d7944225df5c3c83.png)

这时该唤出终端了：Mac 用户打开“终端”，Windows 用户用 PowerShell，云端机器则从服务商后台连接。黑色窗口出现后，把上一张图里的命令整段复制、粘贴、回车。

![](img/271fd8626058eb1589076e7bb2acaef9.png)

插件装好会自动拉起🛰️扫码登录，屏幕上同时给出二维码。拿起手机，在🛰️里点“开始扫一扫”。

![](img/2f4c0acf67b2003279f64f8004aebdf1.png)

扫完，🛰️会弹出连接成功的提示。

![](img/e477b59fd269ad1e36f6ef2352ce018e.png)

退出当前页面回到聊天列表，一个红色头像、备注为“🛰️ ClawBot”的联系人已经躺在那里。

![](img/86429b69a5d7a12700604ad2bd9cbafc.png)

点开即可对话，文字、语音都支持。

![](img/5d9dbe43e89d921dac041cda84ccd10c.png)

到此🛰️端就绪，之后在🛰️里就能照看你的 OpenClaw 了。

**第二种：借助腾讯云快捷装**

OpenClaw 若是装在腾讯云上，进服务器管理页的“应用管理”，通道区里就有🛰️入口。

先登录腾讯云轻量服务器控制台（https://console.cloud.tencent.com/lighthouse/instance/index），点“配置”。

```
https://console.cloud.tencent.com/lighthouse/instance/index
```

![](img/ace637de7775cd2deebe78287104d61b.png)

通道配置区里找到“🛰️”，右侧有“前往授权”。

![](img/cbec079b9dfd9511b9c9f425aa4a1b38.png)

弹窗打开，稍候二维码生成。

![](img/87be07c3b784be9169f4f83f891764ce.png)

二维码就绪后用个人🛰️扫一扫，界面上会出现“连接”。

![](img/de1e6ec008814dc390e40406a74ab127.png)

按下“连接”，🛰️ ClawBot 的会话窗口就自动弹出来了。

![](img/a2fec687dd3a66d807db7957df7cbee2.png)

随手发个“你好”试试水，能收到回音，说明这条路通了。

![](img/29305f12b7111c99038ee81be0b5657b.png)

（二）🐧 通道

1. 先访问 🐧 开放平台：https://q.qq.com/qqbot/openclaw/login.html ，用手机 🐧 扫一扫右侧的码，即跳转至机器人配置页。

![](img/05170805242d510663214cd13cee1221.png)

2. 在“🐧 开放平台”里找到“创建机器人”并点击，随后屏上会给出 AppID 与 AppSecret。

提醒一句：这两串信息务必当场抄下来存好。页面刷新后不会再展示，重置还会改写数值，届时机器的绑定关系可能就断了。

![](img/6dc4fb797cb5abcbf0c318712eed550d.png)

下面的截图就是 AppID 与 AppSecret 的展示位置，趁此刻存妥。

![](img/fab9ef5138d82cc245f35c533f20f251.png)

3. 接下来把绑定信息填进 OpenClaw，示例以腾讯云的配置流程为准。

![](img/5f095faa067dccd6b0bb1fdba1a3e569.png)

配置结束后，🐧 里会收到机器人推送。进入聊天窗口，问一句“你好，你是谁”，有回应就说明大功告成。

![](img/dd242005ea84092145ca553dc7b40d53.png)

![](img/8a59bca20fa191d15169dec9c6f69ceb.png)

（三）钉钉通道

1. 登录钉钉开放平台（https://open.dingtalk.com），右上角进入“开发者后台”。

![](img/b99f1ed79cfdfe7e33cfdf9f527a4498.png)

依次点顶部“应用开发”、左侧“钉钉应用”，屏上会出现“立即创建”。

![](img/3c66af118e700f23f9ddb009e80f915a.png)

2. 跳转到“创建 OpenClaw 机器人”界面，名称与简介留默认或自行修改都行。

![](img/a04d1cb0089d7584ec336b5b600962d5.png)

3. 点“确定”后，新屏会列出 Client ID 与 Client Secret，请保存。

![](img/ccca53799b2c79d8b3049b75692cccb6.png)

4. 回到腾讯云 OpenClaw 完成绑定。

![](img/d824267d65b2e2f0802fffc6ee0adfb5.png)

之后在钉钉搜索刚建好的“OpenClaw 小钉”，进去发“你好，你是谁”，能收到回复即配置成功。

![](img/d8546c61168a5a6fbb39d257c56fcf65.png)

![](img/6fb53ce2d446e501083b9909d4653172.png)

（四）企业🛰️通道

1. 浏览器打开🛰️管理后台 https://work.weixin.qq.com/ ，扫码登录；还没企业的先建一个。在“管理工具”里找到“智能机器人”并进入。

![](img/bd3a003767daa06168cd72bc1dd0ec2d.png)

2. 点“创建机器人”。

![](img/316655717aa61f597da0fdc70aa84d73.png)

3. 页面出现后选择“手动创建”。

![](img/f3f540227dda238d3a22a28440b1ec7d.png)

4. 滚到底部，点“API 方式创建”。

![](img/522b6f126b9442c1e705c6c24d5bfd94.png)

5. 新页面选“使用长连接”，把 Bot ID 与 Secret 记下。

![](img/f6a70064d57a24dd37a243312033c0cd.png)

6. 填好机器人名称、简介，点“确定”。

![](img/e8b22d2f4b13f7068e6fbbc7f63fc482.png)

7. 转到腾讯云 OpenClaw 的绑定区，把 Bot ID 与 Secret 粘贴进去，点“添加并应用”。

![](img/7b9975acbb17d63bea28919cfd9f6d4d.png)

8. 点右上角三个小点调出二维码，手机企业🛰️扫一扫，即可打开对话窗口。

![](img/cba8b55034581becfdab2fde12fb6fc2.png)

9. 在 OpenClaw 会话里发“你好，你是谁”，收到回音即接入完成。

![](img/41c57b230cdf12b69006b26ac624ebe3.png)

## 2.3 换种方式跑 OpenClaw

前面这些步骤看着确实不少。更推荐的做法还是上云服务器，装法灵活；如果你已经在云服务器上跑通，直接翻到实操章节即可，本节只作扩展了解。

要是只想先尝尝鲜，又倾向于本地环境、不愿折腾配置，可以看看下面几种：

• WorkBuddy：本地安装、一步到位，算是 OpenClaw 的一种变体，并非套壳，装在自己机器上。
• QClaw：腾讯手机助手团队出品，是少数支持🛰️的方案之一，同样本地运行。
• 飞书 OpenClaw 一键部署：零配置，一个按钮解决，自动打通飞书体系的权限，开箱即用，跑在云端。

怎么挑：

1. 日常泡在飞书里，就选飞书 OpenClaw。
2. 想在自己电脑上用，优先 QClaw，能连🛰️，一键启动。

（一）WorkBuddy 方案

WorkBuddy 也是腾讯家的东西，由 WorkBuddy 团队收购而来。要说明的是，它并非 OpenClaw 的包装，底子是 CodeBuddy 这款产品。

前面提过，不少模型厂商和云厂商都推出了一键部署方案，把这套能力产品化。你拿到的只是一个实例，不必自备服务器。这类路线门槛最低、性价比也最高，代价是可玩性打了折扣，对新手相当友好。

像智普的 AutoClaw、腾讯的 WorkBuddy、火山的 ArkClaw，都是把能力封装进自家产品，并内置多家模型可选。

之所以选 WorkBuddy 来讲，主要是它能连🛰️——手机上不必再装别的 App，🛰️随手就能用，虽然功能上会弱一些。

新用户有 500 积分的限时赠送，等于零成本试水。

为什么值得一试？

它是腾讯打造的一款桌面级职场 AI 智能体，定位覆盖各类办公场景。你只需把诉求说清楚，它就会像搭档一样自己拆解、自己推进，最后把能验收的成果交到你手上。

它和普通的聊天机器人不一样：既能理解大白话，也会自己动脑，还能动手读写你电脑里的文件，切实替你分担工作。

安装过程跟装一款普通应用没差别：下载、双击、完成。Node.js 不用装，API Key 不必配，macOS 与 Windows 都兼容。

**拿手之处**

• 一句话下达任务：日常口语描述就行，不涉及复杂操作。
• 自主规划执行：任务自动拆解、步骤自动安排、成果自动交付。
• 多任务并行：多个任务可以同时开跑并分别管理，适合并行推进。
• 本地文件操作：经你授权后读取电脑目录，完成批量化处理。
• 结果可验收：输出的文档、表格、PPT 均可直接拿来使用。

**用在哪**

工作模式——对应职场常见事务（默认）：

• 文档生成：工作报告、技术文档、README 等。
• 数据分析：导入数据文件，自动完成分析与可视化。
• PPT/报告生成：根据需求描述直接产出演示稿与报告。
• 深度研究：针对复杂课题深入调研并成文。
• 邮件撰写、周报整理等办公事项。
• 批量文件处理：自动归类、改名、转换格式。

编程模式——对应代码开发：

• 日常编码辅助：生成代码、审查代码、修复缺陷、重构优化。
• 项目理解：迅速摸清陌生仓库的架构与实现逻辑。
• 网站/应用开发：从需求一路辅助到代码落地。

可与🛰️、企业🛰️、🐧、飞书、钉钉直接连通：

模型按需切换：出厂默认 Pony-Alpha-2，同时兼容 GLM-5、DeepSeek、Kimi、MiniMax 等各家模型 API。

![](img/b86cbfaa8590337bc908dbdf3bbb5a06.png)

![](img/47cd775268d5f61da0e927df5d55a0e9.png)

## 一、下载与登录

访问 WorkBuddy 官网 https://www.codebuddy.cn/work/ ，点“下载 WorkBuddy”，底部即是下载区。

![](img/9b57088bd9916c7e6ed9ead08464fd4f.png)

按你的系统版本挑一个。

![](img/cc506538e380007a11eb6f5d967d4070.png)

装好后用🛰️登录。

![](img/c99a89bf32352dee0fc5dece2c5edc2b.png)

![](img/78eb7f57def00cfde427677363007ebd.png)

![](img/a9b0a48d48b79925c6e331591e785f6d.png)

## 二、聊起来

WorkBuddy 以任务为核心。先建一个任务，右侧选类型：

代码开发：开发场景用。
日常办公：日常事务用。

左边那个 Claw 就是 OpenClaw 本体，直接跟它对话就能派活。WorkBuddy 还内嵌了一个 IDE，代码管理和网页预览都在这儿。

![](img/a3dc9531b1f45b2a9714ea49d2610a81.png)

技能 Skills 是供 OpenClaw 调用的能力库。内置已有几十项，似乎暂未打通 SkillHub（腾讯的 ClawHub 镜像），但支持手动导入——从官方市场下载后再导进来即可。

![](img/fa4611335a256ed050e5344aae84525a.png)

插件部分官方预装了不少，例如浏览器操作 playwright-cli、PDF 与 PPT 处理等。

![](img/4c599c795ebff1517497ed7bfcde9b84.png)

自动化相当于 OpenClaw 的定时任务，按设定时间自动执行。

![](img/34c5b48246ee86cf2de528c0fcdb7496.png)

# 让 AI 助手住进🛰️和飞书：安装、部署与避坑

![](img/61e204c9e9ac6b6cf68b4a093fa95823.png)
在右上角点头像，个人中心随即展开，剩余积分看得清清楚楚。

![](img/27a37720a964753fffdc76d8136fd13b.png)
点开 Claw 里的“设置”，配置面板随之出现，各类接入渠道都在这里统一管理。打开🛰️客服的集成开关后，就能借由 WorkBuddy 的客服号，在🛰️里直接和 AI 小龙虾对话。

![](img/dac762c3f6d7230a4488e9e799139ddd.png)
接着试试编程功能，右侧会实时渲染结果，体验相当顺滑。

![](img/8cc49b212a0c68cfe344feefe547c943.png)

![](img/c5e6437b4159d440c51580ce8cc23113.png)

## （二）QClaw

💡本地安装

这款产品出自腾讯电脑管家团队，Windows 与 macOS 都能运行。自带了灵感广场和大量 skills，开箱可用，还附赠 4000 万 TOKEN，目前不用花一分钱。需要留意：它不能配置自定义模型的 API 密钥，也不支持 Coding Plan。好消息是，邀请码已经正式放开了。

官方下载入口：https://qclaw.qq.com/

![](img/faf1644b88f35d80bb7474b7b4893f3f.png)
下载完毕，直接双击运行，这里以常规流程为例。

![](img/3390f9b0238bc96af808821331da272f.png)
系统弹出安全提示时，选“是”即可。

![](img/2bfa7c7d7e897143abdff465e182e5d8.png)
接下来指定安装目录，等待进度条走完。

![](img/dcb4c80c147e84eac25cb18da69281b7.png)

![](img/0133fbdc4276562c59e4758efd92086c.png)
最后点“完成”，桌面上就会出现 QClaw 的快捷方式。

![](img/0e5d8d37c9bbb00bc595c073987788e9.png)

![](img/6e8b4b34cb2999a8cb6d9e626a4ea7c1.png)
装完之后，QClaw 默认会自动打开。

![](img/bfc0d5dab3342bd9569c413e4e678ea4.png)
进入主界面，点左下角的「未登录」，按提示用🛰️扫一扫完成登录。

![](img/a3c526894e176e4672709ab9e863ce7a.png)
屏幕上会弹出二维码，用🛰️扫一下，登录随即完成。

![](img/3cf7efbeb9b811af417760e480a27e85.png)
登录进来后，左下角会提示连接🛰️，按下「关联🛰️」按钮。

![](img/34d28b1c5e10037dc84a3b38170f8fc1.png)
再对着页面中央的二维码扫一次。

![](img/23df5971adf36e94222817b6653e0dd6.png)
手机端随即出现名为 QClaw 客服的🛰️账号；电脑端也会弹出🛰️已连接的提醒，点确定即可。

![](img/1be2f64657ca18dc281c419d2452680e.png)

![](img/111f8575ddb9cfa73a321fdbf29e66fa.png)
如果看到类似截图中的报错，先不用理会，直接去客服机器人那里发条消息。

![](img/be877f5b1526f5a74e7d71f5f7df694b.png)
发一句“你是谁”试试——手机端秒回，电脑端 QClaw 这边也紧跟着展示了消息。

![](img/d3ae62be26fe757fe6113c7726f2d57d.png)

![](img/637ec89a99198242fa95ec33d3b8472c.png)
到这里，QClaw 的基础安装就完成了。接下来探索玩法：左下角的灵感广场值得常逛，没想法时翻翻里面的案例，看中哪个点开即用。

![](img/60c0b5d4831372a201958ab418d32f4e.png)
比如打开“热点资讯自动汇总”，然后按下“立即使用”。

![](img/808feb763493868fa045d83d8280ce59.png)
随后 QClaw 会追着你确认：要采集哪方面的内容？放到几点执行？

![](img/6720d2bd53596ca242c7ab1d50469bb9.png)
照下面这样回一条即可，核心就两点：1. 时间定在何时；2. 要哪一类新闻。

Markdown

```
每日早上8点抓取全网的AI相关新闻，发送给我
```

![](img/e1baa3be070d570821ee286dc178da48.png)
定时任务也是一大亮点——上文让 QClaw 按点推送 AI 新闻，靠的正是这个功能。

![](img/1872be55b9bc7141150517e8db05a526.png)
眼下能连上🛰️的渠道，数来数去只有 QClaw 和前面提到的 WorkBuddy（原文写作 WorkBody），更多玩法可以自行探索。💡坦白说，🛰️生态目前相当封闭，添加进来的这个机器人只是客服号，挂靠在🛰️的次级目录之下；我们既没法把它请进群，也没法把群消息转交给它——这是眼下的客观限制。

![](img/6be2200d80905ffb96f6934c3d57cef8.png)

## （三）飞书一键部署 OpenClaw

💡这个方案的精髓在于“一键”：只点一下，从运行环境到飞书机器人的权限配置全部就位，剩下基本不用动手。等装好的通知送达，OpenClaw 就能直接开用。但要当心额度，可能问不了几个问题就耗尽了。

飞书团队在“妙搭”平台上线了 OpenClaw 的一键部署能力，省去了购置服务器、搭建环境、申请开放平台权限等琐碎环节，轻点几下按钮，就能在飞书客户端内和智能体直接对话。

**1. 操作步骤**

访问飞书妙搭的 OpenClaw 部署页面：https://openclaw.feishu.cn/home，参考图 3-2，点击“创建”即进入部署流程。

![](img/636db52752c2c046e35f69dcd17ccd6b.png)

还没登录的话，记得先把飞书账号登上去。接着参考图 3-3：在“名称”栏填入助手名字，再挑一个合眼缘的头像，最后点“创建”进入下一步。

![](img/45142840133c92d6d365265a4f2fe436.png)

随后出现图 3-4 的画面，OpenClaw 助手开始创建，安心等待即可。

![](img/95ef87725e384c94882f4989cb838691.png)

当图 3-5 的界面显现，就代表添加成功。

![](img/6b5ea81dc76ec9b0c483fd8dec475fff.png)

紧接着飞书会发来 OpenClaw 助手添加成功的消息，如图 3-6。

![](img/63a322e634328d74e5fa0841a369eceb.png)

部署结束，飞书里多出一个机器人联系人。主动打个招呼试探一下——若能收到回复，恭喜：这只“虾”已经成功养起来了，见图 3-7。

![](img/eae1aec9890149310fdf0b18659c3b50.png)

最叫人省心的是权限配置：换作从前自己动手对接飞书，得在开放平台建应用、逐项勾选权限、还要走发布申请流程；现在这些环节统统跳过，妙搭会在对话框里一步步引导你授权。手机端的操作也大同小异：在飞书“工作台”搜出“妙搭”，点进去选“一键部署 OpenClaw”，后续流程和电脑端几乎一致。

**2. 免费额度**

妙搭内置模型每日赠送 100 万 token，注册当天还会额外到账 400 万 token。平时尝尝鲜、轻度用一用，绝对够。云主机规格为单核 CPU、4GB 内存、1TB 硬盘，这台配置带一只“虾”绰绰有余。目前该项服务处于免费期，具体截止以官方公告为准。

**3. 限制在哪**

妙搭确实是上手最快的路线，但它的边界值得了解。

• **模型没有选择权。**只能使用妙搭内置模型，无法替换为 DeepSeek，也换不成 Claude 或 GPT。要是你在模型方面有特定偏好，或者经常需要在不同家之间来回切换，此路不通。

• **活动范围被圈在飞书。**对话只能在飞书这一个客户端里展开，想把钉钉、企业🛰️或 🐧 一起接进来？没门。想通过 Dashboard 统一管理？也不方便。

• **扩展空间有限。**自定义 workspace 文件、安装 Skill、编排多智能体等高阶玩法，论灵活度，妙搭远不如自己搭建的方案。

• **数据落在飞书。**对话记录与配置都存放在飞书的服务器上，不会进入你自己的硬盘。

一句话总结：妙搭很适合来回答一个问题——OpenClaw 是否值得你花一番心思去捣鼓？试了几天若觉得“够了”，继续用妙搭也完全可以；可一旦你开始琢磨：换一个更聪明的模型，也让钉钉跑起来，拥有更宽阔的定制空间——那就到了亲手搭建自有方案的时候。

![](img/3a559c2e0a5f82fa72d7c30b5c7fa4d4.png)

## 2.4 龙虾怎么养🦞

### （一）领养方式有哪些

![](img/14f67ff1eed41b2e38f3521e6b8876c6.png)

| 安装途径 | 适合谁 | 说明 | 快速入口 |
| --- | --- | --- | --- |
| 一键安装：各云厂商的养虾套餐，如智普 AutoClaw | 刚入门的新手 | 下载安装、运行注册即可使用，模型与免费配额都给你备好了 | https://autoglm.zhipuai.cn/autoclaw/ |
| 手动安装 | 想掌握全局的人 | 在终端敲几条命令，模型与配置随意挑 |  |
| 安全优先 / 多智能体 | 注重隐私 / 多人协作 | IronClaw（WASM 沙盒）/ HiClaw（多只虾打配合） |  |
| 云端托管 / Docker | 部署到服务器 | 各云厂商均有托管方案 | 火山引擎 9.9 元起、腾讯一键部署 |

### （二）上岗四步法：把 AI 助手雇下来

| 环节 | 打比方 | 具体动作 |
| --- | --- | --- |
| 找场地 | 给员工安排工位 | 安装 OpenClaw（本地电脑或云服务器均可） |
| 备口粮 | 给员工发报酬 | 配置模型 API 密钥（Token 相当于这只虾的口粮） |
| 留联系方式 | 让客户随时找到人 | 接入聊天平台（🐧 / 飞书 / Telegram） |
| 上岗培训 | 带员工熟悉业务 | 配置智能体、工具和定时任务 |

### （三）避坑要点

**安全：** 安全这事马虎不得，风险来自两头。一头是小龙虾自身的权限过大，它能操作本地文件，稍有不慎就可能删掉硬盘数据，此前已发生过它失手删除 X.com 高管邮件的真实案例；另一头来自外部，很多人把虾装完就完事，服务器连最基本的防护都没有，等于门户大开，黑客一旦得手，虾体内保存的各种 API 密钥就会被卷走，早前有公司因此折损了数万美金。所以一般建议让小龙虾的活动场地与你的工作区隔离开来，比如扔到独立主机里，或起一个虚拟环境，这点后面会讲到。

**成本：** 记得为 API 调用设好权限与消耗上限，尽可能多用缓存和本地模型，同时时刻盯住 Token 用量。接入时优先选编程套餐，更划算。

![](img/a3849a84152c54d423aa6bb7ecc117ea.png)

## 1. OpenClaw 入门玩法（先练练手）

### 3.1 让新闻总结定时送达

💡示例环境：OpenClaw 模板部署在腾讯云的一台轻量服务器上。

先把 skills 装上。

Markdown

```
安装这个 https://clawhub.ai/joargp/news-summary  skills，并介绍下当前这个 skills 功能
```

![](img/04f32348e0714ce7c49120c071a457ff.png)

接着，把下面这段话发给它：

Markdown

```
设置每日「8:00」的自动定时任务，
自动抓取全网的今日「AI科技」相关热点、重要资讯与要闻简报，
整理成简洁清晰的内容发送给我。
```

![](img/74ff051d96462fb469aa3b543df6a4e1.png)

![](img/101ddf5c3e52c3f610515addec22eed8.png)

### 3.2 发票归档与单据统计

💡示例环境：沿用上一节的服务器与 OpenClaw 模板。

这里需要两个 skills，直接把下面的这段内容丢给小龙虾：

Markdown

```
帮我安装如下两个 skills

https://gitee.com/iamzhihuix/claude-official-skills-mirror/tree/main/skills/pdf
https://gitee.com/iamzhihuix/claude-official-skills-mirror/tree/main/skills/xlsx
```

补充一句：这些 skills 其实是 Claude 团队官方发布的技能包，只是做了镜像，方便网络条件受限的朋友使用。

![](img/8298bbc4cacfa885a333fbb34bbbde1a.png)

等它跑完，会主动说明支持哪些功能。我们拿一张发票来试，把发票内容发给它，请它按报销格式整理，效果见下图：

Markdown

```

这个是我的发票信息，帮我整理成报销的格式
```

![](img/7468a87887f3b5ed2b8e6800e7a510c1.png)

整理好的报销表单随一个 Excel 文件一起发了回来。打开一看：收款单位、开户银行、银行账号、总金额，每一处都和 PDF 原件完全一致。

![](img/45f5aad3148d25f375ac0ec110a213af.png)

附上 Excel 原件：

[

![](img/1f45bad69a177710c3f117be8d81ff52.png)

expense_report.xlsx](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/AcszbhHC4o7TqExQgDIcCGjBnUd?response-content-disposition=attachment%3B%20filename%3D%22expense_report.xlsx%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260526%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260526T153247Z&x-oss-expires=86400&x-oss-signature=e8dde14c9c1abeecf1dde524a8b17573c0faeeb43c880fc49fec9338fd0f8d7d&x-oss-signature-version=OSS4-HMAC-SHA256)

如果你的 OpenClaw 跑在本机，直接把文件路径发过去即可。

Markdown

```
/Users/happypeet/Downloads/invoice-农耕记.pdf 这个目录下的这个文件
```

![](img/e4fd0731b01c7dcad7561deda85e3f8e.png)

![](img/15a50b8e4734bd05e183de1638cd78c9.png)

### 3.3 论文检索与精读

💡示例环境：沿用前面的 OpenClaw 部署环境。

还是先装 Skills，这一步交给小龙虾自己完成就好。把提示词丢过去：

Markdown

```
帮我安装下面的两个 skills：
https://gitee.com/iamzhihuix/zhihui-awesome-skills-open/tree/main/skills/arxiv-reader
https://gitee.com/iamzhihuix/zhihui-awesome-skills-open/tree/main/skills/arxiv-watcher
```

等它提示安装结束。

![](img/e4afd2bed78d393c29ff21f11d06f9eb.png)

再请它讲讲那两款 skills 各自能干什么。

![](img/a13dafddd430b3f6b3a978da5a254ead.png)

比如，让它找找与 LLM Agent 相关的近期动态：

Markdown

```
最近一周有哪些关于LLM Agent的新论文？
```

![](img/f49d78e109e520224003241284609bf9.png)

它会递来一份近期的 LLM Agent 笔记清单，并提示：把对应 ID 发过去，即可查看完整内容。到这里，论文检索和单篇精读的目标都达成了。接下来若有了新想法，顺着它的引导继续对话即可。

![](img/9f95a20d51a3e41ea96e3e750ea85192.png)

### 02. OpenClaw 实战：搭一个会说话的知识库

**1. 用 OpenClaw 建自己的知识库，让作者替你出主意**

把梁宁、刘润、华杉请进同一间会议室，让他们围着你正发愁的问题各说各理、来回交锋半小时——这种场面，过去只能存在于幻想里。

现在，一个自己的知识库就能把它变成现实。

在 OpenClaw 的逻辑中，你读过的书、存下的干货，不再只是静态资料。它更像给每位作者配了一个可随时上场的数字替身。比如你抛出一个品牌难题，华杉可能从**超级符号**切入；刘润会顺着底层逻辑算成本账；梁宁则会揪住用户对**确定性依赖**不放。这时的你，更像会议主持人，而不是资料管理员。

接下来这章只做一件事：花半小时，把收藏夹里沉睡的作者唤醒，让他们全天候待命，随时加入你的讨论。

耗时约**30 分钟**，搭完可长期复用。

**开工前，先核对三样东西**

- 一台已经部署 OpenClaw 的腾讯云轻量应用服务器。
- OpenClaw 的模型要已连通，能正常聊天。演示时用飞书与机器人（小龙虾）沟通，你换别的 IM 也没问题。
- 一个🛰️👸号，个人订阅号即可，后面登录导出工具时会用到。

全程不用写代码，按下面流程操作即可。

**第一部分：先把模型接好**

如果 OpenClaw 还没配模型，就从这个环节开始；已经能对话的，直接跳到下一部分。

**1.1 开通 MiniMax Coding Plan**

对话能力要靠模型驱动。这里用 MiniMax，图的是国产模型里比较划算。

1. 浏览器打开 MiniMax 开放平台，注册并登录。
2. 进入「套餐管理 → Coding Plan」，选 Starter 月度套餐，29 元/月。每 5 小时可对话 40 次，日常问答够用。
3. 买完后在同一页面找到 **API Key**，前缀是 sk-cp-，点复制。

![](img/67a71e7e8ebd45cfbcedb4ffacbdc3a6.png)

**1.2 把模型填进 OpenClaw**

1. 进入腾讯云轻量应用服务器的 OpenClaw 管理页。
2. 找到「模型 （Models）」区域，第一个下拉框选 MiniMax（国内-Coding Plan）。
3. 第二个下拉框选 **MiniMax M2.5**，这是最新旗舰，效果最好。
4. 粘贴刚才复制的 API Key。
5. 点添加。

**1.3 接上飞书通道**

1. 在「通道 （Channels）」区域选飞书。
2. 按页面提示创建并绑定飞书机器人。

**1.4 试一句**

在飞书找到刚建好的机器人，发“你好”。有回复就说明通了。

![](img/3b1298fd584c20d3fc68435e2f64ba9a.png)

![](img/c68385ebe6e0af2ccc084962ff72845c.png)

**第二部分：准备要喂给知识库的素材**

知识库的上限由素材决定。投喂劣质内容，产出也难好；喂进高密度信息，它才可能给出高价值回答。

下面拿 4 位商业作者的公号文章做样例。你也可以替换成自己的材料，比如读书摘记、行业报告、竞品拆解，只要是你日后大概率会回查的内容都行。

**2.1 把👸号文章导出来**

这里借助一个网页版免费工具，批量下载👸号文章，不用装软件。

**前置条件**：准备一个🛰️👸号，个人订阅号即可，免费注册。没有就去🛰️公众平台开一个，几分钟能完成；临时借用朋友的👸号扫码也行。

**第一步：打开工具并扫码**

1. 浏览器访问 https://down.mptext.top。
2. 点左下角「登录👸号」。
3. 🛰️扫码，选择自己的👸号完成登录。

![](img/8ff55e72cec8c519dd2488b21f0920d6.png)

**提醒**：扫码只是拿接口权限。登录之后，你搜索和导出任何👸号的文章都不受限制，不限于自己那个号。

**第二步：把目标👸号加进来**

1. 点顶部「添加」。
2. 搜索框输入👸号名，例如“刘润”。
3. 在结果里点中对应账号。

![](img/20262b000ec6e1ad8c38824f9284baa8.png)

接着系统会拉取这个号的文章清单。

![](img/49f296a4731798a172cd1eb8f387da6e.png)

按同样方式可以加好几个号。本次演示用的知识库包含这些👸号：

![](img/8ea6cc1d285b7bfd0e36e42ea6475e81.png)

**第三步：抓正文**

1. 左侧菜单点「文章下载」。
2. 顶部下拉框选一个👸号。
3. 勾选要导出的篇目，点表头全选框可一次全选。
4. 右上角点「抓取」→「文章内容」。

![](img/25cf55ece76c00f998bf7759e65fc07e.png)

随后系统会一篇篇抓取正文，页面上有进度可看。

**第四步：存成 Markdown**

抓取结束后：

1. 再全选一次文章。
2. 点「导出」→ 选 **Markdown**。

![](img/a06752341611fb7e325de5a963b54c8b.png)

3. 浏览器会让你选保存文件夹，确认后开始导出。完成后得到一个文件夹，里面每篇文章对应一个 .md 文件。

![](img/ce894809222e811355ec7c9a358906d6.png)

![](img/c7b8cbcd893be61fb199aa3e7ce76d8b.png)

**第三部分：正式搭知识库**

重头戏在这里。不过不用被技术吓到，实际动手的是 AI，你主要做复制粘贴。

**为什么不直接把文章丢给 AI 问答？**

假设面前摆着一整柜书，每次提问都让 AI 从头翻到尾，显然不现实。更合理的做法是先做一套索引，类似图书馆的目录体系。

AI 会先拆分成小片段，再为每段生成语义指纹并入库。等你发问，它用问题去比对指纹，很快锁定最相关的片段。这里靠的是语义理解，而非字面关键词。

所以即使你问的是“小团队如何对抗大厂”，原文通篇没写“小团队”，它也可能命中讲破坏性创新的段落。

**3.1 打包文章，发给 AI**

不用手工建目录，也不用自己往服务器传。把文章压缩后丢给飞书里的 AI，后面由它自动跑。

提醒：飞书不能直接发文件夹，先压成 .zip。

1. 找到刚导出的文章文件夹。
2. Mac 右键选压缩；Windows 用“发送到 → 压缩文件夹”。
3. 打开飞书，进入 OpenClaw 机器人对话。
4. 把 .zip 拖进输入框发送。

![](img/865465843770e036b0d26e0fb56c7187.png)

**3.2 发搭建口令**

zip 上传完成后，把下面这段指令原样发给 AI：

```
我想用这些公众号文章搭建一个本地 RAG 知识库。请按以下步骤操作：

1. 先看看文件夹里有哪些文件，列出来
2. 安装依赖：pip3 install openai chromadb tqdm python-dotenv
3. 把所有文章文件保存到 ~/.openclaw/workspace/kb_fulltext/ 目录下，按作者名建子文件夹分类
4. 写一个切片脚本 chunk.py，把所有文本文件切成 500 字一段的片段，相邻片段重叠 100 字，记录来源文件名和分类，输出为 chunks.jsonl
5. 写一个向量化脚本 embed.py，用硅基流动的 Embedding API（模型：BAAI/bge-large-zh-v1.5，base_url：https://api.siliconflow.cn/v1），把所有片段向量化后存入 ChromaDB，支持断点续传，每次处理 500 个片段（防止超时）
6. 写一个查询脚本 query.py，接收问题文本，从 ChromaDB 检索最相关的 top-k 条结果，输出来源和摘要

硅基流动 API Key 我稍后提供。先从第 1 步开始。
```

AI 会按步骤自动处理，大致包括：

- 解压并列出全部文章，按作者归好类。
- 安装 Python 依赖。
- 把文章存入工作目录。
- 写切片脚本并执行，产出数千条文本片段。
- 写向量化与查询脚本，然后等你给 API Key。

![](img/ad528bd59e04880724a9079710a2096e.png)

**这里要给它一点时间。** 处理文件、写代码、跑脚本加起来，通常 10 到 15 分钟。素材多的话，比如几十本书，可能拉到 20 到 30 分钟。它没立刻回你不代表卡住，后台还在干活，去倒杯水再回来即可。

**3.3 注册硅基流动，拿 API Key**

跑到第 5 步时，AI 会停住并向你索要硅基流动的 API Key。这个 Key 用于向量化，也就是把文本转成模型可计算的数字表示。

选硅基流动（SiliconFlow）的理由很直接：国内可直连，手机号就能注册。

1. 浏览器打开 cloud.siliconflow.cn。
2. 手机号注册并登录。
3. **做实名认证（很重要）**：进「账号管理」→「实名认证」完成认证。未认证账号请求频率限制很严，向量化时会报 RPM limit exceeded。
4. 左侧点「API 密钥」→「创建新的 API 密钥」。
5. 名称随意，比如“知识库”，点创建。
6. 复制生成的 Key，前缀为 sk-。

![](img/a67b87b70e578001fd83ed5ef86c9cd2.png)

这串 Key 要保管好，丢了只能重新生成。建议先放进笔记软件里保存。

**3.4 交 Key，跑完向量化**

在飞书里把 Key 发给 AI：

```
硅基流动 API Key：（sk-你的真实Key粘贴在这里）
请继续运行向量化脚本。
```

![](img/e99cfb4143d2b5743133fa88e6508dcb.png)

AI 收到后会调用向量化脚本，把全部片段转成语义向量写入库。耗时取决于素材量，大约 2 到 15 分钟。

跑完后，它会回报搭建成功，并给出处理的片段总数。

![](img/b8d735623859b2f4891aef167c209bed.png)

**3.5 让 AI 建一个知识库 Skill**

向量化结束还不够，要让 AI 记住这个库的存在，之后提问时自动检索。把下面这段发过去：

```
知识库搭好了。请帮我创建一个 Skill，让你以后自动使用这个知识库：

1. 在 ~/.openclaw/workspace/skills/knowledge-base/ 目录下创建 SKILL.md
2. Skill 的回答要求：
   - 收到问题后，先把问题拆解为 3-5 个相关关键词，分别用 query.py 检索知识库
   - 不要只找精确匹配——即使知识库里没有直接讨论这个话题，也要从检索到的内容中提炼出作者的思维框架和方法论，用这些框架来分析用户的问题
   - 回答时按作者分段，说明每位作者会怎么看这个问题，引用原文作为支撑
   - 最后给出整合后的建议
   - 永远不要说&quot;知识库里没有相关内容&quot;——只要检索到了任何相关段落，就用它们来回答
3. 创建完后读一下这个 Skill，确认生效
```

它会生成 Skill 文件并回复确认。

![](img/9425716f5e987f07e9e338ad24ebc650.png)

**3.6 实际问一句试试**

库建好后，直接在飞书里试问：

```
小公司怎么跟大公司竞争
```

![](img/64ecfeade7b056704f2073ae3e853f0e.png)

重点看它怎么答。AI 从三位作者的文章里分别抓到了相关观点：

- 刘润谈差异化，引到他讲蓝海战略的内容。
- 华与华强调聚焦，提到企业再小也要守住别人抢不走的根据地。
- 黄有璨讲小而美，带出他对一人公司的思考。

最后它把这些线索合成一句：别跟对手正面拼，先找细分市场扎下根。

这才是知识库的价值所在。这几位作者从未同场讨论过“小企业如何竞争”，但 AI 从各自文本里抽出思维框架，拼出一个没人单独给过的答案。

而且每条观点都带出处，能回到原文核对，不是凭空生成。

**没有知识库时**，AI 像个什么都懂一点的泛泛之交，但都不深。**接入知识库后**，更像是你熟悉的那几位作者一起坐在对面，各自把观点摆出来。

![](img/01131f802bc948300f3f12644ba59c51.png)

**第四部分：进阶用法**

**4.1 往库里加新内容**

知识库不是一次建完就封死，它支持持续扩充。之后要加新文章，照第二部分的导出流程再走一遍：

1. 用 https://down.mptext.top 把新文章导出为 Markdown。
2. 压成 .zip，发给飞书里的 AI。
3. 对它说：

```
我新增了几篇文章，请添加到知识库里，重新切片和向量化。
```

AI 会自行处理，已经入库的部分不会重复折腾。

提醒：别直接把👸号链接丢给 AI，🛰️文章有访问限制，它读不到。必须先用导出工具下载成文件。

**4.2 跨来源关联提问**

这是知识库最值得用的能力。下面几种问法可以试试：

```
知识库里所有作者对&quot;用户增长&quot;这件事，有没有互相矛盾的观点？
```

![](img/7e2ae4f118756ce8204d21e42e718ea9.png)

单靠一个通用 AI 很难完成这类问题，因为它要求在你的库中真实检索、对照并整合多份原文。

**4.3 调风格，并让它记住**

你可能会觉得，刚才那段回答太像学术报告，术语和引用堆得有点多，不太顺口。

这时可以直接把想要的表达方式告诉它：

```
我发现目前你给我的答案，读起来像是论文，非常费力。能不能调整一下？我希望能像朋友吃着小龙虾喝着啤酒在给我唠嗑的感觉。
```

![](img/260db7047795cf8e5923d62fb491401a.png)

**它会马上换风格。** 但更关键的一步是把这个偏好固定住，不然下一轮对话又回去了。

接着对它说：

```
请帮我把这个调整，记录在对应的工作流程里
```

![](img/f08079d019c93347d4d5400a7516d0b9.png)

AI 会把你的偏好写进 AGENTS.md（工作规范）和 SOUL.md（人设设定），之后每次对话都按这个来。

这种调教很实用。回答风格、细致程度、语气都能随时改，再让它记住。比如限制在 200 字内、多用类比少用术语、先给结论再展开。说一次，后面一直生效。

**4.4 还能往里放什么**

教程拿👸号文章举例，但知识库并不挑内容，任何文本都能放：

![](img/f0de32832b558e44b66fee909a17f569.png)

重点不是放进去的东西本身，而是积累到一定量之后，它会抛出你意想不到的关联——那种靠手工翻笔记很久也碰不到的连接。

**附录 A：另一条路——NotebookLM（需能访问 Google 服务）**

如果你能访问 Google 服务，NotebookLM 是更省事的选项。不用跑代码，也不用服务器，浏览器上传文件就能问。

**它和本地 RAG 的差异：**

![](img/2e931df30d2956498d936ef4e24117c5.png)

**两者并不冲突**，完全可以并行。平时用 NotebookLM 快速查，遇到上百篇这种大规模检索，再交给本地 RAG。

**A.1 快速上手**

1. 浏览器访问 notebooklm.google.com。
2. Google 账号登录。
3. 点「新建笔记本」。
4. 点「添加来源」，上传文件。支持 PDF、TXT、Markdown、Google Docs、网页链接。

![](img/6ef6f3977f2ded9d1a0244b90d69e1a7.png)

5. 上传完，直接在下方输入框提问。

可以拿这个问题试手：

```
刘润最近的文章里，有没有观点跟他以前的说法矛盾的地方？
```

![](img/d3edb2f6107ee1e99a73e8c326dff8d7.png)

留意回答挖得有多深。NotebookLM 找出了刘润在不同阶段对同一议题的不同立场：

- 关于 OKR：早期他强调管理要简单，别被复杂数字拖住；后来的说法却转向管理必须量化，OKR 指标要细密。
- 关于人才培养：他一方面认为成年人更适合筛选而非教育，另一方面又强调招人看态度、技能靠培训。

它不只把矛盾挑出来，还给了更深一层的解释：这些看似前后不一致，其实是刘润面对不同管理痛点时的演进，视角从宏观的心智建设下移到微观的人性漏洞防范。

能让同一作者的观点互相照面，这恰好体现了 NotebookLM 的理解力。它是真读懂了内容，而不是只对关键词做匹配。

**A.2 接到 OpenClaw 里（可选）**

如果不想每次都开浏览器，而是直接在飞书里查 NotebookLM 的内容，可以把它接进 OpenClaw。

在飞书里把下面这段发给 AI：

```
请帮我安装 notebooklm CLI 工具，然后接入我的 NotebookLM 笔记本。
我会提供 Notebook ID，你帮我配置好，让我以后可以在飞书里直接查询。
```

![](img/b30b073192ea4cd1569bd01c8405ba53.png)

# 知识库上线了？先绕开这几处暗礁

从安装到参数配置，全程都有 AI 领着你走。你唯一要提前掏出来的东西，是一串 NotebookLM 笔记本 ID——翻一眼浏览器网址栏就能看见它。

一切齐备之后，在飞书对话框里把问题抛给它就行（玩法这里先藏着，好奇心重的自己动手试一次就懂了～）

Plain Text

```
从 NotebookLM 里查一下：刘润怎么看&quot;底层逻辑&quot;
```

## 附录 B：疑难速答

**Q：做向量化时报 RPM limit exceeded 怎么办**

这是硅基流动侧的规则在起作用：账号若没完成实名验证，调用频率就会被压住。处理顺序是：打开 cloud.siliconflow.cn → 进入「账号管理」→ 找到「实名认证」，验证通过后把刚才那步重跑一次即可。

**Q：往飞书里甩了个文件夹，AI 却说读不到**

锅在飞书——它没有直传目录的能力，你实际送出去的只是一条指向云盘的引用。想让它真的读到，先把这个目录打成 .zip 压缩包，再重新发送。

**Q：文件交上去，AI 半天没回音**

别慌，这在预期之内。光是解压缩、切分文本、生成执行脚本就得耗时间，体量大时熬个十到三十分钟也很常见。安静等它跑完就好，切忌连续催问、把流程打断。

**Q：问答给出的答案不够准**

无非这么几种缘故：

• **库里存货太薄**：只塞了几篇东西，检索效果自然比料足时差一截。建议起码凑够十篇以上。

• **问题问得太笼统**：把范围收窄会更有效。比如“商业策略”这种说法太大，换成“初创公司预算紧张时怎么做品牌定位”，指向性立刻不同。

**Q：我存进知识库的东西会不会跑到云端去**

不会。文本与向量两类数据都落在你自己的服务器磁盘上。唯一一次与外界打交道，是请求 Embedding API 完成“文本→向量”的换算，而且送出去的只是五百字上下的一小段切片，绝不是整份文档。

**最后说两句**

动手搭这套东西之前，那些翻过的书、存下来的长文，彼此毫无关联地躺在各个角落，像一地散沙。你清楚记得某处见过一句很对味的话，偏就是想不起来它躺在哪。

一旦跑通，散沙就被编成了一张网：每份资料是网上的一枚结点，而每一次发问，都可能牵出一条你自己都没料到的通路。

也许某天你顺口提了个疑问，系统却能从三个月前归档的一篇旧文里拎出一段话，正巧撞上你当天脑子里盘旋的念头。

那一刻你大概会意识到，学习这件事在 AI 时代已经被重新定义了。

![](img/29a5f8702673f247cdf1035fc6c5a14d.png)

## 2. 用 OpenClaw 打通个人 IP 👸号自动发布

**提醒一句：这一例难度不小。针对「打造专属知识库」与「个人 IP 👸号自动化」两项，二者择其一做完即可（刚上手的话，建议先拿下前一个），剩下的当加餐，没必要全啃。二十一天周期内，只要能跑通其中任何一个 OpenClaw 案例，就已经算赚到了。**

生成式模型替你写稿，最容易出问题的地方并非文笔粗糙。情况正好颠倒：它写得太周正了。每个句子都挑不出毛病，篇章骨架永远四平八稳，语法层面从不失手，以致你通读一遍只会冒出一个念头——标准答案。

但你经营的是个人 IP。

往👸号里发文，本质不是按时交一份作业。别人点下关注，图的是你讲话那股跟旁人不同的劲儿。他们惦记的，是你独有的偏爱、你的腔调、你偶尔冒出来的坏情绪——而非一份机器产出、无可指摘的文本。

以下内容只解决一个命题：如何让机器产出的文字染上你的气味。

**前提**

：手上得有一个能正常运转的 OpenClaw 环境（若尚未准备，请先翻阅部署相关篇章）。

💡两种节奏，挑一种适合你的

教程篇幅不短，但真不需要一次做完。看你的时间，选一条路走：

**快速路线（半小时左右，先把主链路跑通）**

：只做 Step 1 里的 1.1 至 1.3，迅速整出一份风格设定 → 借它写篇短文检验成果 → 存进草稿箱。半小时内，👸号后台的草稿里就会躺着一篇带着你个人色彩的 AI 稿件。先尝到味道，再判断要不要往深处做。

**完整路线（约三小时，全流程打通）**

：自 Step 1 一路做到 Step 6，素材收集、配图、定时推送都包含在内——每个环节都亲手过一遍，形成一条天天可用、持续转动的生产链。

我的建议：先跑快速路线，尝出甜头再回来补齐。

**动工前的核对**

开工以前，先把下面这几项点清楚。免得走到 Step 2 才察觉连不上网，那滋味可不好受。

![](img/28b9b3b6150a2e137f0ad28b021b311e.png)

**运行逻辑**

一句话就能串起来：

Plain Text

```
素材采集（Tavily + MediaCrawler）→ 风格化写作（三层架构）→ 配图（封面+内文）→ 排版（HTML）→ 发布（草稿箱）
```

整条链路的关键，全落在居中那个环节上。换个说法可能更好懂：

假设你请了一位笔力极强、却毫无个人棱角的影子写手，那么交到他手里的必须是三样东西——

• **第一层 · 风格指南**：交代清楚你是怎样一个人：惯用哪些词、说话什么调门、段落长短怎么排

• **第二层 · 范文样本**：把你满意的旧作摆到他面前，用作品说话，而不是靠嘴描述风格

• **第三层 · 禁忌清单**：划定你的语言禁区，像“综上所述”“让我们深入探讨”这类腔调，你从来不碰

三层都喂进去以后，连发十篇出去，朋友恐怕都辨不出哪篇出自机器。

详细的架构图示与 Skill 清单都收在文末附录里，此刻先别分心去翻，动手更要紧。

**搭建流程一览**

![](img/6440f6a87e5a5fb36b5736e1310c0a5d.png)

整体耗时：初次配置约三小时；此后每篇稿件十到十五分钟

Step 1：先立起属于你的风格档案

【声明】

本教程拿咪蒙已公开发表的作品当示范样本，只因她行文的个人印记格外鲜明，三层设定拉开的效果差距一眼就能看清。**这并不等于认同她的创作取向。**文中演示的是一套“让模型习得某种文风”的手法；至于你选择哪种笔调、秉持怎样的价值立场，全凭自己。切勿套用他人的风格设定去冒名发文。真正给自己建档案时，务必用你本人的材料。

余下五个步骤合计一小时；而这一关，或许就要耗掉你两小时。

可一旦省掉这两小时，后面那一小时只会让你更快、更批量地产出机器垃圾。

[

![](img/598d568199b01bc40ea3ff6ff959bbf0.png)

咪蒙文章.txt](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/VOhxbkXq1olNODxZjRTc4fT1nRg?response-content-disposition=attachment%3B%20filename%3D%22%E5%92%AA%E8%92%99%E6%96%87%E7%AB%A0.txt%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260527%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260527T011932Z&x-oss-expires=86400&x-oss-signature=26fba0d85ed179ff3a083434de74977458f99ab33c23d246b32e4573009c8a57&x-oss-signature-version=OSS4-HMAC-SHA256)

[

![](img/e29a45250032ccdfaad1d9727c10264c.png)

咪蒙精选30篇.md](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/MaAbbYnCpoKkhCxEqQ7cSDqvnkh?response-content-disposition=attachment%3B%20filename%3D%22%E5%92%AA%E8%92%99%E7%B2%BE%E9%80%8930%E7%AF%87.md%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260527%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260527T011932Z&x-oss-expires=86400&x-oss-signature=2b4961774ff8ab3412feff5272e2e8c9ac9c7cd426279276b7929515639d2d46&x-oss-signature-version=OSS4-HMAC-SHA256)

[

![](img/bf667c5a3777b5121790431a3f74336c.png)

咪蒙风格DNA分析报告.md](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/SOGmbp0WHoJ8NFx05fZc4NKxnUg?response-content-disposition=attachment%3B%20filename%3D%22%E5%92%AA%E8%92%99%E9%A3%8E%E6%A0%BCDNA%E5%88%86%E6%9E%90%E6%8A%A5%E5%91%8A.md%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260527%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260527T011932Z&x-oss-expires=86400&x-oss-signature=1a3100a3dbe81a4de096fd654b846a7bc12d0a2893c418d0d7434eb5fa28f4ca&x-oss-signature-version=OSS4-HMAC-SHA256)

1.1 攒起属于你的语料

回想一下你在群里敲字的时刻：并非敷衍地回个“收到”或“好的”，而是忽然来了话头、一口气敲出三百来字——那种状态，才是你本来的笔调。

不少人都略过这环。他们习惯在提示词里塞一句“口吻轻松点、幽默点”，转头又埋怨产出不像本人。可你压根没把“自己长什么样”交代给它，凭什么要求它模仿你？

**该准备的语料**（越多越准，底线十篇）：

• **旧文存档**：此前发布过的👸号推文、博客、朋友圈长文

• **聊天留痕**：群聊里那些成段的长回复（你肯认真敲字的那种）

• **语音转写稿**：语音日记、会议发言、播客录音均可

• **讲稿与 PPT 备注**：你在公开场合开口讲过的内容

全部归拢到一个目录里：

Plain Text

```
# 在 OpenClaw 中说：
帮我创建一个文件夹 ~/Documents/我的风格语料库，用来存放我的写作素材
```

再把上述材料逐篇存进去，一份文档对应一个 .md 或 .txt 文件。

验证：

Plain Text

```
# 在 OpenClaw 中说：
帮我看看 ~/Documents/我的风格语料库 目录下有多少个文件
# 输出应该 &gt;= 10，少于 10 篇效果会打折扣
```

**手头实在没有旧作怎么办？**

挑五个你真正在意的话题，安安静静手写五篇五百字往上的东西。不必排版，也无须打磨，脑子里蹦出什么写什么——落纸的正是你自己。

案例走查：公开人物语料的采集与清洗（拿咪蒙练手）

若你想先借一位风格突出的公众人物练练手，采集可以按下面几步走：

**第一步：锁定素材出处**

知名作者的旧文，常有人义务整理成合集流传（PDF、TXT 或网盘链接）。我们手上这份咪蒙合集便是一份十三万八千行的 txt，装了九百多篇文章。

其余可取之处：

• 🧣长文（手工摘录，或者用 MediaCrawler 批量抓）

• 演讲录像（先下载，再用 mlx-whisper 转成文字稿）

• 电子书（🛰️读书、Kindle 之类）

• 知乎与博客上的历年文章

**第二步：挑出代表作**

这类合集往往鱼龙混杂，广告稿、团队成员捉刀、带货文、凑数水文都在里面。你要留下的是署名本人、最能显出个人笔法的纯观点文章。

我们的过滤条件：

• 仅取署名本人的篇目，团队他人所写一律剔除

• 仅取观点、情感、社会评论类；广告篇幅过半的软文不收

• 题材尽量铺开（情感、职场、社会话题、自我成长等）

• 最后落下三十篇

这一步在 OpenClaw 里可以整个交给模型代劳：

Plain Text

```
请读取 ~/Documents/咪蒙合集.txt，从中筛选出 30 篇最能代表咪蒙写作风格的纯观点文章。
筛选标准：必须是咪蒙本人署名，不是带货软文，覆盖不同主题。
保存到 ~/Documents/我的风格语料库/咪蒙精选30篇.md
```

**第三步：洗掉噪音**

网友整理的版本常夹着私货：整理者自己的👸号二维码、联系方式、小广告。这些一律清掉：

• 抹去整理者署名与水印（像“WCplus”“数据部落”这类）

• 清空淘口令（￥…￥）

• 删掉图片占位标记（《《 向左滑动查看图片 》》）

• 末几段若忽然转成商品推销，就截到观点收束处为止

清洗完毕后，这三十篇约九万字，便是你的分析底本。

1.2 拆解你的笔法基因

材料备齐，下一步就是让模型把你的笔法译成它读得懂的描述。

开口只说一句：

Plain Text

```
请读取我接下来发你的所有文章，按照以下维度分析我的写作风格 DNA：
```

紧接着把这套分析框架贴上去。它不只盯着句子形态，还追问思路如何推进——整体调性、偏好的洞察角度、惯用的表达招法、句长与节奏，一并拆开看：

Plain Text

```
请分析我语料库中的文章的写作风格 DNA，从以下维度输出结构化报告：

【调性】
- 整体气质（亲切/犀利/幽默/冷峻/学究/江湖/文艺...）
- 与读者的关系（平等聊天/导师指点/朋友吐槽/专家科普...）

【洞察偏好】
- 偏好&quot;说破型&quot;洞察（说出大家想说但没说出的话）还是&quot;看透型&quot;洞察（揭示大家没意识到的真相）？
- 给出 3 个原文例句佐证

【五个表达招数】
- 把大变小（从宏观缩到具体）的使用频率和典型例句
- 把远变近（建立相关性）的使用频率和典型例句
- 把抽象变具体（用场景/数字/故事）的使用频率和典型例句
- 把复杂变简单（删减/直白）的使用频率和典型例句
- 把平淡变精彩（反差/角色互换/意外）的使用频率和典型例句

【句式节奏】
- 平均句长（短促有力 vs 长句绵密）
- 标志性句式（排比？反问？自嘲？设问？）
- 段落长度和换行习惯

【用词指纹】
- 口语化程度（1-10）
- 是否混用英文/网络用语/成语
- 高频口头禅或标志性用词
- 绝对不会用的词（例：综上所述、不是X而是Y）

【观点表达方式】
- 如何提出观点（直述/先讲故事/先提问/先否定常见看法...）
- 如何论证（摆数据/讲案例/用比喻/引用权威...）
- 如何收尾（总结/反问/留悬念/行动号召...）
```

合格的报告必须落到原文句子作例证，不能只给空泛评语。若通篇都是“您的文风轻松幽默”这类套话，通常意味着语料量不够或材料过于雷同，请补料后重跑。

1.3 产出三层风格配置

分析跑完，把结论落成三份文档。

**第一份：**风格指南.md（第一层 · System Prompt）

Markdown

```
# [你的名字] 的写作风格指南

## 角色定位
[从分析报告中提取]

## 调性
[从分析报告中提取]

## 句式规则
- [规则1]
- [规则2]
...

## 用词偏好
- 偏好：[词语列表]
- 禁用：[词语列表]

## 段落节奏
[从分析报告中提取]

## 观点表达方式
[从分析报告中提取]
```

**第二份：**范文样本.md（第二层 · Few-Shot）

从语料里挑三到五篇最能立住你形象的作品，整篇放进去。

挑选时的尺子：

• 你自己读完要觉得“这就是我”

• 体裁铺开（观点、叙事、干货各取一篇）

• 单篇不少于八百字（篇幅过短，模型摸不到你的句子律动）

**第三份：**负面约束.md（第三层 · Anti-Slop）

Markdown

```
# [你的名字] 绝对不会这样写

## 禁止句式
- 不是X，而是Y（AI最爱的句式）
- 综上所述 / 总而言之 / 让我们深入探讨
- 首先...其次...最后...（除非内容确实需要列举）
- 在当今社会 / 在这个快节奏的时代
- 值得注意的是 / 不可否认的是

## 禁止用词
- 赋能、抓手、闭环、打法（互联网黑话）
- 深度、维度、颗粒度（除非讨论技术问题）
- [从你的分析报告中补充]

## 禁止结构
- 全文只有观点没有故事/案例
- 每段都以转折词开头
- 结尾都是&quot;你怎么看？欢迎留言&quot;
```

第三层有个偷懒的路子，来自 Ruben Hassid：在 Wikipedia 上检索 “Signs of AI writing”，把那页内容整段复制，直接当你的禁忌底稿。他的说法是，模型真正需要的不是“你像什么”，而是“你永远不像什么”。在此基础上再并入你私人的黑名单，收效更佳。

**别幻想一遍就能定稿。**

风格设定全靠反复拧出来，没有一次性成型这回事。节奏大致如此：

1.  拿三层设定让它先产出一篇

2.  通读一遍，把“这句不像我”的地方逐处圈出

3.  回头修改指南里的描述或禁忌条目

4.  再产一篇，再比一轮

如此往复几轮，大约到第五次，产出就趋于稳定；跑到第十次上下，前后一致性甚至强过你亲笔所写——人会受情绪起伏影响，它不会。

若觉得一轮轮手调太熬人，可以试个开源工具 cw-style-skill-creator（仓库 haowjy/creative-writing-skills）：它能自行从你的语料里提炼风格说明，并产出 Claude Skill，省去大量反复折腾的功夫。

核对：三份文档是否都已落盘？

Plain Text

```
# 在 OpenClaw 中说：
帮我确认 ~/Documents/我的风格语料库/ 目录下是否有这三个文件：风格指南.md、范文样本.md、负面约束.md
```

1.4 案例走查：咪蒙的三层配置

为了让你亲眼看见三层结构能拉开多大差距，我们拿她这三十篇代表作做一次完整走查。她的笔触太有辨识度，改动前后的对照格外扎眼。等你建自己的档案时，把这套做法换到你身上即可。

**第一层示范：咪蒙的风格设定**：Markdown

```
# 咪蒙写作风格指南

## 角色定位
一个敢说真话的泼辣闺蜜。有文化底蕴但绝不卖弄，用最口语化的方式输出最犀利的判断。
替读者说出他们想说但没说出的话。

## 调性
犀利毒舌 + 闺蜜式亲切 + 自嘲式幽默，三层叠加。
像一个说话不留情面但你觉得她在帮你的损友。
绝不居高临下——先暴露自己的缺陷或糗事，再输出观点。

## 洞察偏好
偏好&quot;说破型&quot;洞察——不是告诉读者不知道的真相，而是替读者说出知道但说不出的话。
- 例：&quot;你以为你站的是蒋劲夫吗？你站的家暴本身。&quot;
- 例：&quot;我把你当老公，你把我当子宫。&quot;
- 例：&quot;&#x27;你负责赚钱养家，我负责貌美如花&#x27;就是&#x27;大家好，我正在卖身&#x27;的委婉说法。&quot;

## 句式规则

- 极短句为主，10 字以内的断句大量使用
- 一句话一段是常态，强调句必须独占一行
- 排比递进到荒谬——每一条比前一条更极端，制造滑坡式喜剧效果
- 反问句在论述高潮处密集出现，制造压迫感
- 括号内心独白——叙述中插入括号放吐槽/补充/反差评论
- 自嘲+转折是标志结构——先自损再输出观点

## 用词偏好
- 口语化程度 9/10，接近说话状态
- 高频语气词：&quot;特么&quot;&quot;老子&quot;&quot;好吗&quot;&quot;哦漏&quot;&quot;简直&quot;&quot;真的&quot;
- 脏字是节奏工具不是泄愤：&quot;傻逼&quot;&quot;卧槽&quot;&quot;妈蛋&quot;&quot;日了狗了&quot;
- 程度副词密集：&quot;太XX了&quot;&quot;简直&quot;&quot;真的&quot;
- 禁用：学术连接词、官方体、鸡汤套话、文艺腔修饰

## 段落节奏
- 段落极短，大量单句成段
- 一个观点拆成 3-5 个短段，每段只有一两句话
- 视觉上留白极多，阅读节奏极快
- 节奏型号：&quot;短-短-短-稍长-短&quot;

## 观点表达方式
- 开头：新闻事件或身边故事切入，绝不直接说观点
- 论证：故事驱动（自己经历 + 粉丝投稿 + 采访案例），每个论点至少配 1 个具体故事
- 收尾三种模式：金句钉死 / 情感号召 / PS 彩蛋式自嘲
- 全文节奏：&quot;升温-爆发-缓冲-再升温-再爆发&quot;的波浪式推进
```

# 第二层：把范文喂给AI当语感教材

三层配置里，第二层解决的是“AI没见过好东西”这个问题。从三十篇里拎出三篇代表作——社会评论一篇、情感一篇、自嘲幽默一篇：《你支持的不是蒋劲夫，是家暴！》《我把你当老公，你把我当子宫》《我，一个矮子的史诗》。注意，不是挑几句漂亮话放进去，是把全文原封不动塞进配置文件，让模型从整体上感受那种节奏和口气。至于第三层，管的是“禁区”，用Markdown把“什么写法不要碰”一条条钉死。

```
# 咪蒙绝对不会这样写

## 禁止句式
- &quot;在当今XX的时代...&quot;（太官方，咪蒙永远从具体事件/故事开头）
- &quot;首先...其次...最后...&quot;（AI八股，咪蒙用故事推进不用列举）
- &quot;值得注意的是&quot;（学术腔，咪蒙会说&quot;说白了&quot;或直接骂）
- &quot;希望本文对你有所帮助&quot;（太客气，咪蒙不会这么温和收尾）
- &quot;让我们深入探讨&quot;（咪蒙会说&quot;来，老子跟你掰扯掰扯&quot;）

## 禁止用词
- 学术连接词：综上所述、由此可见、与此同时、据此推断
- 官方体：据悉、据了解、笔者认为、不可否认
- 鸡汤套话：岁月静好、不忘初心、砥砺前行、负重前行
- 文艺腔：氤氲、斑驳、温润如玉、浅浅的忧伤
- 互联网黑话：赋能、抓手、闭环、颗粒度

## 禁止调性
- 中立客观（咪蒙永远有鲜明立场，绝不&quot;一方面...另一方面...&quot;）
- 温和委婉（该骂就骂，该粗口就粗口，不要试图显得得体）
- 居高临下（先自嘲再输出，不要像导师在教训学生）
- 滴水不漏（要有情绪的粗糙感，太完美反而不像人写的）

## 禁止结构
- 全文纯说理没有故事（每个观点至少配一个具体场景）
- 开头是抽象论述（必须从事件/故事/场景切入）
- 全文情绪平稳没有爆发点（至少要有 2 个情绪高潮）
- 缺少自嘲或幽默调剂（沉重话题也要有释压点）
```

## 1.5 同一个题目，加不加配置差多远

光聊配置听上去很虚。直接上实验：话题就选“AI写的👸号为什么让人读不下去”。不给任何风格信号，模型的输出你大概能猜到——先交代时代大背景，然后“第一、第二、第三”平铺直叙，中间插一句“需要引起重视”，收尾对读者表达祝愿。每句话都挑不出毛病，每句话也都记不住。毛病出在哪儿？根子上就三件事：模型没有你那些经历和感受；你也没告诉它该用什么调子说话；再加上模型天生挑安全牌打。所以不是AI能不能写的问题，是你怎幺带它上路的问题。

换成带三层配置的版本，同样的模型同样的题目，出来的文字像换了个人执笔：

有个做👸号的哥们儿，砸三千块买了套“AI自动成稿”工具，号称十分钟出货。他把十篇成品甩我面前。我扫了一遍——十篇读着像同一个人在同一天写的：开场白一个句式，论证一个套路，过渡一个词，收尾一句吉祥话。我跟他说，你这不是写文章，你这是让AI玩巨型完形填空。他还挺得意，说排版都自动搞好了。我当时就想回一句：摆盘摆成米其林又怎样，食材本身不行，端上桌照样没人动筷子。

AI写作真正吓人的地方，不是差，是“对”得没边儿。没棱角、没火气、没那句只属于你的口头禅。读者愿意蹲你，是想听你拍桌子说“这什么破事儿”，不是看你端端正正写“此现象需审慎对待”。前一种是AI交差，后一种才是有血有肉的人在跟你唠。短句、大白话、自黑、括号里夹点心里话、打比方别飘——三层配置就是往这个方向使劲。

## 1.6 小试牛刀

迈入Step 2之前，拿刚搭好的三层配置热个身。在OpenClaw里扔一个你最近上心的题目：

```
请读取 ~/Documents/我的风格语料库/ 下的风格指南.md、范文样本.md 和负面约束.md，然后用这个风格写一段 200 字的短文，主题是&quot;为什么大部分人学不会 AI&quot;
```

题目随意换，写你真正想聊的。生成之后先别急着发，问自己一件事：把这段文字丢进朋友圈，你朋友能看出来这不是你写的吗？能看出来，就折回1.2改风格指南，再测。一般来说折腾两三轮很正常，别嫌烦。要是看着差不多了，风格这关就算过了。

我个人的手感：光有风格指南，出来的东西六成像我；搭上范文，能到八成；再把负面约束加进去，九成往上；最后一成靠发之前自己动手捋一遍。三层里抽掉任何一层，效果都会肉眼可见地往下掉。

![](img/8b0bd0db016b6bd7afc102a3d0fdfb88.png)

## Step 2：让AI长出一双会找料的眼睛

写作最头疼的从来不是写砸了，是打开文档不知道敲什么。这一步干的不是洗稿的活儿，是帮你建一套“自动逛菜场”的机制——每天睁眼，桌上一份刚摘的选题，你只管挑。挑完回家自己做菜，菜是你自己的。

### 2.1 入门版：三分钟搞定，够用了（新手推荐）

只需要一件工具：Tavily Search。说白了就是给AI配的搜索引擎，一个API Key就能扫全网，OpenClaw圈子里人手一个。

第一步，去tavily.com开个号，把Key复制出来。完全免费，不用绑卡，注册就送每月一千次查询额度。日更的号一天查个三五回，一个月拢共百来次，绰绰有余。要是网络卡壳拿不到Key，直接跳过也不碍事——2.2节要讲的MediaCrawler不靠任何Key，国内平台的内容它直接就能扒。Tavily属于锦上添花，MediaCrawler才是压舱石。

第二步，在OpenClaw对话框里敲：

```
帮我安装 Tavily 搜索工具，API Key 是 xxxxxxxxxxxxx(填写你的key)
```

![](img/89b28dc564f63b8dab03be47cba9728f.png)

![](img/a04da62044f9f689241e1cfdfb54f296.png)

第三步，跑个测试：

```
# 在 OpenClaw 中说：
帮我搜索一下最近一周&quot;公众号自动化&quot;相关的热门讨论，重点看用户的痛点和吐槽
```

等几秒，全网的公开讨论、帖子、文章会被归拢成一份结构化摘要，这就是你接下来要用的原料。

![](img/d9ab905860df64e496484483b3a696a5.png)

![](img/0e1d59d073128f866dd0a7a02f4f8916.png)

说到底Tavily干的是网页搜索的活儿，只能碰到被搜索引擎收录的公开页面；📕留言区、B站弹幕这种犄角旮旯，它够不着。但用来找方向、扒素材，已经绰绰有余。先把链路跑通比追求平台全覆盖重要一百倍。

![](img/fdc4f94af2ee3d991ee6956bce7b35cc.png)

### 2.2 进阶版：MediaCrawler深挖国内平台（推荐）

Tavily能捞公开页，可📕评论区、B站弹幕、🧣热评这些东西，搜索引擎压根没收录。你得有个能钻进去掏评论的家伙什。MediaCrawler是眼下最热的开源社交平台采集器，GitHub上四万三千多颗星，一套家伙覆盖七个国内主流平台：

![](img/a1d7f9559da94b3b3a6a58aed06ffe4b.png)

不用每个都登录。手头有哪个平台的号就登哪个。📕、B站、🧣三个凑齐已经非常够使，剩下的属于添头。

为啥选它？一套工具通吃国内平台，不用挨个装插件；评论抓取是看家本领，评论区才是真金白银，这正好补上Tavily够不着的地方；底层是Playwright，扔在VPS上无头跑毫无压力；自带WebUI，第一次扫码在网页上就能完成，不用折腾远程桌面；开源不要钱，API Key一个都不用，月成本零。

搭建分四步：

第一步，装。在OpenClaw里说：

```
帮我安装 MediaCrawler（GitHub: NanmiCoder/MediaCrawler），用 Python 环境装好，并安装 Playwright 浏览器
```

![](img/6eb9eacefea5636d3a7fd0308dfc8840.png)

第二步，起WebUI。在OpenClaw里说：

```
帮我启动 MediaCrawler 的 WebUI 界面
```

起来之后，拿手机或电脑浏览器打开http://你的VPS的IP:8080，操作界面就出来了。

![](img/27a78d5ba68912091c03bb44d34c5724.png)

第三步，登录平台，一次就够。在WebUI里点你要登的平台，比如📕，会蹦出个二维码，拿对应App扫一下。

![](img/3b1c457afb1eb1715f42a8a19363dcb9.png)

![](img/b12eef58f65c40335cba3c1798e23404.png)

![](img/ce00bac5f0211b2b84531b959cffb603.png)

扫完登录成功，Cookie会自动存在服务器上。往后采集都复用这个登录态，不用反复扫码，一般撑几周甚至几个月才需要重来一回。

第四步，试采一次。在OpenClaw里跑：

```
# 在 OpenClaw 中说：
帮我用 MediaCrawler 搜索小红书上&quot;公众号自动化&quot;相关的笔记，抓取前 10 条笔记和评论
```

![](img/7ca46e5595a0c1cb91ccb1dfd44a4954.png)

![](img/247a5d7378b4b8b08b32707c9af95749.png)

![](img/e635aabcf0f374294838a90b8d467638.png)

Tavily和它怎么打配合？Tavily负责撒网——搜全网，看哪些话题正在冒泡；MediaCrawler负责下钩——钻进具体平台，把评论区原话一条条捞上来。打个比方：Tavily发现不少人在抱怨👸号AI稿子没人味儿，你就让MediaCrawler去📕和B站搜这个话题，把真实吐槽一网打尽——“全是四点”“没有人味儿”“内容屠宰场缺我这把刀吗”——这些原话往文章里一搁，比AI编的“据某用户反映”有说服力一百倍。

只用Tavily也成，找选题够使。但你要想让论据出自真人嘴里，MediaCrawler就是你的弹药库。

注意事项：

![](img/38ab46abb9f05c7f12fbeea0421f1c9e.png)

海外平台咋办？MediaCrawler管的是国内。要采X、Reddit、YouTube这些，Tavily的搜索结果一般够用。绝大多数👸号作者的读者和素材都在国内，先把国内这摊子支棱起来再说。

入门版加进阶版：一个API Key加一个开源工具，月成本零，能搜全网也能深扒七个国内主流平台的评论区，覆盖九成五的选题场景。

### 2.3 从信号到选题再到文章

甭管你用的是入门版还是进阶版，采回来的素材都不能直接往文章里怼，中间得转一道手：

```
搜索结果（信号）→ 你的观点（选题）→ 文章骨架（大纲）→ 完整文章
```

拿个例子走一遍：

信号：MediaCrawler在📕扫到一条笔记，底下有人留言“用了三个自动化工具，生成的文章全是AI味，改了一下午还不如自己写”，这条评论攒了三百二十八个赞。

选题：👸号自动化工具都在解决一个伪命题——它们让你发得更快，但没人帮你发出来像你亲手写的东西。

大纲：拿Step 1定好的风格指南，把选题撑成骨架。

文章：到Step 3用风格化写作流水线生成。

留意第一步到第二步这个跳跃：信号是别人的经历，选题是你的立场。你不是在当传声筒，你是从别人的话里拎出你自己认的那根筋，然后用你的路数把它论证出来。

弄完之后验一下两个工具。

验Tavily：

```
# 在 OpenClaw 中说：
帮我搜索一下最近关于&quot;AI写作 个人IP&quot;的讨论，找出用户最大的痛点是什么
```

![](img/e71c4eb272845b069b5247000501d4d8.png)

验MediaCrawler：

```
# 在 OpenClaw 中说：
帮我用 MediaCrawler 搜索 B 站上&quot;AI写作&quot;相关的视频，抓取前 5 条视频标题和播放量
```

![](img/df2b87c6e3871bd1f0e3ee0e62dc474e.png)

你应该能看到：Tavily正常吐回标题、摘要、来源链接；MediaCrawler能搜平台并带回内容和评论；你至少能从结果里扒拉出一个选题。这三点齐了，素材采集这摊就算搭成了。往后每次动笔前，Tavily探方向，MediaCrawler掏原话。

![](img/aee486072f5fb1f191d40602c535c8de.png)

## Step 3：风格化写作流水线

核心理念：去AI味不是等稿子出来再返工，是从落第一个字起就带着你的基因。📕上那些去AI味教程，翻来覆去就一招——先让AI整一篇，再回头换措辞、塞口语、拆结构。这跟做砸了一锅菜再猛倒调料有什么区别？调料倒得再凶，底味该不对还是不对。正路是：从挑食材那一步就照你的口味来。

### 3.1 把三层配置焊进写作流程

你手上现在攥着三个文件：风格指南.md（打头那层）、范文样本.md（第二层）、负面约束.md（压轴那层）。接下来要干的是把它们塞进写作流程，让AI每次动笔都自动翻到。在OpenClaw里，你可以打包成一个Skill，也可以搁项目目录里当参考文件。两条路都通，但我更推前一条：做成Skill之后省得每回手动贴，AI自己会去翻。

推荐做法：打包成Skill。在OpenClaw里说：

```
帮我创建一个写作风格 Skill，目录是 ~/.claude/skills/my-writing-style，
把 ~/Documents/我的风格语料库/ 下的风格指南.md、范文样本.md、负面约束.md 合并成一个 SKILL.md 放进去
```

验一下：

```
# 在 OpenClaw 中说：
帮我确认 ~/.claude/skills/my-writing-style/SKILL.md 文件是否存在
```

### 3.2 文章生成流程

一篇稿子从选题到定稿，从头到尾走一趟大概长这样：

第一步：定题，备料

动手前先把两件事落定：写什么，以及凭什么写。这一步不费脑子，工具每天会把可写的题和可用的料打包成一份报告，开机就能读到。

```
# 在 OpenClaw 中说：
写一篇关于&quot;为什么大部分公众号自动化工具都在解决错误的问题&quot;的文章。

参考素材：
- [粘贴从 Tavily/MediaCrawler 采集到的相关信号和用户原话]
```

![](img/12b4f6d7db937a46f0c74375de38d2a7.png)

第二步：拿甲方的劲儿审提纲

AI 会照着你的文风档案先拉一版提纲。别一看就点头，这是最该较真的地方。骨架歪了，后面字句修得再亮，也只是给人看的外壳。

审的时候盯三处：

结构合不合你的路数
你落笔的习惯是先抛故事再收观点，还是开门就给结论？提纲得贴着你这个习惯走。假设你向来第一段就亮刀，提纲却让你铺三层垫子才进正题，退回重做，不用犹豫。

开场有没有烂梗
假如第一行写着"当下 AI 浪潮席卷……"或者"伴随 XX 的高速演进……"，别客气，退回。换成你自己写，会这么起头吗？不会，那就别让机器这么干。

证据是采来的还是编的
每条支撑都得能对上原始材料。上一步用 Tavily 和 MediaCrawler 扒下来的用户原声、留言、数据，才是可用的弹药。机器自己造的"调查表明""专家指出"，一律砍掉。少一条真证据，好过多一条假证据。

第三步：一节一节地出稿

千万别让它一次交全篇，那样腔调十有八九会飘。按提纲分节生成，每节收笔就停下来比对：语气、节奏、用词，还像不像你。

第四步：通篇调成一个味儿

初稿齐了，得整体过一遍。可以交给脚本跑，也可以自己一段段读。

```
请对比这篇文章和我的风格指南，检查以下维度：
1. 是否有负面约束清单中的禁止句式出现？
2. 句式节奏是否符合风格指南描述？
3. 口语化程度是否匹配？
4. 观点表达方式是否一致？

如果发现不一致，请标注具体位置并修改。
```

![](img/42132430358bb048a0b6610e9e4eb4f3.png)

3.3 十篇文章要像一个人写的

不只是单篇内部要稳，连续十篇推出去，读者也该认得出是同一个人。这比写好一篇更难，分量也更重——个人 IP 的地基就压在这上面。

三条落点：

第一条：把开场姿态固定下来

每篇都用同一种进场方式。不是每句都写成一样，而是切入的路数保持一致。好比有人推门前先敲两下，有人抬脚就踹，你的开场就是你的进门动作。

几种现成路子，照着挑：

• 罗永浩式：拿一个反常识的事实开场，或者迎着流行看法顶上去。比如"我最近把 XX 试了一圈，结果挺扫兴。"一落笔就有火药味。

• 半佛仙人式：用离奇的类比或黑色幽默切进去。比如"XX 要算一道菜，那就是把整排调料倒进锅，然后宣布这叫融合。"先让人乐，再让人琢磨。

• 和菜头式：从一件私人的小事起步，忽然拉到大议题。比如"下午在街角咖啡店坐着，隔壁两人在聊 XX……"画面立起来，距离也消了。

第二条：把收尾方式定下来

结尾也得有统一的退场姿势：

• 罗永浩式：绕回理想主义，或甩一句短促的判断。

• 半佛仙人式：把开篇那个荒诞比方收回来，意思却翻个个儿。

• 和菜头式：回到那个私密安静的场景，只是读完之后，心境已经不同。

第三条：养几句自己的口头禅

有意识地在每篇里反复放几个辨识度高的词。罗永浩的"认真""理想主义""彪悍"，半佛仙人的"朋友们""硬核""离谱"，和菜头的"世事如此""且如此这般"——读者瞄见这些字眼，立刻知道是谁写的。

反面例子：头一篇用"我"起头、口语、讲自己的经历；第二篇改成"近年来……"起头、书面腔、通篇讲道理——读者会觉得换人了。这种断裂很伤信任。

3.4 给表达提味：五个招

稿子写完，还有一个可选但很值得做的动作：拿五招再刷一遍，把平的地方磨出锋。

自己逐条对，也可以交给 AI 代劳：

```
# 在 OpenClaw 中说：
帮我用&quot;五个招数&quot;优化这篇文章的表达：把大变小、把远变近、把抽象变具体、把复杂变简单、把平淡变精彩。
```

五招是：

• 大化小：宏观判断压到具体问题上。"AI 在重塑世界"不如"AI 每天替你省出两小时"。

• 远拉近：抽象技术拽回读者身边。"分布式架构"不如"你的服务器快撑不住了怎么办"。

• 虚变实：用数字、案例、场景替掉概念。"性能好了不少"不如"从 8 秒压到 0.5 秒"。

• 繁化简：删掉形容词和行话。大白话能讲清的，别用术语。

• 平出彩：加对照、反差、意外角度。"这个办法还行"不如"这办法让我删掉了 300 行旧代码"。

验证：请朋友当裁判

拿你的文风配置写一篇完整测试稿（1500-2000 字），然后做几件事：

1. 发给朋友，一个字不提示，只问："你觉得这像机器写的吗？"他的第一反应比任何检测器都灵。

2. 把这篇和你从前手写的稿子并排看，风格齐不齐？如果连你都摇头说"这不像我"，回第一步重调文风档案，别将就。

3. 全文搜一遍禁用词表。"综上所述""让我们深入探讨""在当今时代"——一个都不该冒头。

4. 有条件就跑一次朱雀 AI 检测，目标压到 30% 以内。

微练习：现在就能做。随手挑一个你最近关心的题，用你的文风配置让 AI 写 200-300 字的开头。写完自己动笔改——哪些句子不像你说的，就换成你平时会讲的。改完把两版摆在一起看，差得越多，说明你的文风档案还得补。这练习十分钟收工，但能让你对手感有更清楚的体会。

![](img/097a1d9840086b4695126095d028b300.png)

Step 4：配图交给自动化

baoyu 系列 Skills 说明

Step 4 与 Step 5 里用到的 baoyu-cover-image、baoyu-article-illustrator、baoyu-image-gen、baoyu-markdown-to-html、baoyu-post-to-wechat 等，需要先装。在 OpenClaw 里说一句"帮我安装 baoyu 系列 Skills"即可。若你部署的是完整版，这些通常已经带上了。

你刷👸号的时候，遇没遇到过满屏全是字的长文？连着划几屏，拇指就开始不自觉加速——不是内容差，是眼睛乏了。一张图，就能把手指摁住。

插图在👸号里承担两个完全不同的活儿，多数人只看见头一个，漏了后一个：

头一个：正文里的呼吸口。
一篇三千字的稿子，每八九百到一千字该放一张。不为美观，为让读者的眼睛喘口气。缺了这个节拍，人滑到第三屏就走了。

后一个：封面是你在信息流里的视觉签名。
这个更要紧，也更容易被放过。读者刷朋友圈一秒能掠过两三条，你只有 0.3 秒让他认出"这是你的"。靠的不是标题——标题根本来不及读。靠的是封面在色调、构图、质感上攒出的印象。所以封面风格定下来就别再动。

4.1 封面：先选套餐，能跑通就行

封面交给 baoyu-cover-image 这个 Skill。它留了 5 个维度可调，但头一回用不必全弄明白。先从下面三份套餐里挑一份，直接开跑：

选好之后，一句指令就够：

```
# 在 OpenClaw 中说：
给这篇文章生成封面图，用 cool 配色 + digital 渲染 + minimal 构图
```

就这么回事。Skill 会自己读稿、提炼主题、生成对得上的封面。

![](img/bc997df76fa68c4118338c18ede60dff.png)

怎么挑？看内容类型。科技、效率、AI 方向选"科技极简"，文化、生活方向选"文艺手绘"，商业、职场方向选"商务专业"。拿不定主意就选科技极简——干净，不容易出错。

想自己调？
完整的 5 维参数表放在文末附录，等套餐跑顺了再翻也不迟。

产出
：封面落在 cover-image/{topic-slug}/cover.png，同时留一份 prompt 文件，方便回看这张图怎么来的，下次好微调。

打开 cover.png，过四道关：

1. 尺寸对吗？👸号封面推荐 2.35：1（900x383 或同比例）。

2. 是不是你选的那套风格？

3. 图上的字（如果有）看得清吗？

4. 缩到手机信息流那么大，主体还认得出来吗？这步最关键——读者看到的是小缩略图，不是原图。

4.2 正文插图

封面搞定，轮到正文里的图。自己一张张挑太累，让 AI 决定插在哪、插什么。

用 baoyu-article-illustrator 这个 Skill，盯两个维度。

流程全自动，你只管等：

1. 先拆文章结构，找出核心观点与段落分界。

2. 按段落长短定位置，大致每 800-1000 字一张。

3. 为每个位置写图片 prompt。

4. 调 baoyu-image-gen 出图。

5. 自动插回文章对应处。

实际操作：
```
# 在 OpenClaw 中说：
给这篇文章配内文插图，用 notion 风格
```

收工后核几项：

1. 数量合适吗？三千字三到四张。

2. 两图挨得太近没有？至少隔开 600 字。

3. 图和上下文对得上吗？不是随手放的装饰吧？

4. 全套风格统一吗？

![](img/3843774cae56b38bed5ce44a410d40be.png)

4.3 出图的后端

上面两个 Skill，底层都通过 baoyu-image-gen 出图。可以把它想成一个统一收银台——不管货从哪家供应商来，都走这一个口。

当前支持的供应商：

设定默认供应商：在 OpenClaw 里说"帮我把默认的图像生成供应商设为火山引擎的 Seedream"，设完以后每次出图不用再点名。

验证：
```
# 快速测试图像生成是否正常，在 OpenClaw 中说：
用 baoyu-image-gen 生成一张测试图：一只猫坐在电脑前写代码
```

30 秒内回一张图，说明后端通了。

![](img/54b6c3b8b009f2846901817d3f842647.png)

Step 5：排版与推送

👸号排版的本质不是好看，而是别让版式成为读者关掉页面的理由。

这不是故作高深。多数人排版翻车，不是不懂设计——是🛰️那套渲染引擎处处反着直觉来。你在电脑上拾掇得漂漂亮亮，一上手机：列表缩进散了、代码块挤成一坨、字号小得可怜。锅不在你，在🛰️。可读者不会去找🛰️算账，他们直接划走。

好消息是，这些雷 Skill 都替你排过了。你安心写 Markdown，🛰️那些反人类的规矩它来对付。

5.1 把 Markdown 变成👸号 HTML

👸号编辑器不认 Markdown。得先转成内联 CSS 的 HTML——也就是样式直接挂在每个标签上，而不是单放一份样式表，这样在👸号里才显示得正常。

这一步用 baoyu-markdown-to-html Skill，一句指令完事。

4 种预设主题：

实际操作：
```
# 在 OpenClaw 中说：
把这篇 Markdown 文章转成公众号 HTML，用 modern 主题
```

产出：
• 同目录下生成一个 .html 文件
• OpenClaw 会返回图片占位符列表（发布时自动换成图床 URL）

![](img/942d21ea1a80c28071f69c702341f440.png)

![](img/dbfd0c2640bf20158b5d0a91b12ec685.png)

![](img/2f3d9844bae628c5121bb623a5ebc0c4.png)

关键细节（🛰️那些反人类的坑，Skill 都填平了）：
![](img/c656cfd852641cbbd8072beac871ae34.png)

这些 Skill 都处理过了。但你后续要是手动改 HTML，记得别又踩回去。

拿到 HTML 后，快速扫一遍：

1. 打开生成的 .html，在浏览器里预览。

2. 字号看着舒服吗？

3. 列表显示正常吗？

4. 代码块换行正常吗？

5. 图片位置有占位符吗（发布时会替换）？

5.2 送进草稿箱

HTML 有了，最后一步——塞进👸号草稿箱。

用 baoyu-post-to-wechat Skill，建议走 API 方式（比浏览器自动化快十倍，也更稳）。

```
# 在 OpenClaw 中说：
把这篇文章发布到公众号草稿箱
```

密钥怎么拿：

登录 https://developers.weixin.qq.com/ ，在"开发密钥"点重置，弹窗里复制 AppID 与 AppSecret。

![](img/0821349083575306c9cd4a9abb5b9160.png)

![](img/24370d1c2872bbad30db1b7d2dd0a41e.png)

若密钥配好后发布提示 IP 不在白名单，去补一下：

登录 https://mp.weixin.qq.com/ ，进"设置与开发——安全中心——IP 白名单——去设置"，把提示的 IP 加进去。

![](img/cb08c004110e577fec3befe6a5ef03d7.png)

![](img/3981a493b5335d130cd977d54794968d.png)

背后的事你不用操心：Skill 先传图，再传文，最后在草稿箱里拼好，10-30 秒。

一个重要限制，必须知道：
![](img/92d2b3b6f1ce621fd5852d8c0f151d8e.png)

换句话说，AI 帮你走完 95%，最后那下"发布"得你自己按。这其实是好事——发之前多瞧一眼，少翻一次车。

5.3 发布前检查——最后再扫一眼

文章进了草稿箱，别急着点"发布"。两分钟检查，能躲掉不少尴尬：

• 拉到最底，看看结尾还在不在。长文容易被截，草稿箱里前面看着正常，最后三段却没了。

• 图片都正常吗？图床偶尔上传失败，会出裂图。碰上就重传一次，别带着裂图推出去。

• 重点：点"预览"，发到自己手机上亲眼过一遍。电脑上没毛病的版式，手机上可能字小、图大、行距挤。

• 封面没被裁掉吧？（2.35：1 最安全）

• 标题没被截吧？（👸号限 64 字符，超了会砍）

• 顺手查标点：英文冒号换中文冒号，弯引号换直引号。小事，但影响专业度。

经验之谈：手机端预览是最要紧的一步。务必发到手机上看完再推。我自己栽过好几回——电脑上心满意足，发出去手机一开，代码块压成一行，引用块左边框没了。能改，但推出去的稿子改不了。

验证

完整走一遍发布链路，确认通：

1. 备一篇测试用 Markdown，几百字足矣。

2. 转成 HTML：用 modern 主题把这篇文章转成👸号 HTML。

3. 发布到草稿箱：送进👸号草稿箱。

4. 打开 mp.weixin.qq.com，进"内容管理"找"草稿箱"，确认文章在。

```
mp.weixin.qq.com
```

最后确认四件事：

1. 文章躺在草稿箱里。

2. 排版正常，没乱码。

3. 配图都显示出来了。

4. 封面正确。

四项全过——你的"AI 写作 → 配图 → 排版 → 发布"链路就通了。往后每篇从选题到进草稿箱，10-15 分钟。

![](img/3450ca37710f644fbfcbd1636aab08a5.png)

Step 6：把日常运营钉成流程

三小时搭起来的系统，死活就在每天那五分钟上。

你肯定见过这种人：周末兴致上来搭了一套自动化，兴奋三天，之后再没打开过。系统没坏，是没人喂。下面几条 SOP，就是把"你得记着去跑"变成"它自己跑完，等你看"。

6.1 Heartbeat 定时跑

先把最机械的一步交给机器——每天自动收素材。早上开机，一份今日选题推荐已经安安静静摆在那儿。

在 OpenClaw 里说：

```
帮我设置一个每天早上 6 点自动执行的定时任务：
用 Tavily 搜索&quot;公众号自动化&quot;&quot;AI写作&quot;&quot;个人IP&quot;这几个关键词的最新讨论，
整理成今日选题推荐，保存到 ~/Documents/每日选题/ 目录下
```

配好之后，建议连跑三天确认稳定性——有些网络毛病，只有凌晨六点网络环境自动断开时才会现形。

6.2 IM 指令：想到就发

定时任务管住了每日采集，但偶尔你临时冒出个想法，想马上动笔。这时不必开终端、不必背命令——给 OpenClaw 甩一句话就行。

通过飞书/Telegram 发给 OpenClaw：

```
写一篇关于XXX的文章，发到公众号草稿箱
```

OpenClaw 会自己跑完整条流程：

1. 用 Tavily + MediaCrawler 收相关素材。

2. 按你的文风档案写稿。

3. 出封面和内文插图。

4. 转成👸号 HTML。

5. 送进草稿箱。

你只剩一件事：去草稿箱看一眼，然后按"发布"。

# 12分钟成稿，别漏风格复查

一个念头闪过去，到草稿箱多出一篇完整的稿子，前后约12分钟。地铁里动一下手，出站时它已经写好在那儿了。

## 6.3 跑偏自查

这一步最容易被跳过，偏偏也最要命。

先说说什么叫跑偏——它其实就是常讲的风格漂移。举个具体例子：头一周你脱口而出“这玩意儿不靠谱”，过两周AI交上来的版本却成了“该工具的可靠性有待商榷”。它不会突然变脸，而是一点一点退回出厂腔调，等你反应过来，个人特色早被磨平了。

建议每周抽5分钟，给文风做次例行检查：拿本周产出的稿子跟写作规范逐条对照。三个信号尤其要盯：

• **说话越来越端着**：首篇还写“扯淡”，第三篇成了“不切实际”。
• **起手式和收尾变了味**：你本来习惯开门见山，AI却爱用“在这个×××的时代”铺陈。
• **黑名单词汇偷跑**：清单里明令禁用“赋能”，第四篇还是给你埋了个“数字化赋能”。

**怎么应对**：一旦嗅到跑偏，立刻回头修订写作规范和禁用词清单，把这次的漏网之词登记进去。配置不是刻好的碑，得跟着实际产出不断调整。

验证：

```
# 在 OpenClaw 中说：
对比这三篇文章和我的风格指南，检测风格一致性：
1. [粘贴本周第一篇]
2. [粘贴本周第二篇]
3. [粘贴本周第三篇]

重点检查：开头范式、收尾范式、口头禅使用、禁止词出现次数。
```

## 6.4 花费控制

整套流程跑满一个月，钱包压力大吗？答案可能让你意外：真不多。秘诀在于分配——采集阶段用不着多聪明的脑子，写稿这一环却万万省不得。

![](img/37cc623594957a354a0893b2734adf93.png)

**每月开销粗算**（按每周3篇计）：

• 素材采集：约 $2-5/月
• 写稿：约 $10-20/月
• 配图：约 $5-10/月
• **加总：约 $17-35/月**

换成单篇口径更直观：一篇走完全流程，成本不到3元。一杯星巴克的钱，就够撑起一周的更新。

**额外处理**

**朱雀检测这一关**

👸号后台会用朱雀给内容做AI味筛查，指标一旦越过30%这条线，流量就可能被压。

让人安心的是，前面搭的那套三层配置本身就在源头压低了机器感——它不靠事后补救，而是从落笔那刻起就带着真人感。若你还是心里没底，可以再加几道保险：

1. **把亲身经历塞进关键位置**——你的故事AI编不出来，这是最硬的人味凭证。
2. **搬来用户的真实发言**——MediaCrawler抓的评论区素材，带着错字和火气，反而可信。
3. **允许一点毛边**——偶尔的口语、不规范的表达，恰恰是人手的痕迹；滴水不漏才显得可疑。
4. **态度部分亲手写**——把最有锋芒的几句自己敲定，剩下的交给AI铺陈润色。

手头有检测入口的话，成稿后丢进去测一遍，把AI率压到30%以下算过关。若超了，看系统标红的是哪几段，再往那些位置补经历、补原话。

**登录态维护**

走 baoyu-post-to-wechat 的接口路线，得填 AppID 与 AppSecret；这两样永不过期，设好一次便长期有效。

换成浏览器发稿就不一样了，登录状态会失效。处理办法很简单：对 OpenClaw 说一句“帮我看看👸号登录还正常吗”，若已掉线，它会带着你重新走一遍登录。

**高频疑问**

Q：手里没有旧稿，风格档案从哪起头？

A：这是冷启动阶段最常见的卡点。其实不必等成了大V才动手。挑5个你真正在意的话题，坐下来手写，每篇不少于500字。动笔前别先列框架，脑子里蹦出什么就写什么——那股劲儿才是你的原声。

5个破冰题目供参考：

• **最近栽的跟头**——工作、生活、技术皆可，讲清怎么掉坑、怎么脱身。
• **对某个流行说法的不认同**——人人都夸A，你偏觉得有问题，把那股别扭讲透。
• **用过最惊喜与最失望的产品**——各挑一个，好坏标准由你定。
• **写给半年前的自己**——若能回去，你会提醒他什么？为什么？
• **近期让你上头的新知**——一个概念、一件工具、一本书、一句话，说清它为何打动你。

这5篇落笔，你的文风底本就够用了。请记住：文采高低不是重点，读起来像不像本人在开口才是。

Q：稿子一测，朱雀AI率直接100%，怎么破？

A：先回头看看规范写得够不够细。只写一句“语气轻松点”，等于没说。句式、常用词、段落长短节奏，都得落到具体。此外，关键处补真实经历、搬用户原话，效果立竿见影。

Q：每回写稿都手动塞三份文件，太繁琐？

A：打包成 Skill 就行。把写作规范、范文摘录、禁用词清单并进同一个 SKILL.md，OpenClaw 会自动读取，不用你再手动投喂。

Q：我的文风和咪蒙八竿子打不着，这套方法还成立吗？

A：照样成立。咪蒙只是拿来举例的样本。三层框架本身是通用的——温柔也好、锋利也好、学院派也好，路径一样：攒语料 → 提炼DNA → 生成配置 → 写入写作流程。

Q：接口只能存草稿、没法一键群发，怎么处理？

A：这是平台侧的限制，眼下绕不过去。不过草稿箱这一步未必是坏事——你可以在手机上再过一遍，等于多了一道人工质检。

Q：长期跑下来，一个月究竟多少钱？

A：按一周3篇计，采集、写作、配图三项合计约 $17-35/月。大头在写稿环节；选 Sonnet 而非 Opus，价格差不少，成稿质量却够用。

Q：手上好几个号，能共用一套工具吗？

A：工具层面可以复用，但风格档案必须各建各的。两个号定位不同，就得分别配置三层内容——流程共享，风格独立。

**附录：给想深挖的人**

为了行文利落，正文略去了不少细枝末节。哪一块想看得更全，点开对应的折叠区域就行。

**封面图五维参数一览**

**Type（构图类型）**

![](img/0699cd29c13a662cad0c49c2e1b6da14.png)

**Palette（配色方案）**

![](img/0429b42f1f63497c0ce62456a2c7aac4.png)

**Rendering（渲染风格）**

![](img/ed4e97aa04adee56664cb736af6e5049.png)

**Text（图上文字）**

![](img/37f4164b781275f9e7a3d59e5705a2a4.png)

**Mood（情绪强度）**

![](img/f77a8b6fdca2e6e7b3f2a068bba788a8.png)

**出图后端服务商清单**

![](img/a0ded9a683ce043c3c7b35b354746ed4.png)

**怎么挑**：平时出图直接用 Seedream，默认配置已经够用；想要更自然的场景转 Gemini；网络不通畅换通义万相；想折腾小众风格可以试 Replicate。

**Skill 全量清单**

![](img/68de76f32c3af9663e76c607aad87c36.png)

**整体结构示意**

```
┌─────────────────────────────────────────────────────────────────────┐
│                        OpenClaw 公众号自动化工作流                    │
│                                                                     │
│  ┌─ 素材采集层 ──────────────────────────────────────────────────┐  │
│  │                                                               │  │
│  │  ┌─ Tavily 搜索（广度）─────────────────────────────────┐    │  │
│  │  │  全网公开内容搜索，找方向、找选题                       │    │  │
│  │  └──────────────────────────────────────────────────────────┘  │  │
│  │                                                               │  │
│  │  ┌─ MediaCrawler 抓取（深度）───────────────────────────┐    │  │
│  │  │  小红书 │ B站 │ 微博 │ 知乎 │ 抖音 │ 快手 │ 贴吧        │  │  │
│  │  │  ↓ 评论区原话 + 弹幕 + 回复 + 热评                     │  │  │
│  │  └──────────────────────────────────────────────────────────┘  │  │
│  │                                                               │  │
│  └───────────────────────────────────────────────────────────────┘  │
│                          ↓ 选题 + 素材                              │
│  ┌─ 风格化写作层 ────────────────────────────────────────────────┐  │
│  │                                                               │  │
│  │  三层风格固化架构（my-writing-style Skill）                     │  │
│  │  ├─ 第一层：风格指南（System Prompt）                          │  │
│  │  ├─ 第二层：Few-Shot 范文（3-5篇代表作）                      │  │
│  │  └─ 第三层：负面约束（Anti-Slop 清单）                        │  │
│  │                                                               │  │
│  │  写作流程：大纲 → 逐段生成 → 风格校验                         │  │
│  │  可选增强：表达优化（五招）                                     │  │
│  │                                                               │  │
│  └───────────────────────────────────────────────────────────────┘  │
│                          ↓ Markdown 文章                            │
│  ┌─ 配图层 ──────────────────────────────────────────────────────┐  │
│  │                                                               │  │
│  │  ├─ 封面图：baoyu-cover-image（5维参数控制）                   │  │
│  │  ├─ 内文插图：baoyu-article-illustrator（Type x Style）       │  │
│  │  └─ 图像后端：baoyu-image-gen                                 │  │
│  │     └─ Seedream / Gemini / 通义万相 / Replicate               │  │
│  │                                                               │  │
│  └───────────────────────────────────────────────────────────────┘  │
│                          ↓ 带配图的 Markdown                        │
│  ┌─ 排版 + 发布层 ──────────────────────────────────────────────┐  │
│  │                                                               │  │
│  │  baoyu-markdown-to-html                                       │  │
│  │  ├─ 4种主题：default / grace / simple / modern                │  │
│  │  ├─ 自动内联 CSS                                              │  │
│  │  └─ 自动处理微信兼容性（字号/列表/换行）                       │  │
│  │                          ↓                                    │  │
│  │  baoyu-post-to-wechat                                         │  │
│  │  ├─ 上传封面图 → media_id                                     │  │
│  │  ├─ 上传内文图 → 替换占位符                                   │  │
│  │  └─ 创建草稿 → 草稿箱                                        │  │
│  │                                                               │  │
│  └───────────────────────────────────────────────────────────────┘  │
│                          ↓                                          │
│                   手动点击&quot;发布&quot;（微信限制）                          │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

**开工前的检查清单**

**每天（自动化跑起来之前）**：MediaCrawler 是否在正常服务（对 OpenClaw 说“帮我查一下 MediaCrawler 状态”）；需要检索境外内容时，网络环境是否已打开；OpenClaw 实例是否正常。

**每周（维护文风）**：本周稿件有无跑偏迹象（重点看口语浓度、黑名单词）；把新冒出来的机器腔补进禁用词清单；有条件就测一次朱雀指标。

**每月（系统保养）**：修订写作规范（你的文风也在长，好稿子会让它更清晰）；添新范文（把近期满意的收进去，早期不满意的剔掉）；核对接口额度与账单；把 Skill 升到最新版本。

### 03.进阶：OpenClaw 实现业务自动化

**先打个预防针**：进阶篇的案例难度都不低。刚入门的朋友，把实战篇里任意一个案例做完就够了；进阶内容不必全吃透，当作加餐来看待。实操卡住时，截图丢给AI问就行。

1. 用 OpenClaw 做企业知识库与数字员工（面向内部）

本节重点：为企业搭建知识库，进而打造一位企业级的AI数字员工。

1.1 知识库怎么搭

这只“小龙虾”（OpenClaw）如今本事见长：内置能力已经能操作浏览器、改动 Excel 表格、识别语音，感知力越来越接近真人。你还可以给它装上特定的 Skill，让它在各项专业事务上上手，日常替你跑腿办事，甚至解决一些实际工作难题，扮演数字员工的角色。当然，眼下的 OpenClaw 还谈不上完善，不妨把它当成一名实习生——在你盯着、带着的过程中慢慢长进，逐步向正式员工靠拢。

本节要讲的，就是如何搭一套私有知识库，把你手里的专有信息交给它调用。举个例子：把商品资料、公司内部文档挂上去，它立刻成了最熟悉你业务的那位助理；再开发 Skill，让它自动检索知识库、归纳经验，把沉淀做扎实；最后按场景接到飞书、企业🛰️等入口，对应解决具体业务问题。

搭建路径有两条：

第一条是云端方案。火山引擎的知识库服务支持 API 与服务两种调用方式，配置简单，新手容易上手。

第二条是本地化路线，用 AnythingLLM 把知识库部署在自己的机器上。好处是花费更省，数据不出本地，安全上更让人放心。

**先说第一种：**

（一）在火山引擎上建库

1. 打开火山方舟控制台，找到知识库入口。

![](img/035155317bb23e4b9050681ea4e91d2d.png)

2. 新建知识库。版本分标准与旗舰两档：标准版按天计费，每天1元；旗舰版面向企业按月订阅。我们选标准版就够，并且它提供30天免费试用。

# 把资料变成AI能用的能力：两条落地路线
![](img/88e65b3e6db1b9e5735d9c31c6af3bf5.png)
![](img/27161e628c37b2db138bac61933f899b.png)
先看火山引擎知识库这条线。创建时挑“标准版”即可，名字和用途说明填完就能往下走。绝大多数情况默认参数已经够用；若想抠细节，再展开高级设置也不迟。
![](img/028737242c623aa88a992f34fc2d7d7a.png)
![](img/6d68485c07b748349c2c3ee7d646c246.png)
资料仓建好后，马上进入文档灌入环节。
![](img/20e4c7589a8268130ec9f7f7908520d9.png)
本地上传通道覆盖 PDF、Word、Excel、TXT、CSV 等常见文件。
![](img/fa4a6c42851e76d1f2c2d26b5a54d173.png)
飞书里的内容也能直接同步：首次使用要完成账号授权，授权后飞书知识库与多维表格都能较顺地接进来。
![](img/576b2162fff4fe45e34cd288d855b004.png)
![](img/f6c116d2475d4201bec7c76d4028e4cf.png)
勾中目标文件，按页面底部的“导入”。
![](img/553ee1966116d61d4e9226be970344e0.png)
系统会先做文档分块，再把块转成向量并写入数据库；处理进度在状态栏可见。
![](img/fbdfa6bdb35a52eb17d9a4baad3b7ae0.png)
完成后切到“切片详情”，能逐条核对分块结果。
![](img/5cd264d1f855af3386a9f2ff830ca1a7.png)
接着用“知识检索”跑一次查询，看看召回是否符合预期。
![](img/c602cfba4d6a96b917030e79e7a00548.png)
火山引擎这套资料仓还自带大模型问答：依据检索到的内容直接组织答案。该能力可通过接口开放，用于🛰️客服自动回复。
![](img/1c4c6837f3057a28858e8bbc7db6c099.png)
不过本次并不打算把问答直接交给客服，而是要把检索结果送到 OpenClaw（下文沿用“小龙虾”这个昵称），所以接下来得把资料仓接口交给它。
![](img/80e7cd570ac13d76e4589c585c4994cd.png)
OpenClaw 本身不能裸调接口，需要先做一个 Skill 承接业务逻辑，由 Skill 去访问接口，再让 OpenClaw 使用这个 Skill。
![](img/c6cb1752ab249a1902ab239fd217d37d.png)
将下面这段代码交给 Claude Code（CC），让它代劳完成 Skill 的开发。
![](img/3f864fddb338061e01f853ae5589dd65.png)
![](img/dff3f8e6446578b3e0914005b15591a6.png)
Skill 产出后，还要补上访问凭据 AK/SK；CC 会提示你提供。
![](img/f200a65902396bf92b5391747253be4e.png)
凭据在火山引擎控制台获取：点右上角头像，进入“API 访问密钥”即可看到 Access Key。
![](img/4a1d038586687c3888548706c6e35d34.png)
![](img/3369f10c7fb377f36ba60bedbcfabb05.png)
填好凭据后，让 CC 做一次调用测试，确认 Skill 能跑。
![](img/dcce3aa3a53f1920b553b5206229a2c9.png)
若报错，就继续让 CC 修，直到链路通畅。
![](img/9759e857f814fc9cfe8304e76472fc17.png)
随后回到 OpenClaw 管理端，刚生成的 Skill 会出现在列表里。
![](img/a6f592c125c274ccea9902147b7e54aa.png)
最后在 OpenClaw 中再测一遍，验证 Skill 可以被正确调用。
![](img/49bb835f02fa7c43ef6b4c456bd098dc.png)
![](img/efbb68970ed6f8f9b45067f52956d4fa.png)
（二）AnythingLLM：把知识底座装进本机
AnythingLLM 属于全栈型工具：既可用商业大模型，也可搭配开源模型，再加向量数据库，把文档变成私有的对话式知识应用。它既能全本地运行，也能托管到远程；资料不必交给外部平台，还能围绕你手头的文件进行智能问答。
它的组织单位叫 workspace（工作区）。工作区类似会话线程，又额外承担文档容器角色；不同工作区可以共用文件，但内容互不串扰，因此各自的上下文能保持干净。
把它当成一座私人资料馆更直观：文档、笔记都收进去，内置的 AI 文档引擎会依据馆藏作答。引擎可接 ChatGPT 等模型接口，也能在本地跑开源模型。
这次真正要用的，是它开放的资料库 API。
安装方式很省事：官方提供客户端。打开 https://anythingllm.com/ 下载对应版本即可。
![](img/3c5438810890d67293eca11c71a5bcb9.png)
按操作系统选安装包，装完会看到初始化界面。
![](img/f6d089e8e4b980e243b58f61a3e07e7d.png)
首次启动可沿用推荐方案：把 Qwen 模型拉到本地；也可以改用其他模型的 API，看个人偏好。
![](img/870b8d8a39b723a508e98dca6e1d8b52.png)
Provider 与向量模型这两项，保持 AnythingLLM 自带的默认选项即可。
![](img/5a170e7efb716de29e25b2c1cbc5d9ee.png)
该步骤可直接略过，暂时无需处理。
![](img/b9ef729bd759d4859d387433667651d2.png)
之后便进入主界面。
![](img/46cddc08251b1095ac06ab6ca654e852.png)
刚安装时里面是空的，先新建一个工作区。
![](img/ab6476daca7b4eec47af3f52cdb8f446.png)
名称随意，例如用产品名。
![](img/42a6af4f29f98a346592416588f7ceb9.png)
然后点上传文档，把资料灌进去。
![](img/6013986522c8f2fd6f185883c86cb2db.png)
若文件在飞书里，需要先落到本地再上传；它虽然提供链接导入，但实测对飞书文档解析不理想。
![](img/f59c1ab1f1b8338c713c048c3287ad78.png)
它还支持从多个笔记仓库同步数据；若资料存放在可同步的笔记平台，可直接关联。
![](img/fee978be9d0913ed0c57436244e159f9.png)
文件上传后，勾选目标文档，点下方 Move to Workspace，将其归入工作区。
![](img/0f039514e15cb7f8c2897cb859cfb604.png)
再执行 Save and Embed，完成向量化存储。
![](img/d465f633498497cf82f03a5e53c2dc3d.png)
先用系统自带的问答界面验证资料库能否响应。由于前面装了 Qwen 7B 本地模型，基础问答可在本机完成。
![](img/556da8df8de5397bfde2c419abcb8550.png)
随后配置接口调用：点左下角设置。
![](img/77c78796fdc05f169db8121f959517a8.png)
在 Development API 菜单中生成一个 API Key。
![](img/94fc92686aeb8a5337499751ea90c7b9.png)
该页面能看到完整的接口文档。
![](img/294557ac665bbe47b7864c86299e3097.png)
后续若要扩展功能，照这份文档操作即可。
![](img/7871c32b259e5bd311d65c9969ea0a39.png)
AnythingLLM 的默认接口地址为 http://localhost:30001/api/v1。把 Base URL 与刚生成的 API Key 一起交给 CC 测试。
```
http://localhost:30001/api/v1
```
![](img/f395528c3960ce32fb8393aa36aa49ab.png)
测试通过，就说明本地资料库接口可用。
![](img/bad8d0a63f078b9dbbfbb4b34e607d27.png)
同样让 CC 写一个 Skill，供 OpenClaw 调用。
![](img/d1ae1cda461bd314612981e23d812898.png)
重启 OpenClaw 后，管理端会显示新建的 Skill。
![](img/e4dacbb2b2432cc043e242edc870bd42.png)
![](img/e5163fc559e6e5bde8c5e8f4da7765c6.png)
再到 OpenClaw 里测一次，确认它能正常访问资料库。
![](img/e51dd4b30132b51b03daff61d75414c7.png)
OpenClaw 具备资料检索能力后，可拓展的场景不少。
**个人 AI 助理**
把个人笔记、聊天记录等灌入资料库，OpenClaw 就能充当私人助理。执行任务时，它会调取馆藏内容，把你的个性化信息带进结果。
**企业 AI 数字员工**
将 OpenClaw 接入企微，可形成企业内部数字员工：行政问答、财务流程、IT 答疑、客服协助等岗位都能覆盖。
![](img/4f3cfb588fadc7d00465513701907817.png)
1.2 让企业多一个数字员工：OpenClaw 接入企微
先建一个智能机器人。工作台菜单里有“智能机器人”入口；若没看到，用右上角搜索。
![](img/67f9d8aae8a1f936b125a58326b642c7.png)
进入后点创建机器人。
![](img/211982513e01b6fb0325bd1f059565f4.png)
选手动创建。
![](img/59880baf88c190a69be5d61747566f20.png)
创建方式选 API 模式。
![](img/ea11523a6b5b8c4eec43272053a98cd3.png)
连接方式用长连接，并记下 Bot ID 与 Secret。
![](img/2c45a1f0f0366f660cdc0b9f470ddf5e.png)
可见范围要设好，也就是机器人将在哪些内部场景出现，例如某个员工群。
然后回 OpenClaw 终端，装企微插件，执行 Ada。
```
openclaw plugins install @wecom/wecom-openclaw-plugin
```
![](img/79c32d958090b8a25e56d0e77910d6c8.png)
终端里运行 Ada 命令，重启 OpenClaw。
```
openclaw gateway restart
```
添加渠道同样用 Ada 命令。
```
openclaw channels add
```
![](img/c39822b284c10947a9e0a6c5d7755dda.png)
在渠道选择界面（select channel）把 channel 指向企业🛰️，随后填入机器人 Bot ID 与 Secret，选择 finish。
![](img/d38a9d6fa2ca859e83a534505afc51ed.png)
配对方式选 Pairing。继续完成后续配置，界面会提示渠道配置成功。
![](img/361bbf9de537e3a278c051c48dbbccae.png)
![](img/55ec87bb48c0f1257f8077a850e1a53b.png)
回到企微，保存机器人并给它发一条消息，会收到配置密钥。
![](img/636b1407f9d1088c0b1a703ded4e1f1d.png)
把消息最后一行密钥复制到终端。配对完成后，就能在企微里与机器人正常对话。
![](img/d24f9a214d67bbc98019cd9f10aa5d85.png)
![](img/3176d94e44b37d940f0f61c113278fa8.png)
之后在员工群里 @ 这个“数字员工”，即可派任务。
![](img/eeebab733531fa6e9b625d36fcd0cdc3.png)
OpenClaw 还能接🛰️客服，直接答复用户。此前航海分享过用扣子搭客服工作流并接入🛰️客服的做法；现在 OpenClaw 也能实现。官方没有现成插件，但开源插件 openclaw-wecom-kf 可用。它的配置偏复杂，属于进阶玩法，这里只做介绍，感兴趣可自行研究：
https://github.com/rcfcu2000/openclaw-wecom-kf
openclaw-wecom-kf 是🛰️客服渠道插件，目的是让外部🛰️用户通过企微客服系统与 OpenClaw 智能体互动。
它与 wecom-app 的差异不展开。
若要接其他客服系统，例如淘宝、抖音等电商客服，多数平台未开放接口，直接让 OpenClaw 接入会比较费劲。OpenClaw 目前没有 RPA 能力；虽然能操作浏览器，部分客服系统也有 Web 端，但要让 OpenClaw 自行收发送客服消息，仍需一定开发工作。
![](img/833489d4b04c9b82643a8fb6075cd7bc.png)
2. 对外客服自动化：OpenClaw 接入🛰️客服
本节讲如何让企微客服具备 AI 能力：客户扫码后，即可与配置好的 AI 资料库自动对话。
**先花两分钟弄懂链路**
先别急着操作，把整体流程看清楚，后面就不容易卡。
```
客户用微信扫码
↓进入客服聊天窗口，发一条消息
↓消息先到企业微信的服务器
↓企微把消息&quot;转发&quot;到你的服务器（这叫&quot;回调&quot;）
↓你服务器上的 OpenClaw 收到消息，丢给 AI 处理
↓AI 用你喂的知识库生成回答
↓回答通过企微的接口发回给客户
↓客户微信里收到回复 ✅
```
有三个词会反复出现，先认识一下：
- 🛰️客服：企微中面向外部🛰️用户的服务模块，类似淘宝店铺的在线客服入口。
- 回调：企微收到消息后，把事件推送到你指定的服务器网址，好比留下收件地址后快递直接送上门。
- OpenClaw：承载 AI 客服的开源 Agent 平台，可理解为 AI 调度中心。
还要区分两个后台，否则很容易配错位置：
1. 企微管理后台：https://work.weixin.qq.com/wework_admin/frame
   用于创建自建应用，后续补可信 IP。
2. 🛰️客服后台：https://kf.weixin.qq.com/
   这是本教程的主场地。创建客服账号、查找 openKfId、配置回调 URL、生成 Token 与 EncodingAESKey、获取 corpSecret，都优先在这里完成。
需要收集 5 个值。以🛰️客服后台为主，收齐后填入 OpenClaw：
1. 企业 ID（corpId）：待录入，位置在🛰️客服后台 → 企业信息。
2. 客服账号 ID（openKfId）：待录入，位置在🛰️客服后台 → 客服详情；页面不显示时可用接口兜底查询。
3. 回调 Token：待录入，位置在🛰️客服后台 → API 配置。
4. 回调 EncodingAESKey：待录入，位置在🛰️客服后台 → API 配置。
5. 🛰️客服 Secret（corpSecret）：待录入，位置在🛰️客服后台 → API 管理，回调验证通过后获取。
有两个坑要留意：
1. 第 5 项 Secret 并非自建应用的 Secret，而是“🛰️客服”自己的 Secret。
2. openKfId 有时在页面中不显眼，甚至一时找不到。不必卡住，后面可用接口查出来。
第一步：注册企微并记录企业 ID
1.1 注册企微（已有可跳过）
个人也能注册，不要求真有公司。
1. 电脑打开 https://work.weixin.qq.com/
```
https://work.weixin.qq.com/
```
2. 点页面中间的蓝色「立即注册」按钮。
3. 类型选「企业」——个人同样选这个，不影响。
4. 开始填写资料：

# 🛰️客服接入 AI，九步配置通关

动手前先把三个基础项填掉：公司名称随意取，比如“XXX 工作室”；行业类型按实际情况挑；人员规模直接选最低那档。

1. 拿手机用你日常的个人🛰️，扫一下页面上的码。
1. 跟着系统提示点确认，这一步就结束了。

![](img/43878f357c78e28cc982cce72d4eaebb.png)

1.2 保存企业 ID

1. 确认完一般会自动跳到管理后台；要是没跳，自己在地址栏敲开：https://work.weixin.qq.com/wework_admin/frame
1. 进后台后看左边导航，一路拖到最底部，点「我的企业」。
1. 进入后继续往下拉，会碰到「企业 ID」这一项。
1. 它的值是一串 ww 打头的字符，例如 ww1a2b3c4d5e6f7890。
1. 复制下来，先丢进手机备忘录。

![](img/e63d4b63ed769499dccc18fd66db4ebc.png)

这一段做完，把它填进表格第一行。

**第二步：搞一个自建应用**

1. 左侧导航里点开「应用管理」。
1. 页面往下滑，找到「自建」那一块。
1. 点「创建应用」按钮。

![](img/426b422b670b65d48d9e8c858c36070f.png)

1. 表单这样填：
- 应用名称：写“AI客服助手”或者你顺口的名字。
- 应用 Logo：随便传一张图。
- 可见范围：直接挑「全公司」，后面会省很多事。

![](img/3165e60af056d34520838d99985f84d8.png)

1. 点「创建应用」确认，这一步收工。

**第三步：开通🛰️客服并建客服账号**

3.1 把🛰️客服功能打开

1. 在左侧导航里找「🛰️客服」；列表里没看到的话，去「应用管理」里翻一翻。
1. 第一次点进去，系统会让你开通，按「开通」就好。

![](img/a785f1dd20102d3a4af94461f9637b18.png)

![](img/ee2ec29611d1478cc8f961af06b6cd4f.png)

3.2 建一个客服账号

1. 点「添加客服账号」。
1. 填这几项：
- 客服名称：客户将来在聊天窗口看到的那一个，比如“在线客服”“智能客服”。
- 客服头像：传一张，客户对话时看到的就是它。
1. 在「添加接待人员」那里勾上你自己。

这里有个容易漏的地方：被勾上的人必须落在第二步那个应用的可见范围内。前面如果选了「全公司」，这里自然没问题。

1. 按「确定」。

![](img/f064980b588be68b8ed767eeb5cdef25.png)

3.3 存下客服账号 ID

1. 点开刚建好的账号，进详情页。
1. 里面有个 open_kfid，形如 wkABCDEF1234567890，wk 开头。
1. 复制它。

页面上翻不到 open_kfid 也别死磕，两条路：
1. 先记下客服名称，之后再回来看；
1. 直接走接口把客服账号列表拉出来，从中取 ID。

我当时的做法就是让小龙虾调接口查出来的。

拿到之后，填到表格第二行。

**第四步：到🛰️客服后台拿回调参数**

这一趟能带回两个值：Token（第三个）和 EncodingAESKey（第四个）。

请认准🛰️客服后台 https://kf.weixin.qq.com/，别跑去自建应用详情页。

1. 进🛰️客服后台。
1. 找到 API 配置那一页。
1. 生成 Token。
1. 生成 EncodingAESKey。
1. 先把它们复制下来存好。
1. 此刻先不要按「完成」或者「开始使用」。

![](img/dab2bd65131ae202404af7782d06e36b.png)

原因很简单：一点完成，🛰️客服马上就会去请求你填的那个回调地址。OpenClaw 此时还没弄好，验证十有八九会挂。

另外再强调一句：回调 URL、Token、EncodingAESKey 这三个东西，都在🛰️客服后台这边搞定，不要去自建应用的「接收消息」里折腾。

![](img/734424485cef011cc7ca6b221fc45e1c.png)

![](img/158350185231cfb48dc4630147106727.png)

![](img/b4392cecf38af3057a3cefd7475fdea2.png)

**第五步：把服务器 IP 加进白名单**

企业🛰️有个硬性安全机制：API 只认白名单里的 IP。你的机器不在名单中，接口会当场回绝。所以得手动加。

1. 左侧导航进「应用管理」，点你自己建的那个应用。
1. 进入应用后往下翻，找到「企业可信 IP」。
1. 点「配置」。
1. 把服务器的公网 IP 填进去——只写 IP，端口号不要带。
1. 点「确认」。

![](img/89a73a163668fba13fa391420d9b1f0f.png)

不清楚 IP 的话，打开云厂商控制台，服务器详情页里就写着“公网 IP”。

![](img/fd4d7ff39f8a400cf530c06bd1829c92.png)

**第六步：打开一次终端，粘贴命令结束战斗**

整个流程里只有这里需要碰终端。你只需复制一段命令再粘贴，不用手写代码。

6.1 连上服务器

终端说白了就是一个黑框，你敲指令，服务器照做。连接方式看系统：

- Mac：打开「终端」，敲 ssh root@你的服务器IP，回车后输密码。
- Windows：可以用 PuTTY 或者 Windows Terminal。
- 最省事的办法：去云服务商控制台找「远程连接」，阿里云、腾讯云都提供了网页版终端。

![](img/84bfd09f3ff7dbbf21bdecab0c1d34de.png)

屏幕上出现 root@server:~# 这类提示符，说明已经连进去了。

6.2 复制命令并替换变量

别急着敲。下面这段命令里有四个位置要换成你自己的数据，先把前面收集的四个值摆在手边。

整段复制，把四个“替换成你的 xxx”逐一改成实际值，再粘贴进终端回车：

Bash

```
# 第一步：安装微信客服插件
openclaw plugins install @openclaw-china/wecom-kf &amp;&amp; \
# 第二步：填入你的 4 个配置值
openclaw config set channels.wecom-kf.enabled true &amp;&amp; \
openclaw config set channels.wecom-kf.webhookPath /wecom-kf &amp;&amp; \
openclaw config set channels.wecom-kf.token &quot;替换成你的Token&quot; &amp;&amp; \
openclaw config set channels.wecom-kf.encodingAESKey &quot;替换成你的EncodingAESKey&quot; &amp;&amp; \
openclaw config set channels.wecom-kf.corpId &quot;替换成你的企业ID&quot; &amp;&amp; \
openclaw config set channels.wecom-kf.openKfId &quot;替换成你的客服账号ID&quot; &amp;&amp; \
openclaw config set channels.wecom-kf.welcomeText &quot;你好！我是 AI 客服，有什么可以帮您的？&quot; &amp;&amp; \
# 第三步：允许外网访问 + 重启
openclaw config set gateway.bind lan &amp;&amp; \
openclaw gateway restart
```

举个例子，假设你手上是这些：

- Token 为 aBcDeFgHiJkLmN
- EncodingAESKey 为 abcdefghijklmnopqrstuvwxyz01234567890ABCDEF
- 企业 ID 为 ww1a2b3c4d5e6f7890
- 客服账号 ID 为 wkABCDEF1234567890

那就把“替换成你的Token”那段改成 aBcDeFgHiJkLmN，其余三项同理处理。

命令里没有 corpSecret 是刻意为之，它要到下一步才出现，这里空着不影响回调验证。

6.3 判断成功与否

跑完应该能看到三件事同时成立：

1. 插件装上，屏幕上出现 installed @openclaw-china/wecom-kf。
1. 几条 config set 命令无报错。
1. Gateway 完成重启。

想进一步确认 Gateway 真的活着，再执行一条命令：

Bash

```
openclaw gateway --verbose
```

屏幕上打出 [wecom-kf] webhook registered at /wecom-kf，就说明插件已经就位，正等着企微把消息送过来。

装插件时如果报错，基本是网络卡了。换个国内镜像重新来一遍：

Bash

```
npm config set registry https://registry.npmmirror.com
```

**第七步：回后台完成验证，把 Secret 拿回来**

7.1 走完回调验证

这一步仍然回🛰️客服后台 https://kf.weixin.qq.com/，不是自建应用的详情页。

1. 打开🛰️客服后台的 API 配置页。
1. URL 框里填：http://你的服务器公网IP:18789/wecom-kf

举个例，IP 是 123.45.67.89 的话，就填 http://123.45.67.89:18789/wecom-kf。

1. Token 与 EncodingAESKey 两个框，确认填的是前面保存下来的那两个值。
1. 点「保存」或「完成」。

![](img/c2648b6f246c1a89e9764de3972d268d.png)

几个关键点再强调一次：

- 回调 URL 一定落在🛰️客服后台。
- 如果你的第一反应是去自建应用里配——请打住，按这里的路径重来。
- 我自己最早就是配错了地方，客户发消息过来毫无动静，后来换到🛰️客服后台才通。

看返回结果：

![](img/095a95b6e01df2546a25a0fc2df996f2.png)

验证没通过，逐条排查：

1. Gateway 进程还在吗？回终端看日志。
1. 是否执行过 openclaw config set gateway.bind lan？这条不做，外网访问无门。
1. 18789 端口是否放行？去云服务商安全组里确认。
1. IP 是否填准？控制台里核对。
1. Token 和 EncodingAESKey 是否和配置一字不差？注意别多出空格或漏掉字符。

![](img/78e65b56f91ab6894c8e7c20d35ca640.png)

7.2 补齐可信 IP 与接口授权

要是在这一步发现应用调不通🛰️客服接口，再补两个动作：

1. 回企业🛰️管理后台。
1. 打开自建应用。
1. 配好「企业可信 IP」。
1. 然后回到🛰️客服后台，把这个应用标记为「可调用接口的应用」。

顺序上容易绕晕，你记这一句就够：先让回调通，再补可信 IP 和应用授权。

![](img/f9174c5899f43db07d1aaa6b89f16628.png)

7.3 取回🛰️客服的 Secret

这个 Secret 最终是在🛰️客服后台拿到的，不在企微应用页面里。

1. 回到🛰️客服后台。
1. 找到 API 管理相关页面。
1. 定位到🛰️客服的 corpSecret。
1. 按提示完成验证后复制。

再三提醒：这是“🛰️客服”的 Secret，跟第二步那个自建应用的不是同一个东西。外形接近，含义不同，别混用。

到这里，五个值全部凑齐。

7.4 写入 Secret

最后再进一次终端，只有两条命令。连上服务器，粘贴并把占位值换掉：

Bash

```
openclaw config set channels.wecom-kf.corpSecret &quot;替换成你的Secret&quot; &amp;&amp; \
openclaw gateway restart
```

看到 Gateway 重启成功，就可以关掉终端。剩下的操作都在浏览器和手机上完成。

**第八步：取得客服入口**

方式一：二维码（最常用）

1. 在「🛰️客服」里点开你建的客服账号。
1. 找到「客服链接」或「获取二维码」。
1. 把图片下载下来。

这张码的用处很广——网站、👸号菜单、朋友圈海报、名片、传单、包装盒，贴哪儿都行。

![](img/112a40f47180d8c1c424bb28ab0e8bff.png)

方式二：链接

同一个页面能拿到对应的 URL。可以放在：

- 网站的“在线咨询”按钮上。
- 用短信发给客户。
- 👸号自定义菜单里（自定义菜单 → 跳转网页 → 填入这个链接）。

方式三：嵌入网页或小程序

网页里加一个链接即可：

HTML

```
&lt;a href=&quot;客服链接URL&quot;&gt;在线咨询&lt;/a&gt;
```

小程序的话：

JavaScript

```
wx.openCustomerServiceChat({ extInfo: { url: &#x27;客服链接URL&#x27; }, corpId: &#x27;你的企业ID&#x27; })
```

**第九步：跑一次完整测试**

1. 掏出手机，用个人🛰️（注意不是企业🛰️）扫上一步保存的二维码。
1. 进入对话后，欢迎语应该会自动弹出来。
1. 随便发一句，比如“你好，你们有什么产品？”
1. 等几秒钟。
1. 如果一切正常，AI 会回你。

万一迟迟没动静，翻到下面的“常见问题”对照排查。正常状态下，几秒内就有响应。

看到回复，恭喜，整条工作流已经跑通。

后面是排查与进阶，用到时再来查。

![](img/4edae389207a542f273f64532b1c4560.png)

**常见问题**

找不到 openKfId 怎么办？

别慌，这不是你一个人的困惑。有些页面就是把它藏得深，甚至不直接露出。

处理路数：

1. 先确认客服账号确实建成了。
1. 把客服名称记下来。
1. 然后走接口拉客服账号列表来定位 ID。

不要因为界面上暂时看不到，就怀疑前面每一步都白做了。

回调配好了，为什么发消息没反应？

先问自己回调 URL 到底配在哪儿。

如果你把它塞进了自建应用而不是🛰️客服后台，八成就是这里出的岔子。在 wecom-kf 这条链路里，回调 URL 应该优先写在🛰️客服后台。

客户发消息了，AI 不回复

三关排查，哪一关断了修哪一关。

第 1 关：消息到服务器了吗？

看日志里有没有 [wecom-kf] callback received。

- 没有 → 消息根本没进来，去查 URL 是否正确、端口有没有放开、Gateway 是否在跑。
- 有 → 说明消息到了，看第二关。

第 2 关：消息拉取成功了吗？

看日志里有没有 sync_msg。

- 报错 → 通常指向 corpId 或 corpSecret 填错，或者 IP 白名单没加。
- 正常 → 继续第三关。

第 3 关：AI 处理了吗？

看日志里有没有 dispatching to agent 或者 reply sent。

- agent 报错 → 说明问题在 AI Agent 本身，与🛰️客服无关，去查 Agent 配置。
- reply sent 出现了但客户没收到 → 对着错误码往下看。

报错 95017

48 小时窗口过期。客户最后一条消息已经超过 48 小时，企微不允许你再回复。

正常客服场景基本碰不到。调试时撞上了，让客户重新发一条即可。

报错 60030

接待人员不在应用可见范围内。

回第二步那个应用，改「可见范围」，把接待人员所属部门加进去。

回复格式乱了（星号井号满天飞）

🛰️客服不认 Markdown。插件会自动转一道（标题变成【标题】，加粗去掉星号），但不保证每次都完美。

对策：在 Agent 的系统提示词里补一句——“回复客户用纯文本，不要用 Markdown。”

回复太长被截断

企微单条消息上限 2048 字节，折合约 680 个汉字。插件会自动拆成多条，但超过 5 条就会受限。

对策：在 Agent 提示词里加一句——“回复控制在 500 字以内。”

没有公网 IP

方案一：ngrok 内网穿透。

Bash

```
ngrok http 18789
```

它会给出一个公网地址（形如 https://abc123.ngrok.io），填进企微的回调 URL 里：

Plain Text

```
https://abc123.ngrok.io/wecom-kf
```

注意免费版每次重启地址都会变。要长期用，建议上云服务器。

方案二：VPS + Nginx 反向代理

用 Nginx 把回调转发到本地，配置里加上：

Bash

```
openclaw config set channels.wecom-kf.apiBaseUrl &quot;https://your-vps.example.com&quot;
```

**进阶玩法**

以下都是可选项。基础功能在前面已经能跑起来了。

改欢迎语

Bash

```
openclaw config set channels.wecom-kf.welcomeText &quot;你好呀！我是 XX 品牌的 AI 客服，有啥问我~&quot;
```

小提示：欢迎语有 20 秒有效期，客户进来 20 秒内发出去才有效，超时就不发了。正常场景碰不到。

白名单模式（只让特定客户聊）

Bash

```
openclaw config set channels.wecom-kf.dmPolicy allowlist
```

然后在配置文件里加：

JSON

```
&quot;allowFrom&quot;: [&quot;external_userid_1&quot;, &quot;external_userid_2&quot;]
```

每条外部访客记录都带着一个 external_userid，翻一翻 Gateway 的日志记录就能对上号——外部用户一人一个，不会重复。

同一条链路里跑几条业务线，就可以让它们各自对接不同的 AI：买东西的咨询交给“销售客服”，技术问题丢给“技术支持”。不过有个前提动作别漏掉：企微后台得为每个客服号单独开通、单独登记回调地址，之后靠 bindings 这份配置，把消息派发到对应的 Agent 手上。

```
{&quot;channels&quot;: {
    &quot;wecom-kf&quot;: {
      &quot;enabled&quot;: true,
      &quot;corpId&quot;: &quot;wwXXXXXX&quot;,
      &quot;accounts&quot;: {
        &quot;sales&quot;: {
          &quot;openKfId&quot;: &quot;wkSALES123&quot;,
          &quot;corpSecret&quot;: &quot;sales-secret&quot;,
          &quot;token&quot;: &quot;sales-token&quot;,
          &quot;encodingAESKey&quot;: &quot;sales-aes-key&quot;,
          &quot;webhookPath&quot;: &quot;/wecom-kf-sales&quot;,
          &quot;welcomeText&quot;: &quot;欢迎咨询我们的产品！&quot;
},&quot;support&quot;: {
          &quot;openKfId&quot;: &quot;wkSUPPORT123&quot;,
          &quot;corpSecret&quot;: &quot;support-secret&quot;,
          &quot;token&quot;: &quot;support-token&quot;,
          &quot;encodingAESKey&quot;: &quot;support-aes-key&quot;,
          &quot;webhookPath&quot;: &quot;/wecom-kf-support&quot;,
          &quot;welcomeText&quot;: &quot;技术支持为您服务。&quot;
}}}}}```

JSON

```

JSON

```

{&quot;bindings&quot;: [

    { &quot;agentId&quot;: &quot;sales-agent&quot;, &quot;match&quot;: { &quot;channel&quot;: &quot;wecom-kf&quot;, &quot;accountId&quot;: &quot;sales&quot; } },

    { &quot;agentId&quot;: &quot;support-agent&quot;, &quot;match&quot;: { &quot;channel&quot;: &quot;wecom-kf&quot;, &quot;accountId&quot;: &quot;support&quot; } }

]}

```

**已知限制**

| 限制 | 说明 | 影响 |
| --- | --- | --- |
| 只能回纯文本 | 不支持 Markdown，不能发图片 | 客服够用，后续会支持 |
| 48 小时窗口 | 最后一条消息后 48h 内才能回 | 正常秒回，碰不到 |
| 单次最多 5 条 | 每次最多回 5 条 | 回复别太长就行 |
| 单条 2048 字节 | 约 680 字，超了自动拆 | 让 Agent 控制长度 |
| 要公网地址 | 回调必须公网可达 | 用 VPS 或穿透搞定 |
| 欢迎语 20 秒 | 超时不发 | 正常不会超 |

**相关链接**

| 资源 | 说明 |
| --- | --- |
| openclaw-china | wecom-kf 官方仓库 |
| OpenClaw | 核心框架 |
| 企微文档 - 微信客服 | 官方文档 |
| 企微文档 - 接收消息 | 回调格式 |
| 企微文档 - 发送消息 | 发送接口 |

# 选修篇

## 四、Claude code 的拓展玩法

### 01.用 Claude code 进行第二大脑的搭建

1.项目介绍

这个项目主要来介绍下当前 AI 火爆的前提下，我们如何使用 Claude Code 来搭建我们的第二大脑（知识库）

**技术方法：**

Obsidian+Claude code，通过指挥 Claude Code，来让它帮你维护和调用 Obsidian 里的资料。

Obsidian 是用来存放知识库的素材（聊天记录、会议纪要），Claude code 是可以在电脑中运行 Obsidian

让 Claude code 按照你的 S.O.P。（标准作业程序）去自动化处理你的知识库

**参考学习文档：**

[https://mp.weixin.qq.com/s/Bz](https://mp.weixin.qq.com/s/BzYUPEByISXJ5WslgQostA)YUPEByISXJ5WslgQostA

1.1Markdown 介绍

💡本小节作为 markdown 的知识普及章节

看第一遍知道就行，后面有不懂的可以再回来进行查看

! ! 如果不懂的可以结合后面的 Obsidian 软件创建下笔记多练习下！！

markdown 作为一种特殊的普通文本文件的语言，是目前大模型可以识别的一种文本类型。

那大家可能疑惑，为什么 word 类型的格式不行，word 是微软文档的特殊格式，是属于商业标准，并且解析 word 文件是比较困难，也不方便识别

**用纯文本写作，通过几个简单符号控**制格式，不需要像 Word 那样点按钮。

**为什么新手值得学？**

你可能会在这些地方经常遇到 Markdown：

• 写笔记：Obsidian / Notion（部分）/ 飞书文档（部分）

• 写项目文档：GitHub 的 README、开源文档

• 写技术文章：博客、掘金、语雀（很多都支持）

• 跟 AI 协作：让 AI 输出结构化内容（标题、步骤、代码）

它的优势对新手很友好：

• **不需要鼠标点格式**：键盘一把梭

• **格式统一**：不容易写成“排版灾难现场”

• **跨平台**：几乎到处都支持

**学习建议**

Markdown 语法非常少，上面这些基本覆盖了**日常 9**0% 的使用场景。最好的学法就是边写边练——找一个支持 Markdown 的编辑器（比如 VS Code、Typora、Obsidian），直接开始写就行。写个几篇笔记，自然就记住了。

最核心的语法（你学会这些就够用了）

下面每条都给你“写法”和“效果”。

**标题**

```

Plain Text

```text

# 一级标题
## 二级标题
### 三级标题
```

**斜体、加粗、删除线：三种文字强调法**

想让某几个词跳出来？加粗最直接；想带点语气，斜体合适；标个删除线，表示这句作废。

Plain Text

```
**加粗**
*斜体*
~~删除线~~
```

**列表：出场率最高的结构**

```
- 苹果
- 香蕉
  - 小香蕉（缩进两个空格或一个 Tab）
```

无序列表：并列的信息一行一条，最清爽。

Plain Text

```

1. 第一步
2. 第二步
3. 第三步
```

有序列表：讲步骤、排优先级，用它更清楚。

Plain Text

```
&gt; 这是一段引用
&gt; 可以多行
```

引用：把别人的一句话单独拎出来强调。

Plain Text

```
[显示文字](https://example.com)
```

超链接：让裸网址变成可点击的文字。

Plain Text

```
![图片说明](图片链接或本地路径)
```

图片：一段描述，往往比不上一张图。

```
用 `pip install` 安装依赖
```

Plain Text

单个词或短命令，包一层反引号就是行内代码；要贴整段程序，换成多行代码块。

Plain Text

**多行代码块这样写：**

Python

```
print(&quot;hello&quot;)
```

Plain Text

**新手容易翻车的地方，提前扫一眼：**

Plain Text

```
标题 # 后面要有空格
 ✅ # 标题
 ❌ #标题
列表的缩进要对齐
 子列表要缩进，否则会“散架”。
代码块的三连反引号要成对出现
 少一个就会把后面内容全变成代码。
不同平台支持不完全一致
 比如表格、任务清单，有的平台支持得更好（GitHub 一般最稳）。
```

**1.2 走近 Obsidian**

如果你习惯拿 Markdown 敲字，又想把日常积累攒成一座私人资料库，Obsidian 是个绕不开的名字。它装在本地，既管笔记，也管知识。

**它的定位**

说到底，它就是个 Markdown 编辑器。真正让它出圈的是“双链”——两对方括号把两篇笔记拴在一起，时间久了自然长出一张网；再打开图谱视图，这张网长什么样，一目了然。

**几处硬实力**

- 内容全在你自己的硬盘上：每篇笔记就是一个 .md 文件，没有云端依赖，隐私握在自己手里，也不必操心哪天台子倒了。
- 双链加持的图谱：普通笔记工具只存文字，它让文字之间产生关系，散落的碎片因此能连成片。
- 社区插件多到夸张：上千款，日程、看板、表格视图、脑图、对接各种服务，基本想到的都有。
- 想怎么改就怎么改：配色、热键、面板摆放，全凭个人习惯。

**哪些人会更爱它**

打算给自己建一套外挂记忆体的；写东西离不开 Markdown 的；在校生、做研究的、码字的、写代码的；以及不愿把私人记录交给云厂商的。

**要花多少钱**

自己用不花钱。跨设备同步（Sync）和对外发布（Publish）属于增值服务，需要付费；不想掏钱，也能靠 iCloud 或 Git 自行搞定同步。

**横向比一比**

Notion 强在多人实时编辑与数据表；Logseq 和它思路相近，但插件成熟度上 Obsidian 更胜一筹，而 Logseq 一上来就是大纲流。

**怎么开始**

别急着设计一套完美体系。先记，边记边拿双链把相关的内容连起来，结构会自己浮现。入门可以先摸清 Daily Notes、Templates、Outliner 这几个内置能力。

概括一句：门槛低，天花板高，值得上手试试。

**1.3 把 Obsidian 装上**

官网地址：https://obsidian.md/

Windows 用户：进下载页 https://obsidian.md/download 拿安装包 ![](img/2d0aa9e4ba78ce221be0a4033e7de832.png)，双击启动 ![](img/d95f66b6dd82fceb877bab251a457c4f.png)，系统弹权限框就点“是” ![](img/b42603529a5cf872a244eeede38f91df.png)，挑个安装位置 ![](img/e2e1f3aa2b9186eca5691c71afe65308.png)，等进度条走完 ![](img/7dd0231cb4b0b13953a3b51716d6241e.png)，按下“完成” ![](img/584003ccbbb0edea390d943390cade51.png)，桌面上就会多出一个 Obsidian 图标 ![](img/7a99f23c00b577144644b7ec26af21f7.png)。剩下的配置放到下一节说。

Mac 用户：同样在下载页点按钮 ![](img/61a9f3a448ea5212e97e4c069d87d0e3.png)，拿到 DMG 后双击打开 ![](img/3a320735428a03718f97f7d3e2ddb567.png)，把图标拖进右侧的 Applications 里 ![](img/12e0b50d73b80311282e3befba4c267f.png)，完事。从系统里的程序列表找一下，就能看见它 ![](img/229d6255c8e2b31e87fb0f571c11c6e8.png)。

**1.4 初次启动的配置**

Obsidian 里的内容都得归属于某个仓库（vault），所以动手前先把仓库建好。点“创建” ![](img/5f897bbcad267ab9bc047d9056995d49.png)，按提示往下走 ![](img/24684622d15a9b95072d7b2f424cb1fe.png)，浏览时挑一个专门用来放 Obsidian 数据的目录 ![](img/c053d17b5a5c10e04dcc8ac4893f6892.png)，完成后会停在默认界面 ![](img/1b356fb1829ccd1285b0c4589231a797.png)。

**1.5 上手几个基础动作**

新建一篇笔记：左侧栏空白处点右键，选新建笔记 ![](img/3ad0fd10eef44f2e4317f2dac6986547.png)，出来的样子是这样的 ![](img/b053240c83bf212dae4e7c4e5a3725cf.png)，接着直接往里写就行 ![](img/e77865d5c3015f7de184b5692c51547e.png)。

改动内容：光标放进去敲字即可。

装插件：照图点，头一回进插件页得先把安全模式关掉 ![](img/42c2db14af3e4b8458c59d48ddca0fb7.png)，再点“浏览” ![](img/a1d171912a10d58d943ff874df404dbd.png)，就能逛社区插件了 ![](img/5bdad991f4a74ef3d04f1f3b216f00c7.png)。

**2. Claude Code 搭配 Obsidian 的实战准备**

真正的重点从这里开始。Obsidian 管的是知识与素材，Claude Code 扮演的是你的 AI 副手，两者配合，笔记体系的打理能轻松不少——相当于给 Obsidian 装上一个外脑。

💡组合方式不止一种，下面这套是我认为多数人接受门槛最低的。另有两个灵活点值得记住：其一，Obsidian 自带 canvas 画布与 base 表格视图这类能力；其二，直接把 Obsidian 的库当成一个项目交给 Claude Code，思路跟前面练过的完全相通。

**2.1 准备：拿到仓库模板**

想顺顺当当跑起来，前期准备不能省，核心就是一份现成的仓库模板。

建议新开一个 Obsidian vault。这里有一份现成的知识管理模板，自己还没成体系的，可以直接拿它打底；用熟之后再按需要改目录。别的模板也行，重点是先跑起来。假如你本地已经堆了不少笔记，也可以让 Claude Code 借用卡片法、知识管理等思路，替你重新梳理一遍层级目录。

模板地址：https://github.com/MarsWang42/OrbitOS/blob/main/README_CN.md

在电脑上选个位置放它，然后在地址栏敲 powershell 回车，终端就出来了 ![](img/c49318ae702a9b273da9b1fd3c8f1fbc.png)，后面的步骤都要在里面敲。Mac 用户在目录上右键选终端打开即可；没这个选项的话，装个 iRightMouse。

**2.1.1 Windows 端怎么弄**

Windows 下那条命令多半跑不动，于是换成下载解压的路子。打开 https://github.com/MarsWang42/OrbitOS，找到下载按钮点下去 ![](img/a200b29eca4c6f7bad62254557bf600c.png)，下好之后解压 ![](img/2592891c3f7468dbdd27701cf27f1263.png)，把 CN 这个目录拷出来，它本身就是最终的 Obsidian 仓库 ![](img/19561b84af61358b26ecb895103c154a.png)；我把它改名叫 orbitos-vault ![](img/8eb674372d5b89cb69855d76b37d2d56.png)，你随意起名，用英文比较稳妥。

**2.1.2 Mac 端怎么弄**

Plain Text

```
npx degit MarsWang42/OrbitOS/CN orbitos-vault
```

把上面那条命令粘进终端，回车即可。

# Obsidian 第二大脑搭建实操

整段选中后原样粘贴，别逐字输入，数量也别增减。

Windows 快捷键是 Ctrl+V，Mac 快捷键是 Cmd+V。

![](img/739a844944af0658919b0f2a8ad14ad4.png)

当目录列表里冒出 orbitos-vault 文件夹，即完成拉取。

![](img/b99c8706e75a9f967895426a28337d20.png)

## 2.2 给 Obsidian 加装 Claudian 扩展

完成上述动作，orbitos-vault 中会看到类似下列文件：

![](img/f8200a3fb16635b5663435878ff0225f.png)

下一步要装一个 Obsidian 扩展，名字叫 Claudian。

💡有了它，Claude Code 就能在 Obsidian 里顺畅调用，右侧边栏直接开聊。

该扩展目前需手工部署，流程略绕，因此改由 Claude Code 代装。

![](img/8d2e48381745d7c1ac666f4758486aca.png)

终端弹窗后，把后续命令原样贴入，使 Claude Code 切到 yolo 模式：

Plain Text

```
claude  --dangerously-skip-permissions
```

![](img/0a3784fb2cd778bdcb38e3ff0d8034c9.png)

初次运行时屏幕会给出选项，选 yes 后敲回车。

![](img/b477c0729f3442772bd6a3451c1b0989.png)

再输入下列提示语，静候安装结束：

Plain Text

```
https://github.com/YishenTu/claudian
这个是 Obsidian 的插件，帮我安装到当前目录的 vault 下
```

![](img/56f7ff99d4ad168fb22fcc6350c54212.png)

看到末尾出现类似汇总的信息，说明部署完成。

![](img/75eec54503c8e19d35bb2ce90e888587.png)

现在调出预先备好的仓库位置。

![](img/c32b197442d1736b6d1ebd2cd2acebd5.png)

弹窗中按「打开」。

![](img/d00bfa2cb0bdb46c28fca70b82e83881.png)

将之前准备的那个目录选中。

![](img/d0b73f8661705075109f13c9beca1cae.png)

若出现插件信任弹窗，点选信任。

![](img/e8ebf959dadc654b3eaf9d47de2d4254.png)

进入下图页面，把 Claudian 的启用开关切到开。

![](img/71d0c6f71e380b15f545747f0ecadcdb.png)

关闭当前页，回到起始页，照图示继续。

![](img/491205da989ec2e61aa2145dd520d409.png)

若消息能正常返回，说明扩展可用。

Windows 系统还需多做一步：将 skills 文件夹复制到位。

![](img/3455e15c760c6b75db9f979a695d31ef.png)

![](img/b9583346c0d709c0709e5cc4a3c74d76.png)

![](img/9e79955cdfa1acd9ffe6738710cb4e72.png)

## 2.3 补齐 skills

第一步是把 skills 配给 Claude Code。

来源：https://github.com/kepano/obsidian-skills?tab=readme-ov-file

这套技能由 Obsidian 官方出品，可靠性有保障。

Plain Text

```
https://github.com/kepano/obsidian-skills
这个下面的 skills 帮我安装到这个项目下
```

截图：

![](img/733c813fde0ccdd72753e30b6c6f2755.png)

准备工作到此完毕，接下来可以折腾你的 Obsidian 大脑。

![](img/fae40898690cb1aee6467cd4e7f82a89.png)

## 3. Claude Code 搭配 Obsidian：入门玩法

💡下面这些案例用于带路。熟悉之后，完全能按个人偏好延展。Obsidian 可玩的方向多，Claude Code 作为通用 agent 能接的场景也多，组合后的空间很大，后续慢慢开发。

### 3.1 启动今日路线

操作不绕：自定义指令已就位，调用即可。

![](img/08ae8181c74b6f5f3061148685b5ead2.png)

关键是搜集材料；脑中冒出想法，就归入相应文件夹。

Plain Text

```
/start-my-day
```

今天的规划便由此展开。

![](img/0727407901547dadc0ae51e88eb6f3e3.png)

操作细节见图：

![](img/9d89148954cd488b8de8fc1352b66c82.png)

返回的结果：

![](img/03c374a8928b43d566147140af1b5020.png)

另会多出一篇 0305 日记。

![](img/8656025e0edcc3d2e1f6dae75e9f9da6.png)

灵感则落入收件箱，便于日后归档。

![](img/a958b31db3c266d1868843c05f6d6fff.png)

### 3.2 回看 2025

Plain Text

```
帮我回顾下 2025 的内容
```

![](img/c87cf34d0e24156b69d107aad2f52210.png)

归纳如下：

![](img/b0b9c6197e6a9715c83fba43bea2a456.png)

### 3.3 生成 canvas 画布

把下列提示语发出去：

Plain Text

```
帮我画一个明代的历史以及各个皇帝的canvas
```

![](img/d92deaa310bcafe95189cfb21f7baf48.png)

画布生成后可直接查看。

![](img/bd8f7c401ed843708bcfff3ee2de7546.png)

![](img/6813aff78c3965af0508a28ca159d3cc.png)

## 4. Claude Code 搭配 Obsidian：进阶玩法

仍以“第二大脑”为主线。第一步先判断目录是否趁手。

### 4.1 再盘一次目录

先回看下载的模板：https://github.com/MarsWang42/OrbitOS

其目录组织如下：

OrbitOS 自己设计了 **C.A.P 项目结构**（Context/Actions/Progress），知识面则划分为 Research（研究笔记）、Wiki（原子概念）、Resources（精选内容）三个层次。

![](img/ee9707a7e67ec856b548e51b7dfaac5c.png)

还可参考这个项目：https://github.com/heyitsnoah/claudesidian

其目录组织是：

Claudesidian 走经典 PARA 路线（Projects/Areas/Resources/Archive）。

![](img/f285444de05e61ca52be9be4fbd35653.png)

差别并不大。我让 Claude Code 做了对照归纳，供你参考。

![](img/2c873fcc0af4d4e82a48f8a81cb0e438.png)

比较后可见，各有长处。若你还没想好，先用 OrbitOS 的版本也成，之后随时能改。下面公开我的目录，供借鉴。我主要盯五件事：

1. 内容创作：主要阵地是🛰️公号、推特、YouTube、B 站。
2. 建站变现：聚焦 AI 产品、SaaS 服务。
3. 工具箱：收纳电脑软件与杂项资料。
4. 学习笔记：记录学到的知识。
5. 收藏箱：核心区域。🛰️文章、有价值的聊天记录、X 上的好帖，先收再理。

![](img/300be55a57e279ed0528b7a246c04d2e.png)

### 4.2 内容创作与分发

创作侧有两块：一是写稿、配📕图；二是内容外发，比如🛰️图文排版。下面分述。

#### 4.2.1 内容创作

思路取自「李默 AI 实战」这位号主的内容创作分享。做法很多，落点是用 AI 围绕选题产出稿子和图片，抽取环节交给 skills。提示词来自钱塘江鲤，已征得同意在此使用。

C++

```
/skill-creator
请你帮我创建技能：rewritepost
【核心功能】
根据用户输入的主题/内容，自动生成三种不同写作风格的文章，每篇配图，输出为Markdown文件，便于后续在 Obsidian操作。
【三种写作风格】
1. 娓娓道来风格 (narrative-style)
   - 占位提示词：{{NARRATIVE_PROMPT}}
   - 特点：温和、循序渐进、引导式叙述

&lt;!-- list-split --&gt;

1. 犀利点评风格 (critical-style)
   - 占位提示词：{{CRITICAL_PROMPT}}
   - 特点：观点鲜明、论证有力、批判性思维

&lt;!-- list-split --&gt;

1. 故事描述风格 (story-style)
   - 占位提示词：{{STORY_PROMPT}}
   - 特点：场景化、情节化、沉浸式体验
【执行流程】

1. 接收用户输入主题
2. 针对每种风格：
   a. 使用对应提示词生成文章内容（800-1500字）
   b. 提取文章核心概念，生成图片描述提示词
   c. 调用即梦 4.5 API生成配图
   d. 组装MD文档（标题+配图+正文+元数据）
3. 保存三个文件到当前目录

【图片生成配置】

API调用示例：

curl -X POST https://ark.cn-beijing.volces.com/api/v3/images/generations \
  -H &quot;Content-Type: application/json&quot; \
  -H &quot;Authorization: Bearer $ARK_API_KEY&quot; \
  -d &#x27;{
    &quot;model&quot;: &quot;doubao-seedream-4-5-251128&quot;,
    &quot;prompt&quot;: &quot;[根据文章风格动态生成的图片描述]&quot;,
    &quot;sequential_image_generation&quot;: &quot;disabled&quot;,
    &quot;response_format&quot;: &quot;url&quot;,
    &quot;size&quot;: &quot;2K&quot;,
    &quot;stream&quot;: false,
    &quot;watermark&quot;: true
}&#x27;【图片提示词生成规则】

- 娓娓道来风格：温暖色调、平和场景、教育感

- 犀利点评风格：对比强烈、视觉冲击、概念化

- 故事描述风格：戏剧性、情境化、细节丰富

【输出文件规范】

文件命名：

- {topic}_narrative.md

- {topic}_critical.md

- {topic}_story.md
```

在 Claudian 发出后，记录如下。

![](img/01ee70e0b12690131279a93a0b5f28c5.png)

最后会需要 key。前往：

https://console.volcengine.com/ark/region:ark+cn-beijing/model/detail?Id=doubao-seedream-4-5

按图点「API 接入」，再点「创建 API Key」。若已有，会展示现成 key，复制即可。

![](img/567ba9989188e2a4bc54bbe9ed8309ef.png)

把 key 贴进 Claudian 输入框，CC 会代为保存。

![](img/e5f6faa11bb95a1a45e7de0cedf882cd.png)

重启 Obsidian。调用 /rewirtepost，后接主题文章链接。

Markdown

```
/rewritepost https://claude.com/blog/1m-context-ga
```

![](img/a1341f949be00ea139d59a9854e37499.png)

当前成品有封面和文字，后续还能优化 skills，让正文中也插图，留给大家继续研究。

#### 4.2.2 平台分发

稿件完成后要发🛰️。这里以🛰️图文为例，仍借 skills 完成。

💡为什么用 skills：

1. 比插件更灵活，遇到问题或要微调，自己改即可。
2. 与 Claude Code/Codex 搭配更聪明。

要装前面说过的 baoyu-skills，里面已有🛰️图文发布技能，也带🧣、X 等渠道，可自行尝试。

下面用🛰️图文发布做演示。先装 skills，把提示词发到 Claudian。

Markdown

```
帮我安装下面的 skills 到这个项目级别
https://github.com/JimLiu/baoyu-skills
```

![](img/fc76fd06b9d1dd20ed53e0991f284014.png)

装好后，用提示词让 Claude Code 执行发文。

Markdown

```
@claude-1m-context_story.md 这篇文章发送到公众号草稿箱
```

届时会问 AppID 与 AppSecret，按手册操作。

![](img/0a0253b37e71176334a898401304faf3.png)

在🛰️公众平台里进「账号设置」，AppID 可见，AppSecret 却不见踪影——它被挪到另一处。

![](img/7d19b1fe44829840cb010fffc6bd0501.png)

去🛰️开发者平台 https://developers.weixin.qq.com ，点👸号进入。

![](img/0a6e21840fbde8b9924852f3ed7c864d.png)

下图处可看到 AppSecret。首次需激活。注意只展示一次，第一次复制后务必存好；再打开无法复制，只能重置，忘了也只能重置。

![](img/90da345486bec53393831c1880269011.png)

再用 VSCode 打开仓库下的 .baoyu-skills，按图操作，最后记得存盘。模板里把 {xxx} 换成自己的内容，括号也全部替换。

Markdown

```
WECHAT_APP_ID={换成你的 app id}
WECHAT_APP_SECRET={换成你的 app Secret}
```

![](img/cf77f929bbc84e983cc5bb2de04915be.png)

存盘后回到 Claudian 窗口，继续发文即可。

### 4.3 知识沉淀

沉淀内容有一部分来自收藏：🛰️文章、有价值的对话、网页等。这里主要说「收藏箱」。

#### 4.3.1 浏览器收藏

装个扩展即可。在 Chrome 应用市场搜 Obsidian Web Clipper，安装即可。

![](img/551ffea4fa50b32a1d3bce7bedf4da16.png)

用法：网页打开后想收藏，点扩展图标即可。

**网页和🛰️文章，一键收藏进 Obsidian（附 OpenClaw 命令）**

打开某个网页时，剪藏插件会显示出该站点的摘要信息，有些页面甚至连正文都能完整抓出来。看到想要的内容，直接点击「Add to Obsidian」按钮即可。

![](img/bb6c8a1eed7448baface0c729292fb68.png)

这时系统会引导你唤起 Obsidian 应用。

![](img/4a60eaf54842e2ccb6db5e89023d2b1c.png)

随后内容就会被存入 Obsidian。默认归档目录是 Clippings，如果不想放在这里，你也能自己改：找到插件设置里对应的目录项，替换成想要的路径就行。

![](img/b87d8da603de3613d605c506376269f1.png)

**4.3.2 🛰️文章收藏**

接下来聊聊👸号文章和🛰️消息的收藏。我用的方案是 MpClipper 插件：只要把需要保留的文章、信息或链接，直接丢进 MpClipper 对话框。

![](img/935f5d7bff4910130696be6dacc668b5.png)

同时在 Obsidian 里装上 MpClipper Sync 插件，👸号内容就可以自动同步到指定目录。

![](img/72557273702bc80e7d4cd25ce419934a.png)

我这边同步到了「90.收藏箱/🛰️剪藏」这个路径，还可以按时间自动归档。

![](img/03c2189ffdff8df131ba2da036e7a2dd.png)

下面把配置步骤拆开细说。过程稍微繁琐，耐心一点就能搞定。

💡 提醒：MpClipper 有 30 次免费收藏额度，超出额度需要付费，介意的朋友注意一下。

**🔧 第一步：小程序端配置**

先在🛰️里搜索「NotionMpClipper」小程序并打开。

1. 进入【我的】-【Obsidian】页面，按照页面提示设置图床。支持阿里云、腾讯云、缤纷云、Cloudflare R2，以及其他兼容 S3 协议的对象存储服务。

![](img/660f9a99c854ab7f59e88a62dcaa2814.png)

![](img/f6290e138b5b76bd5b6b3004669554cc.png)

- 会员权限：想要使用需要开通会员。
- 图床可以选缤纷云（bitiful.com 有 50G 免费额度），腾讯云、阿里云也都可以。
- 打开「保存到 Obsidian」开关：在【我的】-【个性设置】页面中，把这个开关开启。

![](img/3cabf5bb2057cb1fed48a090fcd92e50.png)

**💻 第二步：Obsidian 插件安装**

安装包下载入口：

![](img/246675fa31e37c67e5328d91bae926e3.png)
mpclipper-sync(1).zip（下载地址：https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/CnT8bh6FzoZeLFxoJe1cQ465ndh?response-content-disposition=attachment%3B%20filename%3D%22mpclipper-sync%281%29.zip%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260526%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260526T134041Z&x-oss-expires=86400&x-oss-signature=4d1b27630d2b18cb403badb82ef73bcc25d67d26626c6cb933d62525ac3809e0&x-oss-signature-version=OSS4-HMAC-SHA256）

下载后导入 Obsidian 并完成配置。另外，小程序【我的】-【Obsidian】页面里提供了一键复制配置的按钮：复制后先存到记事本，再粘贴到 Obsidian 插件的配置表单中，非常省事。

![](img/9696a5acb7a8255026d0396626b2fc41.png)

**⚠️ 第三步：图床 CORS 配置**

这一步容易踩坑：无论你用哪家图床，都需要去图床平台开启 CORS 跨域配置。比如我这边用的就是缤纷云（https://www.bitiful.com/）。

![](img/435b06ca2b66b03519e83e5d4bae8b88.png)

缤纷云的设置方式可以参考截图，其他图床的配置思路一致。搞定这些后，后续剪藏流程照旧：把文章链接发给小程序，或者用🛰️收藏助手剪藏，都可以。

**请注意**：开启 Obsidian 剪藏后，Notion 剪藏会自动关闭；反过来也一样。两者互斥，你随时可以在设置中切回来。

最后附上 OpenClaw 的安装命令，需要的话自取：

```
## 五、OpenClaw 的拓展玩法

### 01. OpenClaw 本地部署（有风险，谨慎尝试）

1.OpenClaw 支持的平台

OpenClaw 可以运行在所有主流操作系统上，配套 App 提供语音、摄像头等额外能力。

| 平台 | Gateway 支持 | 配套应用 |
| --- | --- | --- |
| macOS | 原生支持 | 原生支持最完善，可操作日历、备忘录、截图等系统功能 |
| Windows | 支持（强烈推荐 WSL2） | 完全可用，但部分系统集成功能受限 |
| Linux | 原生支持 | 适合开发者，配置灵活 |

**Gateway 服务安装方式**

Gateway 作为后台服务运行，有多种安装方式：

| 方式 | 命令 | 说明 |
| --- | --- | --- |
| 向导安装（推荐） | openclaw onboard --install-daemon | 一站式完成配置和服务安装 |
| 直接安装 | openclaw gateway install | 仅安装服务，不运行配置向导 |
| 配置流程 | openclaw configure | 在配置流程中选择安装 Gateway 服务 |
| 修复/迁移 | openclaw doctor | 自动检测并修复服务问题 |

服务注册方式因操作系统而异：

• macOS: LaunchAgent(ai.openclaw.gateway)

• Linux / WSL2：systemd 用户服务（openclaw-gateway.service）

2.安装环境准备

本地安装建议小龙虾运行环境与本机隔离，所以推荐虚拟机方式安装，虚拟机可以随时备份、删除和恢复，即便我们把小龙虾玩坏了也可以快速恢复。

Windows 推荐用 Vmware 或者 VirtualBox（开源免费）Windows 也可以安装 WSL 想当于在 Windows 上安装了一个 Linux 虚拟机

![](img/f68e7661ae0f9753913bdd32ab53ca9d.png)

Mac 就推荐 小龙虾官方推荐的 lume 好像也是免费的

**Windows 用户：什么是 WSL2？如何安装？**

WSL2（Windows Subsystem for Linux 2）让你在 Windows 上运行完整的 Linux 环境。如果你不想折腾，直接用 PowerShell 即可，跳过此步骤。

1. 以管理员身份打开 PowerShell

2. 运行：wsl --install

3. 重启电脑，按提示设置用户名和密码

之后在开始菜单搜索&quot;Ubuntu&quot;即可打开 WSL2 终端，使用上面 macOS / Linux 的安装脚本。

具体安装命令可以参考官方文档：[https://docs.openclaw.ai/install#from-source](https://docs.openclaw.ai/install#from-source)

安装版本我们统一用 3.11 版本

Ada

```text
npm install -g openclaw.3.11
```

3.Windows 环境安装

打开 Powershell，输入安装命令， 因为前面我们在课前准备都安装好了 Node 环境，所以这里也可以通过 NPM 方式安装

一键安装脚本

Ada

```
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
iwr -useb https://openclaw.ai/install.ps1 | iex
```

![](img/e5fc8f98838b7d6ef0f1d1002afaedc7.png)

Nodejs 安装命令

Ada

```
npm install -g openclaw.3.11
openclaw onboard --install-daemon
```

![](img/efd11a90bc45b12bd6db5de9c6a19e84.png)

安装完成之后，下一步我们来初始化一下配置

首先配置 AI 模型，OpenClaw 本身不包含 AI 大脑，需要连接一个"模型提供商"来获得智能。如果安装脚本已启动了配置向导，按下方说明填写即可；如果跳过了向导，手动运行

Ada

```
openclaw onboard --install-daemon
```

然后选择继续

![](img/1e61c5ac007dc783c8f2ea62068e1444.png)

选择快速开始

![](img/2b2135070b42a20af6ca50b6c8f2653f.png)

模型配置这里先跳过，等会我们后台配置

![](img/842a5408f4dd630e0f49d928d5f54af2.png)

供应商筛选选择 All

![](img/4500a1d85436124591e3d92e28767be5.png)

默认模型选择默认

![](img/586cc2774e21de72f37cbfd33279dc8f.png)

对话去掉我们选择飞书，除非你想配置其他平台

![](img/a72a075faa8b1e521d3ea188c4ba9249.png)

确认安装飞书插件

![](img/c5c83b723ad96d3ede6f5c3de5b831cc.png)

这里需要我们现在飞书开放平台创建一个 APP， 给这个应用配置 IM 权限，然后把 APP ID 和 APP Secret 复制到这里

![](img/c5caef8315e1abc20d5d91b87313dc8a.png)

到飞书开放平台创建一个应用，https://open.feishu.cn/app

![](img/11e091efd7be1ec093e105f10a226ee4.png)

给应用起个名字

![](img/288be20c06e7acf2f813b1d9af667e6b.png)

到 凭证与基础信息 菜单 ，复制 APP Id 和 APP Secret

![](img/7e7013bcab4dc640de04f925066d94a4.png)

下一步选择 WebSocket 链接方式

![](img/360fd799340cd473d9f05241681fe4ac.png)

这里你用的国内版 就选飞书，如果是国际版就选 lark

![](img/cd74deb6bee819a58ee7d8fc69b26d9e.png)

然后选择群聊策略，只允许特定群可以跟小龙虾对话，还是所有群， 默认选所有就行

![](img/78eb985f52c4485e1a98cb6b4c3e8aa6.png)

下一步配置联网搜索，可以先跳过，后面再配置

![](img/b8d3cb9f73b11444216c96c952755f81.png)

是否配置 Skills， 选 yes

![](img/ab102a3a1da7f2075dd54cf20744c6ab.png)

根据你的需求选择要安装的 Skill， 如果要生图可以安装 Nano Banana Pro， 要调用 Gemini 就选 Gemini

![](img/b5cae7aa4cbb3fe22d8f4ef6c084a428.png)

报管理工具就选 npm， 我们一直都是用 npm

![](img/f1905607aa49edc94b8caee4d2856d4f.png)

然后等待从 ClawHub 安装

![](img/7d13c1781f99495a5874edb2c8ea31e2.png)

安装失败了就跳过，这个不影响，后面可以重新安装

然后就可以看到安装完成的配置，这里是 WebUI 的地址

![](img/b64b1e1995e8eb6734781df1f443585b.png)

如果我们安装过程中遇到任何问题，可以直接让 CC 解决

然后在浏览器看到这个 WebUI， 就说明安装成功了

![](img/7be052c510ac6da2df4f9a1b81873046.png)

4.Mac 环境安装

Mac 环境安装就比较丝滑了，Macmini 应该是运行小龙虾运行最佳选择，性能高耗电低。

同样我们可以在 Mac 上可以安装多个虚拟机，同时运行多个小龙虾实例，互不干扰。

这样你将获得：

• 完全隔离的 macOS 环境（你的宿主机保持干净）

• 通过 BlueBubbles 获得 iMessage 支持（在 Linux/Windows 上无法实现）

• 通过克隆 VM 实现即时重置

• 无需额外硬件或云成本

**你需要准备的内容（Lume）**

• Apple Silicon Mac( M1/M2/M3/M4)

• 宿主机运行 macOS Sequoia 或更高版本

• 每个 VM 大约 60 GB 可用磁盘空间

• 约 20 分钟

首先我们安装虚拟机， 使用[Lume](https://cua.ai/docs/lume/guide/getting-started/introduction)在你现有的 Apple Silicon Mac 上的沙箱化 macOS VM 中运行 OpenClaw。

Ada

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/trycua/cua/main/libs/lume/scripts/install.sh)"
```

如果~/.local/bin不在你的 PATH 中：

Ada

```
echo 'export PATH="$PATH:$HOME/.local/bin"' >> ~/.zshrc && source ~/.zshrc
```

验证：

Ada

```
lume --version
```

创建 macOS VM

Ada

```
lume create openclaw --os macos --ipsw latest
```

这会下载 macOS 并创建 VM。VNC 窗口会自动打开。

注意：下载可能需要一些时间，具体取决于你的网络连接。

安装完之后，进行系统初始化设置

在 VNC 窗口中：

1.  选择语言和地区

1.  跳过 Apple ID（或者如果你之后想使用 iMessage，也可以登录）

1.  创建一个用户账号（记住用户名和密码）

1.  跳过所有可选功能

设置完成后，启用 SSH：

1.  打开“系统设置”→“通用”→“共享”

![](img/9e1567e755d689b33a0dc3bdfc6d4250.png)

1.  启用“远程登录”

![](img/cfad27099023bbd971a88ecd0cdac12c.png)

获取 VM 的 IP 地址

Ada

```
lume get openclaw
```

查找 IP 地址（通常为192.168.64.x）

![](img/4d5a8661e98074c306e77d925e8ac8b9.png)

通过 SSH 登录 VM

Ada

```
ssh youruser{"id":117325,"name":"锋度","xq_group_number":192,"avatar":"https://search01.shengcaiyoushu.com/upload/avatar/FpBm3I9cPVn9OGK9x22S3md6Eahb"}.168.64.X
```

将youruser替换为你创建的账号，并将 IP 替换为你的 VM IP。

![](img/543cb4695c4e3932f3fdb9b3eb1c53e1.png)

安装 OpenClaw

Ada

```
npm install -g openclaw.3.11
openclaw onboard --install-daemon
```

![](img/2c21cc0898798e0e4e310caa53a0964d.png)

然后初始化配置跟 Windows 都是一样的，就不赘述了

![](img/9e964bca8056779890d1292df75dccf0.png)

5.大模型配置

前面安装的时候我们没有配置大模型，那是因为需要在后台配置比较方便，安装完成之后 OpenClaw 应该会返回 WebUI 的地址，http://127.0.0.1:18789， 如果没显示我们也可以通过命令来查看

Ada

```
openclaw dashboard

waoowaoo 部署：四关跑通故事到成片

想把一段文字故事变成分镜、画面、配音，最后拿到能下载的视频文件，waoowaoo 给了一条可验收的路径。它把生成过程切成四个节点，每完成一段都有明确产物，执行时不容易迷失方向。

先准备命令行工具：

```

![](img/40426edfeaaa6c61e883aec1d74ee14d.png)

然后打开这个 WebuUI 就代表安装成功了

![](img/0501c28797856335f28c42a870455019.png)

在配置之前，我们需要准备好一个 GLM 的编程套餐

![](img/45f81db469676902b621a4d4e540fded.png)

进入 OpenClaw 的管理页面，打开 Config 设置，点击 Models 修改模型配置。添加一个模型提供商glm，填写 API 调用配置，包括 API 接口类型、API 密钥和调用地址 Base Url。

注意 Base Url 的配置：

使用[GLM 编码套餐](https://docs.bigmodel.cn/cn/coding-plan/overview)[时，需要配置专属的 Coding 端点http](https://open.bigmodel.cn/api/coding/paas/v4)s://open.bigmodel.cn/api/coding/paas/v4

否则，使用通用端点[https://open.bigm](https://open.bigmodel.cn/api/paas/v4/)odel.cn/api/paas/v4/

![](img/0f7f5d8559cdb953129c1ba33e2f8ccf.png)

![](img/0c87d0f5640680e5871b648af119f611.png)

然后，在 glm 模型提供商中添加一个要调用的大模型，注意模型名称填写准确，完成后点击 Save 按钮保存。

![](img/88a6f059a1a53302ef1efc7ff17b1f12.png)

![](img/8b6dc4cc819c5c971d6672fbe828e9d0.png)

最后，在 Agents 设置中修改智能体使用的默认模型，记得保存：

![](img/b765e44ef2b8362acddd4b42457d3909.png)

然后我到 chat 界面，和 AI 打个招呼

![](img/a26ce543d967b86353e870423f330e0b.png)

6.飞书渠道配置

用[小](https://www.feishu.cn/content/article/7613711414611463386)龙虾自带的飞书渠道配置相当复杂，要配置事件回调、权限等，飞书官方开发了小龙虾插件，直接扫码一键创建应用，相当丝滑，具体可以查看飞书文档：https://www.feishu.cn/content/article/7613711414611463386

安装飞书插件

Ada

```

接下来是四个验收节点，流程图如下：

```

安装之后，插件会自动检测是否有已经配置的应用，这里我们选否，要重新创建才能用二维码绑定

![](img/005da2a7687d79f9db8653e053694ee2.png)

![](img/3d9ba0e80a1e2b16404d4c10714fa64d.png)

### 02.用 OpenClaw 生成 AI 漫剧

全程大概 80 分钟。但你真正动手的时间只有 20 分钟，剩下全是等 AI 干活。你只需要负责写故事和复制粘贴命令，AI 负责画画、配音、做动画。

这意味着什么？

如果你是做自媒体的，一个下午能量产 3 到 5 条。故事素材从网文、童话、民间传说里随便找，AI 帮你搞定画面、声音、动画。成本就是 API 调用费，一条视频几块钱。

我们这里会用到一个 waoowaoo 的开源工具（GitHub 快一万 Star 了），这个开源只专门干一件事：把故事变成 AI 漫剧。

它把"写故事 → 画分镜 → 生成图片 → 配音 → 生成视频 → 合并"这一整条流水线全串起来了。你不需要自己去拼各种工具。

而且它有网页界面，也支持命令行。咱们这个教程走命令行——好处是每一步都能复制、能自动化。跑通一次，下次换个故事再来一遍就行。

**你需要准备什么？**

| 准备项 | 说明 | 预计耗时 |
| --- | --- | --- |
| 一台云服务器（VPS） | 最低 2 核 4GB 内存，40GB 硬盘，Linux 系统 | 买一台约 5 分钟 |
| 火山引擎账号 | 生成图片和视频用的（Seedream 画图 + Seedance 做动画） | 注册约 10 分钟 |
| Google AI 账号 | 故事分析用的（Gemini 帮你理解角色和场景） | 注册约 5 分钟 |
| FAL.ai 账号 | 生成配音用的（Index TTS 2 能克隆声音） | 注册约 3 分钟 |
| 一段故事 | 100-300 字，建议 2-4 个角色，场景别太跳 | 你自己定 |

关于服务器位置，这里有个坑。

因为要调 Google 的 Gemini API，国**内服务器是连不上** Google 的。所以建议买海外服务器，比如日本、新加坡、美国的 VPS。不然到"故事分析"那步就直接卡死。

费用大概是：海外 VPS 30-50 元/月，API 费用一条视频 3-8 元。

**全流程长什么样？**

整个过程分四个阶段。每个阶段做完，你都能看到一个明确的东西——不是那种"做完了但不知道做没做对"的状态。

Plain Text

```

这四个节点的判断标准可以这样理解：首页能打开且接口状态正常；AI 已经拆出角色与画面描述；首张漫画图和角色配音出现；完整 MP4 成功下载。每一步都有可见结果，按顺序推进即可。

部署到服务器时，先登录主机：

```

耗时参考：

| 阶段 | 你动手 | 等 AI |
| --- | --- | --- |
| 环境准备 | 约 20 分钟 | — |
| 故事变分镜 | 约 5 分钟 | 约 5 分钟 |
| 分镜变画面和声音 | 约 10 分钟 | 约 15 分钟 |
| 画面变完整视频 | 约 5 分钟 | 约 60 分钟 （最长，可以去干别的） |

第一阶段：环境准备

这个阶段做完，你会看到 waoowaoo 的界面跑起来了，三个 AI 服务全部连接正常。

相当于把工作台搭好，工具摆上去，确认每个都能用。

1.1 部署 waoowaoo 到服务器

**先连上你的服务器。**

打开电脑上的终端（Mac 搜"终端"，Windows 按 Win+R 输入cmd），敲这行：

Bash

```

然后执行安装脚本：

```

回车，输密码。看到类似root@server:~#的东西，就进去了。

连不上？先看看 IP 有没有打错。提示Connection refused的话，多半是服务器的 22 端口没开，找你的 VPS 服务商开一下就行。

**然后一键装 waoowaoo。**

把下面这行复制粘贴进去，回车：

Bash

```

装好后查看容器状态：

```

脚本会自动帮你装 Docker、下载 waoowaoo、把所有服务拉起来。大概 3-5 分钟。

装的过程中会问你几个问题，一路回车就行。装完会告诉你访问地址。

如果你的服务器已经装过了，跳过安装，直接确认服务还活着：

Bash

```

若容器尚未运行，再补一条启动命令：

```

看到所有服务状态都是Up或running就行。有没跑起来的：

Bash

```

接着在浏览器打开服务地址：

```

**打开浏览器看看。**

在你自己的电脑上，浏览器访问：

Plain Text

```

进入页面后先完成身份验证。将示例邮箱与密码改成个人凭据，再执行认证：

```

看到 waoowaoo 的登录页面，说明部署成功了。

**注册一个账号。**

在登录页点"注册"，设一个邮箱和密码。

记住这个邮箱和密码，后面命令行登录也得用。

1.2 获取三个 API Key

API Key 是什么？

打个比方。你去一家餐厅吃饭，得先办一张会员卡。waoowaoo 就是那个帮你点菜的服务员，但它得拿着你的会员卡才能去后厨（AI 服务）帮你下单。

每个 AI 服务都要注册一个账号，然后找到"API Key"那个页面，复制一串密码出来。

火山引擎 ARK（画图 + 做视频用的）

1.  打开 https://www.volcengine.com/ ，点"立即注册"

1.  手机号注册，设密码

1.  **实名认证**——这步不能跳，不然啥也用不了。进控制台后会提示你，选"个人认证"，微信或抖音扫码刷脸就行

1.  进控制台，找到**"火山方舟"**（直接访问 https://console.volcengine.com/ark ）

1.  **左边菜单点**"API **Key 管理"** →"创建 API Key"

1.  复制保存（长得像xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx）

1.  **充值**：右上角"费用中心"→ 充值。建议先充 50 块试试水，支付宝微信都行

新用户有免费额度（50 万 tokens/天），但图片和视频生成要另外花钱。

Google AI（分析故事用的）

1.  打开 https://aistudio.google.com （得能上 Google）

1.  用 Gmail 账号登录

1.  同意服务条款

1.  左边菜单点**"Get API key"**（或者直接 https://aistudio.google.com/app/apikey ）

1.  点**"Create API key"**，选个 Google Cloud 项目（没有就建一个）

1.  复制保存（长得像AIzaSy...）

免费的。不用绑信用卡，有每日限额但做教程够用。

FAL.ai（配音用的）

1.  打开 https://fal.ai ，邮箱注册

1.  进 Dashboard，左边点**"API Keys"**（或者直接 https://fal.ai/dashboard/keys ）

1.  点**"Add Key"**，起个名，点**"Create Key"**

1.  复制保存

新注册有免费额度。配音价格大概 $0.002/秒，一条 2 分钟视频的配音成本不到 1 块钱。

1.3 在 waoowaoo 里配置 API Key

三把钥匙拿到手了，现在得告诉 waoowaoo 怎么用它们。

方式一：网页界面配（推荐，简单）

1.  浏览器打开http://你的服务器IP:13000，登录

1.  进**"设置中心"**（Settings）

1.  找到这三个服务商，把对应的 Key 粘进去：

◦

**火山引擎 Ark**：粘你的 ARK API Key

◦

**Google**：粘你的 Gemini API Key

◦

**FAL**：粘你的 FAL.ai API Key

1.  每个填完点**"测试连接"**。看到绿色的"连接成功"就对了

方式二：命令行配（网页打不开的备选）

先登录拿凭证：

Bash

```

验证通过后，写入三家服务商的密钥：火山引擎 Ark、Google、FAL。示例值只是占位，记得换成自己的：

```

然后配 Key：

Bash

```

全部配置完成后做一次体检。脚本会检查 curl、python3、docker、ffmpeg 是否可用，并确认服务能否正常响应：

```

1.4 环境检查

正式开干之前，跑一下这个，确认工具都在：

Bash

```

如果提示 ffmpeg 缺失，补装：

```

ffmpeg 没装的话：

Bash

```

最后再确认一次登录状态，方便后续请求携带身份：

```

全部 ✅？可以了，进入下一阶段。

![](img/b6237a5902064b94077f92de3de64e5b.png)

第二阶段：故事变分镜

这个阶段，AI 会"读"你的故事，分析出里面有哪些角色、每个场景发生了什么，然后把故事切成一个个画面，告诉画图 AI 每张图该画什么。

打个比方：你把一篇小说递给一个插画师，让他先通读一遍，在每个关键情节旁边标注"这里画什么"。这步就是让 AI 干这个活。

2.1 命令行登录

如果你在 1.3 已经用命令行登录过，而且终端窗口没关过，这步跳过。

Bash

```

整个流程的关键在于确认服务能正常响应、首页与接口都状态无误，然后按照四个节点继续生成。服务器 IP、邮箱、密码以及三家平台的密钥都要替换成自己的，按顺序执行，就能从故事一路做到成片。

# AI 漫剧全流程：从建项目到出图

想把一个故事自动跑成漫剧？下面这条链路会把项目、剧集、故事分析、片段切分、分镜和图片生成串起来。关键 ID 都会落盘保存，终端断开也能接着往下做。

## 先建项目，再把 ID 存好
```

这个命令干了什么事呢？它在/tmp/auth_cookies.txt里存了一张临时"身份证"。后面每个命令都会带着这张身份证去请求。

关了终端窗口重新连的话，这张身份证就作废了，得重新跑一遍这个登录。

2.2 创建项目

Bash

```
```bash
PROJECT=$(curl -s -b /tmp/auth_cookies.txt \
  -X POST http://localhost:13000/api/projects \
  -H "Content-Type: application/json" \
  -d '{"name": "我的第一条AI漫剧", "description": "第一次尝试"}')

PROJECT_ID=$(echo $PROJECT | python3 -c "import json,sys; print(json.load(sys.stdin)['project']['projectId'])")

echo "✅ 项目已创建，项目 ID：$PROJECT_ID"

# 写入会话文件，防止终端断开后找不到
echo "PROJECT_ID=$PROJECT_ID" > /tmp/waoowaoo_session.env
```

这里用登录 cookie 调创建项目接口，项目名和描述可以按需替换。拿到 `projectId` 后马上写进会话文件，后面所有操作都靠它定位项目。

## 找回项目 ID
```

我的第一条AI漫剧你可以换成自己喜欢的名字。

**终端断开了怎么办？**

别慌。重新连上后先跑登录命令，然后：

Bash

```
```bash
# 方式一：之前存过环境文件
source /tmp/waoowaoo_session.env
echo $PROJECT_ID

# 方式二：列出全部项目
curl -s -b /tmp/auth_cookies.txt http://localhost:13000/api/projects | python3 -c "
import json,sys
for p in json.load(sys.stdin)['projects']:
    print(p['projectId'], p['name'])
"

# 找到后手动赋值：PROJECT_ID=对应ID
```

如果终端重开，先 `source` 之前的环境文件；忘了 ID 就拉项目列表，按名称找到对应 ID 再手动设置。

## 建第一集并保存剧集 ID
```

2.3 创建剧集并写入故事

**先创建一个剧集。**

Bash

```
```bash
EP=$(curl -s -b /tmp/auth_cookies.txt \
  -X POST "http://localhost:13000/api/novel-promotion/$PROJECT_ID/episodes" \
  -H "Content-Type: application/json" \
  -d '{"name": "第一集"}')

EPISODE_ID=$(echo $EP | python3 -c "import json,sys; print(json.load(sys.stdin)['episode']['id'])")

echo "✅ 剧集已创建，剧集 ID：$EPISODE_ID"

# 追加保存
echo "EPISODE_ID=$EPISODE_ID" >> /tmp/waoowaoo_session.env
```

在项目下创建“第一集”，从返回结果里取出 `episode.id`，再追加到同一个会话文件，方便后续步骤直接复用。

## 准备故事文本
```

**然后写你的故事。**

用nano打开一个文件：

Bash

```
```bash
nano /tmp/story.txt
```

把故事写进 `/tmp/story.txt`，后面会直接读取这个文件。示例故事可以改成下面这样：

```

把你的故事粘贴进去。下面是示例，你换成自己的就行：

Plain Text

```
老森林的边上，小狐狸阿金安了家。它有一身橙红色的毛，尾巴蓬松得像一团大毛球。阿金最喜欢的时刻，是傍晚坐在大石头上看夕阳发呆。

一天傍晚，小松鼠跑得气喘吁吁，冲它喊：“阿金阿金！林子深处有一棵会讲话的树，你敢去瞧瞧吗？”

阿金歪头想了想，笑道：“敢啊！不过咱们得捎上蜂蜜饼干，说不定那棵树也馋甜口。”

于是两个小家伙出发了，走进一段谁也不知道结局的冒险。

## 把故事写入剧集
```

粘贴完，按**Ctrl+O**保存 →**回车**确认 →**Ctrl+X**退出。

几个写故事的建议：

• 100-300 字最好。太长的话生成时间翻倍，你等得烦

• 2-4 个角色就够了。角色越多，后面配音越麻烦

• 场景别太跳。一会儿森林一会儿太空，画风容易崩

• 可以写对话，AI 会自动识别谁在说什么

**最后把故事写入项目。**

Bash

```
```bash
STORY_TEXT=$(cat /tmp/story.txt)

curl -s -b /tmp/auth_cookies.txt \
  -X PATCH "http://localhost:13000/api/novel-promotion/$PROJECT_ID/episodes/$EPISODE_ID" \
  -H "Content-Type: application/json" \
  -d "{\"novelText\": $(python3 -c "import json; print(json.dumps(open('/tmp/story.txt').read()))")}" > /dev/null

echo "✅ 故事内容已更新"
```

读取故事文件内容，用 `PATCH` 请求更新剧集的 `novelText` 字段。文件内容先经 `json.dumps` 转义，避免引号破坏 JSON 结构。

## 触发故事分析并等待
```

2.4 让 AI 分析故事

接下来让 AI "读"你的故事。它会分析出有哪些角色、长什么样、每个场景在讲什么。

Bash

```
```bash
echo "⏳ 正在让 AI 读故事..."
TASK=$(curl -s -b /tmp/auth_cookies.txt \
  -X POST "http://localhost:13000/api/novel-promotion/$PROJECT_ID/analyze-global" \
  -H "Content-Type: application/json" \
  -d "{\"episodeId\": \"$EPISODE_ID\", \"locale\": \"zh\"}")

TASK_ID=$(echo $TASK | python3 -c "import json,sys; print(json.load(sys.stdin).get('taskId','?'))")

# 最多轮询 3 分钟
for i in $(seq 1 36); do
  sleep 5
  STATUS=$(curl -s -b /tmp/auth_cookies.txt "http://localhost:13000/api/tasks/$TASK_ID" | python3 -c "import json,sys; print(json.load(sys.stdin).get('task',{}).get('status',''))")
  if [ "$STATUS" = "completed" ]; then echo "✅ 故事分析完毕！"; break; fi
  if [ "$STATUS" = "failed" ]; then echo "❌ 分析未成功：请确认 Google API Key 配置无误，并检查服务器能否访问 Google"; break; fi
  echo "  继续等待... ($i/36) 当前状态：$STATUS"
done
```

提交全局分析任务，拿到 `taskId` 后每 5 秒查一次状态。成功会提示完成；失败则重点检查 Google API Key 和服务器访问 Google 的网络情况。

## 切分故事片段
```

失败了？十有八九是 Google API 连不上。检查一下你的服务器是不是在海外，或者有没有配代理。

2.5 生成片段

AI 读完故事后，要把故事切成一个个小片段。每个片段对应一张图。

Bash

```
```bash
echo "⏳ 开始拆分故事片段..."
CLIP_RESULT=$(curl -s -b /tmp/auth_cookies.txt \
  -X POST "http://localhost:13000/api/novel-promotion/$PROJECT_ID/clips" \
  -H "Content-Type: application/json" \
  -d "{\"episodeId\": \"$EPISODE_ID\", \"locale\": \"zh\"}")

# 等待片段产出
for i in $(seq 1 12); do
  sleep 5
  CLIP_COUNT=$(curl -s -b /tmp/auth_cookies.txt \
    "http://localhost:13000/api/novel-promotion/$PROJECT_ID/episodes/$EPISODE_ID" | \
    python3 -c "import json,sys; d=json.load(sys.stdin); print(len(d.get('episode',{}).get('clips',[])))" 2>/dev/null)

  if [ "$CLIP_COUNT" != "0" ] && [ -n "$CLIP_COUNT" ]; then
    echo "✅ 片段切分完成，共 $CLIP_COUNT 段"
    break
  fi
  echo "  仍在等待... ($i/12)"
done
```

调用片段切分接口后，轮询剧集详情里的 `clips` 数量。只要片段数不为 0，就说明切分完成。

## 生成分镜
```

这步特别容易被跳过。但你不能跳——不做这步，下一步会直接报错No clips found。别问我怎么知道的。

2.6 生成分镜

现在 AI 要给每个片段写一份"分镜"：这张图画什么构图、什么角色、什么表情动作。

就像导演拿着剧本画分镜头脚本。AI 就是那个导演。

Bash

```
```bash
echo "⏳ 正在产出分镜，大约需要 2 分钟..."
TASK=$(curl -s -b /tmp/auth_cookies.txt \
  -X POST "http://localhost:13000/api/novel-promotion/$PROJECT_ID/script-to-storyboard-stream" \
  -H "Content-Type: application/json" \
  -d "{\"episodeId\": \"$EPISODE_ID\", \"locale\": \"zh\"}")

TASK_ID=$(echo $TASK | python3 -c "import json,sys; print(json.load(sys.stdin).get('taskId','?'))")

for i in $(seq 1 36); do
  sleep 5
  STATUS=$(curl -s -b /tmp/auth_cookies.txt "http://localhost:13000/api/tasks/$TASK_ID" | python3 -c "import json,sys; print(json.load(sys.stdin).get('task',{}).get('status',''))")
  if [ "$STATUS" = "completed" ]; then echo "✅ 分镜已生成！"; break; fi
  if [ "$STATUS" = "failed" ]; then echo "❌ 分镜生成失败，请重新执行本步骤"; break; fi
  echo "  等待中... ($i/36) 状态：$STATUS"
done
```

把脚本转成分镜同样走任务轮询。完成就进入出图；失败则重新运行本步骤。

## 提交图片生成
```

![](img/fb2cf072a4fc6c31bcbc9a84f547f8db.png)

第三阶段：分镜变画面和声音

这个阶段结束后，每个分镜都会有一张漫画图片，每个角色都有了自己的声音。

如果说上一步是导演画分镜，这一步就是画师照着分镜一张一张画，配音演员照着台词一句一句录。只不过画师和配音演员都是 AI。

3.1 生成所有图片

每张分镜会发给火山引擎的 Seedream 4.5 模型。AI 根据描述画一张漫画风格的图。大概 30 张图并发着跑，3-5 分钟搞定。

Bash

```
```bash
echo "⏳ 开始提交图片生成..."
cat > /tmp/submit_panels.py << 'PYEOF'
import json, subprocess, sys, time

PROJECT_ID = sys.argv[1]
EPISODE_ID = sys.argv[2]

d = json.loads(subprocess.check_output([
    "curl", "-s", "-b", "/tmp/auth_cookies.txt",
    f"http://localhost:13000/api/novel-promotion/{PROJECT_ID}/episodes/{EPISODE_ID}"
]).decode())

panels = []
for sb in d.get("episode", {}).get("storyboards", []):
    for p in sb.get("panels", []):
        if not p.get("imageUrl"):
            panels.append(p["id"])

if not panels:
    print("图片都已存在，不用重复提交")
    sys.exit(0)

print(f"待生成图片数量：{len(panels)}")

for i, pid in enumerate(panels):
    r = json.loads(subprocess.check_output([
        "curl", "-s", "-b", "/tmp/auth_cookies.txt",
        "-X", "POST", f"http://localhost:13000/api/novel-promotion/{PROJECT_ID}/regenerate-panel-image",
        "-H", "Content-Type: application/json",
        "-d", json.dumps({"panelId": pid, "locale": "zh", "count": 1})
    ]).decode())
    print(f"  [{i+1}/{len(panels)}] 已提交")
    time.sleep(0.3)

print("提交完成，等待 AI 出图...")
PYEOF

python3 /tmp/submit_panels.py $PROJECT_ID $EPISODE_ID
```

这段脚本会先扫描剧集里的分镜面板，只挑还没有 `imageUrl` 的面板提交生成请求。如果全部都有图，就直接跳过；否则逐个提交，并打印进度。

## 等待图片出炉
```

然后等它画完：

Bash

```
```bash
echo "⏳ 轮询图片生成结果（每 15 秒一次）..."
for i in $(seq 1 20); do
  sleep 15
  RESULT=$(curl -s -b /tmp/auth_cookies.txt \
    "http://localhost:13000/api/novel-promotion/$PROJECT_ID/episodes/$EPISODE_ID" | \
    python3 -c "
import json,sys
d = json.load(sys.stdin)
panels = [p for sb in d['episode']['storyboards'] for p in sb['panels']]
missing = [p for p in panels if not p.get('imageUrl')]
print(f'{len(panels) - len(missing)}/{len(panels)} 张已好')
if not missing:
    print('ALL_DONE')
")
  if echo "$RESULT" | grep -q "ALL_DONE"; then
    echo "✅ 图片全部生成完成！"
    break
  fi
  echo "  等待中... ($i/20) $RESULT"
  if [ "$i" = "20" ]; then
    echo "⚠️ 轮询超时，可稍后再查或继续等待"
  fi
done
```

最后每 15 秒检查一次剧集详情，统计还有多少分镜面板缺图。全部补齐就结束；如果 20 轮后还没好，可以先等等再查，或者继续轮询。整套流程跑下来，项目、剧集、分镜和图片就串成了一条完整链路。

# 漫画图片到成片：AI全自动流水线实录

这条流水线做的事情很纯粹：把漫画图片配上声音、变成动态视频，最后合成一条完整成片。你要动手的地方很少，大部分环节都交给了脚本和AI。

首先是图片检查环节。脚本会用Python数一遍带 imageUrl 的 panel 数量，然后和总 panel 数比对：一致就通过，不一致就退出重试。默认最多轮询20次，每轮都会打印“图片进度: X/i”，直到全部完成会提示“所有图片生成完成”。

```

有几张没出来？可能被内容审核拦了（比如你故事里有打斗、武器之类的描述）。重新跑上面的 Python 脚本就行，它会自动跳过已经成功的，只重新提交失败的。每次生成有随机性，通常第二次就过了。

现在可以打开浏览器看看效果了。进项目页面，你会看到 AI 画好的漫画图片。

这就是你视频的每一帧画面。到这一步，成就感应该已经来了。

3.2 配置角色配音

[下一步给每个](http://FAL.ai)角色配声音。waoowaoo 内置了FAL.ai的 Index TTS 2 模型——它能根据一段参考音频来"克隆"说话风格。

你给它一段 5 秒的男声录音，它就用这个风格帮你念所有台词。

**第一步：准备参考音频**

先用微软的免费工具edge-tts快速生成两个参考声音（一男一女）：

Bash

```

接着安装 edge-tts，用它来生成角色参考音频。示例里准备了两条声线：男角色用 zh-CN-YunxiNeural，少年感；女角色用 zh-CN-XiaoxiaoNeural，更活泼。两条音频都会保存为独立的 MP3 文件，作为后续配音的音色基准。生成完会有“参考音频生成完成”的提示。

```

然后传到 waoowaoo 的存储里：

Bash

```

音频文件需要传到 MinIO 文件服务（也就是 waoowaoo）。脚本会优先用 docker cp 拷进 waoowaoo-minio 容器，如果容器不存在，就回退到宿主机的 /opt/waoowaoo/data/uploads 目录。上传成功后显示“音频已上传”。

```

想要更真实的声音？录一段你自己的（或者你想要的任何声音），5-10 秒就够了，保存成 MP3 替换上面的文件就行。Index TTS 2 会模仿你的声音来念台词，效果好很多。

第二步：看看你的故事里有哪些角色

Bash

```

然后从本地 13000 端口的接口拉取当前集的 voiceLines，把里面的 speaker 字段去重排序，列出故事里到底有哪些角色，并统计每个角色有多少句台词，输出格式类似“角色名（N句台词）”。

```你会看到类似这样的：
```

Plain Text

```
=== 你的故事里有这些角色 ===
  旁白（4句台词）
  阿金（2句台词）

  小松鼠（1句台词）
```

第三步：给每个角色分配声音

这一步要做的事情很明确：把角色和声线绑定起来。你只需要修改 VOICE_MAP 那几行映射，其他脚本不用碰。

Bash

```
cat &gt; /tmp/setup_voices.py &lt;&lt; &#x27;PYEOF&#x27;
import json, subprocess, sys

PROJECT_ID = sys.argv[1]
EPISODE_ID = sys.argv[2]

# ============================================================
# 👇 在这里修改角色和声音的对应关系
# &quot;角色名&quot;: &quot;voice_male.mp3&quot; 或 &quot;voice_female.mp3&quot;
# ============================================================
VOICE_MAP = {
    &quot;阿金&quot;: &quot;voice_male.mp3&quot;,
    &quot;小松鼠&quot;: &quot;voice_female.mp3&quot;,
    &quot;旁白&quot;: &quot;voice_male.mp3&quot;,
}
# ============================================================

speaker_voices = {}
for name, audio_file in VOICE_MAP.items():
    speaker_voices[name] = {
        &quot;voiceType&quot;: &quot;uploaded&quot;,
        &quot;audioUrl&quot;: f&quot;http://localhost:13000/api/files/{audio_file}&quot;
    }

# 通过 API 更新
data = json.dumps({&quot;speakerVoices&quot;: speaker_voices})
result = subprocess.check_output([
    &quot;curl&quot;, &quot;-s&quot;, &quot;-b&quot;, &quot;/tmp/auth_cookies.txt&quot;,
    &quot;-X&quot;, &quot;PATCH&quot;,
    f&quot;http://localhost:13000/api/novel-promotion/{PROJECT_ID}/episodes/{EPISODE_ID}&quot;,
    &quot;-H&quot;, &quot;Content-Type: application/json&quot;,
    &quot;-d&quot;, data
]).decode()

print(&quot;✅ 角色声音设置完成&quot;)
for name, audio in VOICE_MAP.items():
    print(f&quot;  {name} → {audio}&quot;)
PYEOF

python3 /tmp/setup_voices.py $PROJECT_ID $EPISODE_ID
```

这里有个特别容易踩的坑：VOICE_MAP 里的角色名必须和接口返回的角色名完全一致，差一个字都匹配不上。

第四步：分析配音

Bash

```text
echo &quot;⏳ 正在分析配音...&quot;
curl -s -b /tmp/auth_cookies.txt \
  -X POST &quot;http://localhost:13000/api/novel-promotion/$PROJECT_ID/voice-analyze&quot; \
  -H &quot;Content-Type: application/json&quot; \
  -d &quot;{\&quot;episodeId\&quot;: \&quot;$EPISODE_ID\&quot;, \&quot;locale\&quot;: \&quot;zh\&quot;}&quot; &gt; /dev/null

for i in $(seq 1 12); do
  sleep 5
  echo &quot;  等待中... ($i/12)&quot;
done
echo &quot;✅ 配音分析完成&quot;
```

第五步：生成所有配音

Bash

```
echo &quot;⏳ 开始生成配音...&quot;
RESULT=$(curl -s -b /tmp/auth_cookies.txt \
  -X POST &quot;http://localhost:13000/api/novel-promotion/$PROJECT_ID/voice-generate&quot; \
  -H &quot;Content-Type: application/json&quot; \
  -d &quot;{\&quot;episodeId\&quot;: \&quot;$EPISODE_ID\&quot;, \&quot;locale\&quot;: \&quot;zh\&quot;, \&quot;all\&quot;: true, \&quot;audioModel\&quot;: \&quot;fal::fal-ai/index-tts-2/text-to-speech\&quot;}&quot;)
TOTAL=$(echo $RESULT | python3 -c &quot;import json,sys; print(json.load(sys.stdin).get(&#x27;total&#x27;,0))&quot;)
echo &quot;已提交 $TOTAL 条台词，等待生成...&quot;

# 按台词数量动态计算等待时间（每条约 15 秒）
WAIT=$((TOTAL * 15 + 60))
echo &quot;预计需要 $((WAIT / 60)) 分钟&quot;
for i in $(seq 1 $((WAIT / 10))); do
  sleep 10
  echo &quot;  等待中... ($((i * 10))/${WAIT}秒)&quot;
done
echo &quot;✅ 配音应该已完成&quot;
```

![](img/4cb2ee6a8ff907dcf905dc5de7acb1be.png)

第四阶段：画面变完整视频

图片和配音全部就位之后，就要让静态画面“动”起来了。每张漫画图都会交给AI生成一个4秒的动态片段，最后再全部拼接成完整视频。相当于过去动画工作室里“原画—动画—剪辑”的完整链路，现在全程由AI代劳。

4.1 生成视频片段

这一步是整个流程里最费时间的部分。每张图都会发给火山引擎的 Seedance 模型，让AI判断画面该怎么运动。按30段视频、每段4秒来估算，全部跑完大约需要60分钟。请求提交之后人不用一直盯着，过一阵子回来看结果就行。

Bash

```
echo &quot;⏳ 正在提交视频生成请求...&quot;
RESULT=$(curl -s -b /tmp/auth_cookies.txt \
  -X POST &quot;http://localhost:13000/api/novel-promotion/$PROJECT_ID/generate-video&quot; \
  -H &quot;Content-Type: application/json&quot; \
  -d &quot;{
    \&quot;episodeId\&quot;: \&quot;$EPISODE_ID\&quot;,
    \&quot;locale\&quot;: \&quot;zh\&quot;,
    \&quot;all\&quot;: true,
    \&quot;videoModel\&quot;: \&quot;ark::doubao-seedance-1-5-pro-251215\&quot;,
    \&quot;generationOptions\&quot;: {
      \&quot;generateAudio\&quot;: false,
      \&quot;duration\&quot;: 4,
      \&quot;resolution\&quot;: \&quot;720p\&quot;
}}&quot;)TOTAL=$(echo $RESULT | python3 -c &quot;import json,sys; print(json.load(sys.stdin).get(&#x27;total&#x27;,0))&quot;)
echo &quot;✅ 已提交 $TOTAL 段视频生成请求&quot;
echo &quot;&quot;
echo &quot;⏰ 预计需要 60 分钟，你可以：&quot;
echo &quot;   - 去喝杯咖啡&quot;
echo &quot;   - 想想下一个要做什么故事&quot;
echo &quot;   - 或者就放着，等会儿回来查看&quot;
```

需要注意 generationOptions 里的三个参数：generateAudio、duration、resolution，必须全部写上。少任何一个都会报 VIDEO_CAPABILITY_COMBINATION_UNSUPPORTED。我第一次跑的时候就漏了一个参数，排查了很久才找到原因。

随时查看进度：

Bash

```
curl -s -b /tmp/auth_cookies.txt \
  &quot;http://localhost:13000/api/novel-promotion/$PROJECT_ID/episodes/$EPISODE_ID&quot; | \
  python3 -c &quot;
import json,sys
d = json.load(sys.stdin)
panels = [p for sb in d[&#x27;episode&#x27;][&#x27;storyboards&#x27;] for p in sb[&#x27;panels&#x27;]]
done = sum(1 for p in panels if p.get(&#x27;videoUrl&#x27;))
total = len(panels)
pct = int(done/total*100) if total else 0
print(f&#x27;视频进度: {done}/{total} ({pct}%)&#x27;)
if done &gt;= total * 0.9:
    print(&#x27;✅ 已完成 90% 以上，可以进行下一步了&#x27;)
elif done == total:
    print(&#x27;✅ 全部完成！&#x27;)
else:
    print(f&#x27;还需要等待，预计还剩 {(total-done)*2} 分钟&#x27;)
&quot;```

生成进度到90%以上就可以继续往下走了。没完成的那几段不会影响最终合并，合成时会被自动跳过。

4.2 下载并合并成最终视频

Bash

```

Bash

```

下载脚本会先输出“⏳ 正在下载所有视频片段...”的提示，然后从接口拉取全部分镜数据，找出带 videoUrl 的 panel，存到 /tmp/panels 目录后逐个下载，最后合并输出。下载过程中会记录被跳过的片段数量，少数未完成的部分不会阻断流程，直接滤掉即可。

到这里，整条自动化流水线就走完了。从图片校验、配音准备、角色音色绑定，再到AI生成动态画面并拼接成片，全流程闭环。

视频渲染完成后，想拿到完整的成片，得先把分片内容抓回来再合并。这个过程里，脚本会逐个检查分片文件的大小：超过 1KB 的才被视为有效内容，会被写进合并清单；太小的则说明视频还没渲染完，直接跳过。清单生成后，统一交给 ffmpeg 合并成最终文件。

```text
fname = f"/tmp/panels/{i:03d}.mp4"

subprocess.run(["curl", "-s", "-b", "/tmp/auth_cookies.txt", url, "-o", fname],
               capture_output=True)

size = os.path.getsize(fname) if os.path.exists(fname) else 0

if size > 1000:
    lines.append(f"file '{fname}'")
    print(f"  [{i+1}/{len(panels)}] ✅ 下载完成 ({size//1024}KB)")
else:
    skipped += 1
    print(f"  [{i+1}/{len(panels)}] ⚠️ 跳过（文件太小，可能还没生成完）")

# 写入 ffmpeg 合并列表
with open("/tmp/filelist.txt", "w") as f:
    f.write("\n".join(lines))

print(f"\n共下载 {len(lines)} 段视频" + (f"，跳过 {skipped} 段" if skipped else ""))

PYEOF

python3 /tmp/download_and_merge.py $PROJECT_ID $EPISODE_ID
```

```text
# 合并成一个完整视频
echo &quot;⏳ 正在合并视频...&quot;
ffmpeg -f concat -safe 0 -i /tmp/filelist.txt -c copy /tmp/final_video.mp4 -y 2&gt;/dev/null

FILE_SIZE=$(du -h /tmp/final_video.mp4 | cut -f1)
echo &quot;✅ 视频合并完成！文件大小: $FILE_SIZE&quot;
```

4.3 把视频保存到本地

合并后的视频放在服务器上，怎么拿到自己的电脑里？这里推荐两种方式。

**方法一：通过浏览器直接下载**

先将 `/tmp/final_video.mp4` 放到服务器的上传目录里，或者用 docker cp 直接塞进 MinIO 容器，再在浏览器里打开输出链接即可。

```
Bash

```

```bash
cp /tmp/final_video.mp4 /opt/waoowaoo/data/uploads/ 2>/dev/null || \
  docker cp /tmp/final_video.mp4 waoowaoo-minio:/data/uploads/final_video.mp4
echo "✅ 用浏览器打开以下链接下载视频："
echo "http://你的服务器IP:13000/api/files/final_video.mp4"
```

**方法二：用 SCP 直接拉回本地**

如果不喜欢走浏览器，也可以直接用 scp 命令把文件从服务器拿回来：

```

把"你的服务器 IP"换成实际的 IP。

方式二：scp 直接传到 Mac

在你 Mac 的终端里（不是服务器的）跑：

Bash

```

```bash
scp root@你的服务器IP:/tmp/final_video.mp4 ~/Downloads/
```

如果换了新的 API Key，重新写一下配置就行：

```

视频会下到"下载"文件夹。

![](img/49f9f764eda4af14e83b8a229c3814a1.png)

附录

**附录一：各阶段耗时参考**

| 阶段 | 你动手 | 等 AI | 总计 |
| --- | --- | --- | --- |
| 环境准备（首次） | 20 分钟 | — | 20 分钟 |
| 故事变分镜 | 5 分钟 | 5 分钟 | 10 分钟 |
| 图片生成（约 30 张） | 2 分钟 | 5 分钟 | 7 分钟 |
| 配音生成 | 5 分钟 | 10 分钟 | 15 分钟 |
| 视频生成（约 30 段） | 2 分钟 | 60 分钟 | 62 分钟 |
| 下载合并 | 3 分钟 | — | 3 分钟 |
| 首次总计 | 约 37 分钟 | 约 80 分钟 | 约 117 分钟 |

第二次做会快很多。环境配好了，流程也熟了，动手时间也就 10 分钟。

**附录二：常见报错怎么办**

**UNAUTHORIZED**或**403**

登录凭证过期了。关了终端、等太久都会过期。

解决：重新跑 2.1 的登录命令。

**API Key 相关报错**

Key 没配，或者配错了。

解决：

Bash

```

```bash
curl -s -b /tmp/auth_cookies.txt \
  -X PUT http://localhost:13000/api/user/api-config \
  -H "Content-Type: application/json" \
  -d '{"providers": [{"id": "ark", "name": "火山引擎 Ark", "apiKey": "你的新Key"}]}'
```

如果之前的会话环境还在，直接重新加载保存好的变量；如果文件也丢了，就用 API 查一下项目列表：

```

**No clips found**

你跳过了 2.5 那步。

解决：回去跑 2.5。

Google API 超时或连不上

服务器在国内，Google 访问不了。

解决：把 waoowaoo 部署到海外服务器（推荐），或者给服务器配代理。

**VIDEO_CAPABILITY_COM**BINATION_UNSUPPORTED

视频生成的参数没写全。generateAudio、duration、resolution三个缺一不可。

**图片被内容审核拦了**

故事描述里有敏感内容（武器、暴力之类的）。

解决：重新跑 3.1 的图片生成脚本。它会自动跳过成功的，只重新提交失败的。每次生成有随机性，通常第二次就过了。

**终端断开，变量全丢了**

解决：

Bash

```

```bash
source /tmp/waoowaoo_session.env
echo "PROJECT_ID=$PROJECT_ID"
echo "EPISODE_ID=$EPISODE_ID"

curl -s -b /tmp/auth_cookies.txt http://localhost:13000/api/projects | \
  python3 -c "import json,sys; [print(p['projectId'], p['name']) for p in json.load(sys.stdin)['projects']]"
```

需要补传音频素材时，也可以直接把文件丢进 MinIO：

```

**附录三：怎么让配音更像真人？**

教程里用的edge-tts是微软的免费合成语音。质量还行，但你一听就知道是机器人。

升级方法很简单：

1.  用手机录一段 5-10 秒的音频，说一句完整的话（比如"今天天气真不错，我们一起去散步吧"）

1.  保存成 MP3，传到服务器/tmp/目录

1.  上传到 waoowaoo 存储：

Bash

```

```bash
docker cp /tmp/你的音频.mp3 waoowaoo-minio:/data/uploads/
```

```

1.  在 3.2 第三步的VOICE_MAP里，把角色的音频文件名改成你上传的

Index TTS 2 会模仿你给的声音来念台词。5 秒的参考音频就够了，效果比默认的强太多。

附录四：waoowaoo 还能接哪些 AI？

教程里只用了三个服务商。其实 waoowaoo 支持的远不止这些：

| 服务商 | 能力 | 说明 |
| --- | --- | --- |
| 火山引擎 Ark | 图片 + 视频 + 文本 | Seedream 画图，Seedance 做视频，豆包做分析 |
| Google | 文本 + 图片 + 视频 | Gemini 做分析，Imagen 画图，Veo 做视频 |
| FAL.ai | 图片 + 视频 + 配音 | Index TTS 配音，Kling 做视频 |
| 阿里百炼 | 文本 + 视频 + 配音 | Wan 视频，QwenTTS 配音 |
| 硅基流动 | 全能 | 文本、图片、视频、音频都支持 |
| MiniMax | 视频 | 海螺视频 |
| Vidu | 视频 | 生数科技 |

在"设置中心"里可以配多个服务商，生成的时候选不同的模型。比如用 Imagen 画图风格不一样，用 QwenTTS 配音又是另一种味道。

**附录五：第二条视频怎么做？**

环境都配好了，做第二条只需要：

1.  登录（凭证过期的话）

1.  创建新项目（2.2）

1.  写入新故事（2.3）

1.  按顺序跑 2.4 → 2.5 → 2.6 → 3.1 → 3.2 → 4.1 → 4.2

熟练之后，你动手时间也就 10 分钟。等 AI 的时候可以同时开两个项目，让它并行跑。

## 六、Claude Skills 的拓展玩法

### 01.打造 AI 应用开发 Skills

**一定程度辅助到 AI 设计者：AI 编程，用 skills 接模型，UI 设计的规范，代码审**核；部署也可以接 API，对出海比较方便，做成 skills 一键上站，做成网页

终于到了重头戏环节了，本章节，我将带大家从 0 开始，直接完整地跑出一个上站 demo 的全流程，实测完整跑出一个能用的 demo 并上站大概是 5 个小时左右，当然这个和应用难度本身也有关系，不过以下面我要讲的这个案例来看，效率是非常高的。

这次案例以我的新站[larkbase.club](http://larkbase.club)为例，来给大家演示一下怎么把这个网站给做出来。

我现在的工作流程分成三步：

步骤一：需求澄清，一个项目的第一个文件夹会放这个部分的东西，这个文件夹命名为 requirements；

步骤二：将澄清的需求做成原型设计和数据流程，项目的第二个文件夹放这部分内容，命名为 design；

步骤三：将前后端分别写出来，然后完成上站的动作，文件夹命名为 develop。

第三步完成后如果效果还不错，我就会把它套上模板拿去上站销售，已有的页面套模板也很有讲究，这个有机会再另说。

每一个步骤我都单独在项目文件夹下面起一个文件夹，它们就不会相互串门了。这样也有一个好处，产品迭代的完整周期都通过 requirements - design - develop 的方式迭代进来，清晰可见。

[让我们开始，首先我建了一个](http://larkbase.club)文件夹，叫larkbase.club。

步骤一：从想法到 PRD（brainstorming + doc-coauthoring）

在写代码之前，我们需要先明确要做什么。这一步，我们将借助 AI 进行头脑风暴，并输出一份完整的产品需求文档（PRD）。

首先打开终端：

如果你是 Windows 用户：

在刚才建好的[larkbase.club](http://larkbase.club)文件夹空白处，按住键盘上的Shift键并点击鼠标右键，选择‘在此处打开 PowerShell 窗口’（或‘在终端中打开’）。

**如果你是 Mac 用户：**

打开‘启动台’搜索‘终端’，打开后，输入cd（注[意 cd 后面有个空格），](http://larkbase.club)然后把你建好的larkbase.club文件夹拖拽到终端窗口里，按下回车键。”

![](img/3226cfda5b3dca8bcc5955fe93fd2dcb.png)

在打开的终端中，复制并粘贴以下命令，然后按下回车键，这一步会自动帮你创建一个名为requirements的需求文件夹，新建完成后，再通过cd requirements进入该文件夹。

```

Plain Text

```text
mkdir requirements
cd requirements
```

![](img/49fdf4181ccae02217aea97875ff8dc8.png)

接下来要装两个 Skills，一个叫 `brainstorming`，负责带我们开脑洞、扩展思路；另一个叫 `doc-coauthoring`，负责陪我们一起写文档、改文档。

**⚠️ 注意：**

动手之前，先确保电脑上已经装好了 Node.js（如果还没装，回到附录或前置准备教程看一眼）。确认无误后，在终端里逐行粘贴下面的命令，每粘一行按一次回车执行：

Plain Text

```
npx skills add obra/superpowers
npx skills add anthropics/skills
```

安装 Skills 的操作和 1.2 节完全一致，都是通过 `npx skills add` 来装。先把 brainstorming 装上：

![](img/bd4c8599e05524a3c07973e4e5aa0032.png)

再把 doc-coauthoring 装上：

![](img/33587c9bdee460e920a290962a1ebaa6.png)

看到终端里出现绿色 `Done!`，就说明全部安装完成了。

![](img/648ab45b1b3b13d3811085fa2e7fbad6.png)

接着，在终端的光标处输入 `gemini`，回车启动 gemini-cli。

![](img/1c959684d3bce81d3f0aac8ff6f5687d.png)

启动成功后，会看到一个巨大的 GEMINI 字母图案。

![](img/cc32d778d0137080f94831306cdc84b4.png)

在输入框里键入 `/skills list`，回车查看。

![](img/f575c2869798e2cb170c0c76e7b70d09.png)

如果列表里同时出现了 `brainstorming` 和 `doc-coauthoring`，恭喜，准备工作全部就绪！

![](img/a9bf0495d09f015c9caef24a862c1faa.png)

完整截图如下：

![](img/4715ce0923d0c8b3a45254b501c56844.png)

呜呼！它开始调用技能了！来吧，放开手脚，痛快地头脑风暴一波！

![](img/7cf0a55040378c6675bdd152fda6362c.png)

第一步：把项目背景提示词投喂进去

把下面这段提示词直接发给它，然后回车。

Plain Text

```
我正在做一个关于飞书多维表格行家俱乐部的club网站，这个网站用于邀请专家进入行家俱乐部，挂行家的模板，博客，名人墙，还提供b端宣传，让大家可以在club网站找到想对接的maker帮自己交付应用。请和我一起头脑风暴一下，这个网站的mvp版本做什么比较合适
```

![](img/4ae5623c12c09f7c2f7dd197e62ff40e.png)

第二步：给 brainstorming 和 doc-coauthoring 放行

在运行过程中，gemini-cli 会弹出一个安全确认窗口，我们直接选择 `Allow for this session`，这样整个项目流程里，这两个 skill 都能随意使用。

![](img/bf4f9c044a794fa7308478e04666d5da.png)

之后它会连环提问，我们用大白话正常回答就行，就跟平时操作 coding cli 的感觉一样。几轮聊下来，它就会给出一版简单的初稿。

![](img/2a24d1e7c0ac4921507e4616e75d13a4.png)

拿到初稿后，我们继续让 doc-coauthoring 上场精修。

（小提示：如果 AGENTS.md 里提前约定了工作流，它一般不会直接输出 MVP 计划，而是会转去调用 doc-coauthoring 继续优化；这次我们没加约束，所以 brainstorm 自己就闭环了。）

![](img/695113141ba5fb81bad4c50a1c8ae49b.png)

然后继续让 doc-coauthoring 陪着我们一问一答地改进。

![](img/8dfd2da3d550735db2e08af0143db3c3.png)

继续推进。

![](img/9647680513ace6791968d4cc1e4b87c7.png)

让它把 Project overview 展示出来看看。

![](img/c2af4c50454a361cda663b9b00de611b.png)

不错，再看看第二章节。

![](img/327263be4d3610cdbb2791a63a0cf0fa.png)

嗯！这个味儿对了！继续看第三章节。

![](img/9200b2993b118074d3516a1c7e929833.png)

没问题，继续！

![](img/0673ba04e0168939b1995ce8764ba38a.png)

再往后。

![](img/beeaadddfdb3ea2b0e687fa54b8d0db4.png)

漂亮！

![](img/3036fe32efa65d890ef18c90c2bcab35.png)

好，已经到最后一个环节了。

![](img/b28adf48d2c4225945ea37eedb4983df.png)

到这里，第一步就算圆满收尾。把我们精心沉淀出来的约 7KB 的 requirements 复制好，后面第二步会用到。在接下来的步骤二里，AI 会拿着这份“设计图纸”，直接帮我们生成前端代码原型。

![](img/c2370bef05706598338c304293611e30.png)

**步骤二：三样工具，落地页面原型**

这一节继续推进：先认识三样工具。

**stitch**：Google 提供的前端代码生成服务，擅长把想法迅速做成视觉完整的页面；地址：https://stitch.withgoogle.com/

**web-design-guidelines**：一套网页设计准则，让 AI 明白视觉审美和版面秩序该遵循什么标准。

**doc-coauthoring**：协作型文档 Skill，用来读取、消化上一节产出的 PRD。

准备完毕，开始动手。

**第一步：准备 design 目录**

回到项目最外层，开一个名为 design 的目录。把上一节得到的 mvp-requirements.md 拷贝进去。

![](img/362afee6ea7873596885d05430de92eb.png)

用 VS Code 打开这个目录。

![](img/50213d878f07b67ff30fe395a6d4b00b.png)

确认该文件就在其中。

![](img/61c13e1443618b202e68240003d951c5.png)

**第二步：装好两个 Skill**

文件就位后，把两个 Skill 装上：先处理 web-design-guidelines，再处理 doc-coauthoring，流程同上一节。

Plain Text

```
npx skills add https://github.com/vercel-labs/agent-skills --skill web-design-guidelines
npx skills add https://github.com/anthropics/skills --skill doc-coauthoring
```

全程基本按回车确认即可。

![](img/531defe1478a05f6f063c2e15d24cc67.png)

![](img/d82b576e5c1c1a1972078faa7463f64c.png)

在终端敲 claude 并回车，进入 Claude Code。会话里执行 /skills 并回车，确认两个 Skill 在线。出现下图状态，说明已就绪。

![](img/5503b73ffffd5d7a8db10a0cabe672ee.png)

**第三步：逐页敲定原型**

下面进入原型环节。记得用 @ 把先前那份 requirements 带入会话。

Plain Text

```
根据 @larkbase-club-mvp-requirements.md 帮我整理一下，我们总共有多少个页面，需要怎么设计。
```

发送后，Claude 会给出回应。

![](img/82aa6b5d54ca410cbc3bbd6746ba9646.png)

随后逐屏推进。可以让 Claude 先用字符画（ASCII）画出页面草图。例如：

Plain Text

```
请根据你的理解使用ASCII码生成原型的布局，我们来进行讨论。
```

首屏效果挺顺眼。

![](img/f11990086351d51add2c972a3666abf4.png)

哪里不顺眼就直接提。草图阶段 token 消耗很少，可以反复打磨；按钮摆哪、文案怎么写、控件尺寸与排布，都能在这轮敲定。

几轮下来，三页的定稿字符画都齐了。

![](img/91a8f452c2c80195682e75aa72052301.png)

![](img/6b8c08eef03e53e59bac608fc5b0919a.png)

![](img/a7606277c42a140eb27041c9c5ac1c69.png)

再让 Claude 把全部字符画与配套说明汇总成 Markdown 文件。我的导出结果如下：

Markdown

```

# Lark Base Club - Homepage (Page 1) 原型设计 ## ASCII 原型图 ```
```text
╔══════════════════════════════════════════════════════════════════════════════╗
║ 🔍 Lark Base Club [Square] [Join] [🌙 Light/Dark] 📱 Mobile             ║
╠══════════════════════════════════════════════════════════════════════════════╣
║                                                                              ║
║ ┌─────────────────────────────────────┐                                     ║
║ │                                     │                                     ║
║ │ HERO SECTION                        │                                     ║
║ │                                     │                                     ║
║ │ ┌─────────────────────────┐         │                                     ║
║ │ │                         │         │                                     ║
║ │ │ &quot;连接飞书多维表格专家 │         │                                     ║
║ │ │ 与企业需求的平台&quot;      │         │                                     ║
║ │ │                         │         │                                     ║
║ │ └─────────────────────────┘         │                                     ║
║ │                                     │                                     ║
║ │ &quot;找专家？展示作品？获取客户？    ║
║ │ 这里是飞书多维表格极客的家园&quot;    │                                     ║
║ │                                     │                                     ║
║ │ [ 🚀 浏览行家广场 ]                 │                                     ║
║ │                                     │                                     ║
║ └─────────────────────────────────────┘                                     ║
║                                                                              ║
╠══════════════════════════════════════════════════════════════════════════════╣
║                                                                              ║
║ ┌────────────────────────────────────────────────────────────────────┐     ║
║ │                                                                    │     ║
║ │ INTRODUCTION - &quot;什么是 Lark Base Club?&quot;                       │     ║
║ │                                                                    │     ║
║ │ ┌─────────────────────┐    ┌─────────────────────┐                │     ║
║ │ │                     │    │                     │                │     ║
║ │ │ 👔 B端老板          │    │ 🛠️ Maker 专家       │                │     ║
║ │ │                     │    │                     │                │     ║
║ │ │ &quot;需要SRM/HR系统？  │    │ &quot;擅长飞书多维表格？│                │     ║
║ │ │ 不想从零开发？&quot;    │    │ 想展示你的技能？&quot;  │                │     ║
║ │ │                     │    │                     │                │     ║
║ │ │ ✓ 浏览专家          │    │ ✓ 展示作品集        │                │     ║
║ │ │ ✓ 找到现成模板      │    │ ✓ 获取客户线索      │                │     ║
║ │ │ ✓ 一键预约咨询      │    │ ✓ 加入极客社区      │                │     ║
║ │ │                     │    │                     │                │     ║
║ │ └─────────────────────┘    └─────────────────────┘                │     ║
║ │                                                                    │     ║
║ └────────────────────────────────────────────────────────────────────┘     ║
║                                                                              ║
╠══════════════════════════════════════════════════════════════════════════════╣
║                                                                              ║
║ ┌────────────────────────────────────────────────────────────────────┐     ║
║ │                                                                    │     ║
║ │ FEATURED EXPERTS - 精选行家                                        │     ║
║ │                                                                    │     ║
║ │ ┌─────────┐  ┌─────────┐  ┌─────────┐  ┌─────────┐              │     ║
║ │ │ [IMG]   │  │ [IMG]   │  │ [IMG]   │  │ [IMG]   │              │     ║
║ │ │         │  │         │  │         │  │         │              │     ║
║ │ │ 张三    │  │ 李四    │  │ 王五    │  │ 赵六    │              │     ║
║ │ │ 顾问    │  │ 开发    │  │ 架构师  │  │ 产品经理│              │     ║
║ │ │         │  │         │  │         │  │         │              │     ║
║ │ │ #CRM    │  │ #HR系统 │  │ #SRM    │  │ #财务   │              │     ║
║ │ │ #零售   │  │ #制造   │  │ #供应链 │  │ #发票   │              │     ║
║ │ │         │  │         │  │         │  │         │              │     ║
║ │ │ [→]     │  │ [→]     │  │ [→]     │  │ [→]     │              │     ║
║ │ └─────────┘  └─────────┘  └─────────┘  └─────────┘              │     ║
║ │                                                                    │     ║
║ │ ┌─────────┐  ┌─────────┐                                        │     ║
║ │ │ [IMG]   │  │ [IMG]   │                                        │     ║
║ │ │         │  │         │                                        │     ║
║ │ │ 钱七    │  │ 孙八    │                                        │     ║
║ │ │ ...     │  │ ...     │                                        │     ║
║ │ │         │  │         │                                        │     ║
║ │ │ #...    │  │ #...    │                                        │     ║
║ │ │         │  │         │                                        │     ║
║ │ │ [→]     │  │ [→]     │                                        │     ║
║ │ └─────────┘  └─────────┘                                        │     ║
║ │                                                                    │     ║
║ │ [ 查看所有行家 → ]                                                 │     ║
║ │                                                                    │     ║
║ └────────────────────────────────────────────────────────────────────┘     ║
║                                                                              ║
╠══════════════════════════════════════════════════════════════════════════════╣
║                                                                              ║
║ © 2025 Lark Base Club | Powered by Feishu                                 ║
║                                                                              ║
╚══════════════════════════════════════════════════════════════════════════════╝
```
``` --- ## 布局说明 ### 1. **Header (全局导航)** - **位置**: 固定在顶部 - **左侧**: Logo + 站点名称 - **中间**: 导航链接 (Square广场, Join加入) - **右侧**: 主题切换器 (🌙/☀️) - **响应式**: 移动端折叠为汉堡菜单 --- ### 2. **Hero Section** - **对齐**: 居中对齐 - **内容**: - 大标题: &quot;连接飞书多维表格专家与企业需求的平台&quot; - 副标题: &quot;找专家？展示作品？获取客户？这里是飞书多维表格极客的家园&quot; - CTA 按钮: &quot;🚀 浏览行家广场&quot; (跳转到 `/square` 页面) - **样式**: 大字号、粗体、飞书蓝色强调 --- ### 3. **Introduction (双栏布局)** - **布局**: 左右两栏，分别面向两类用户 - **左栏 - B端老板**: - 标题: &quot;👔 B端老板&quot; - 痛点问题: &quot;需要SRM/HR系统？不想从零开发？&quot; - 核心利益点: - ✓ 浏览专家 - ✓ 找到现成模板 - ✓ 一键预约咨询 - **右栏 - Maker专家**: - 标题: &quot;🛠️ Maker 专家&quot; - 痛点问题: &quot;擅长飞书多维表格？想展示你的技能？&quot; - 核心利益点: - ✓ 展示作品集 - ✓ 获取客户线索 - ✓ 加入极客社区 --- ### 4. **Featured Experts (网格布局)** - **数据来源**: 从 Lark Base 获取 `is_featured=true` 的行家数据 - **展示数量**: 4-6 位精选行家 - **响应式网格**: - 桌面端 (≥1024px): 4 列 - 平板端 (768px-1023px): 2 列 - 移动端 (&lt;768px): 1 列 - **卡片内容**: - 头像 (圆形/圆角方形) - 姓名 - 职位/头衔 - 标签 (2-3个，徽章样式) - 查看详情按钮 (→) - **底部**: &quot;查看所有行家 →&quot; 按钮，跳转到 `/square` 页面 --- ### 5. **Footer** - **内容**: - 版权信息: &quot;© 2025 Lark Base Club&quot; - 技术支持: &quot;Powered by Feishu&quot; - **样式**: 简洁、居中对齐、灰色文字 --- ## 技术实现要点 ### 响应式断点 - **Mobile**: &lt; 768px - **Tablet**: 768px - 1023px - **Desktop**: ≥ 1024px ### 数据获取 - **Server Component**: 使用 Next.js App Router - **数据源**: Lark Base Bitable API - **缓存策略**: ISR, `revalidate: 60` 秒 ### SEO 优化 - **Meta Title**: &quot;Lark Base Club - 连接飞书多维表格专家与企业需求&quot; - **Meta Description**: &quot;找专家？展示作品？获取客户？这里是飞书多维表格极客的家园&quot; - **Keywords**: 多维表格, 飞书Base, 行家, 极客社区

```

**第四步：交给 stitch 出视觉稿**

打开并登录 stitch。把刚才那页字符画整体贴进去，发送。

![](img/e386288da299cdce3dcf5ae8728af1f5.png)

接着在 stitch 中继续补充要求，等一会儿就能拿到稿子。

![](img/7bd6e8a6138c31cc481f4875be3fd51c.png)

效果大致如下。

![](img/d00ea00a5c7ecdc65b4a20c7da3f5315.png)

![](img/03ac0b82ce9c9b6d9eb1a2e645a0d343.png)

![](img/90e6cd968326570ad512f296628341c3.png)

满意就保存。

**第六步：保存设计文件**

在页面左上方点 Download project 按钮，浏览器会收到 zip 包；包内是各页面 HTML 与配图。解压后放进 design 目录。

![](img/8b1d6edbee8e0cf22380f8560d035e51.png)

**第七步：用 doc-coauthoring 收尾 PRD**

视觉稿完成后，PRD 也可以收尾。依旧用 gemini-cli 生成内容，发送下面这段提示词：

```
来看一下 stitch_larkbase_club_homepage文件夹里的设计稿，以及 @larkbase-club-mvp-requirements.md ，整理一下交互，用 doc-coauthoring 和我一起把 prd 写出来
```

想快速把 Next.js 项目骨架搭起来，同时把前端设计、SEO 审计和组件库这些能力一次配齐？按下面几步走就行。先在当前目录生成一个最新的 Next.js 应用，省去交互确认：

```

![](img/22cad52f3862735fc8e8ea2f519dc52e.png)

开始。

![](img/71a454394189b9f43b56e911884d2761.png)

一顿对话之后……我们的 PRD 就做好了。

![](img/f8d962955c49d6af12e4431e021ce066.png)

打开看看，good！good! 这就是我们想要的 PRD！用户故事、页面设计、功能交互、数据及后段逻辑都在里面！

![](img/55d3db875215e67c1fe089d10b223a9a.png)

![](img/d86db2bfc3be654059536abd9a2a4c66.png)

爽！我已经开始期待把站点弄出来了。

![](img/89a87c4fe740775079ea2ae51b2f8a34.png)

步骤三：从原型到站点（react-best-practices + web-design-headlines+frontend-design+shadcn-ui+seo-audit+ralph-wiggum+context7+chrome devtool mcp）

本部分使用的内容相当多，这里简单介绍一下。

React-best-practices：前端用 react 框架的，全部都可以装上这个。

Web-design-guidelines：网页设计专用，在步骤二里也用到了，这里也要装上。

frontend-design：极力推荐，前端设计必装。

shadcn-ui：如果你的网站用 nextjs，那么这个 skills 必装，这个 skills 可以规范化使用 shadcn/ui 的组件。

seo-audit：SEO 审查，适当地注入一些关键字以提升搜索结果。

然后是 plugin，这里也推荐三个。

Ralph-wiggum：这个是代码循环审查的插件，可以让代码质量上一个台阶，必装；

context7：老 mcp 工具了，获取最新 code 实践，必装；

chrome devtool mcp：我们做的是网站，它到时候自己测试要用，装。

第一步：使用 nextjs 脚手架起一个 nextjs 项目

在stitch 干活的同时也不要闲着，直接开一个 vscode 把 nextjs 环境给起了。

Tips：值得注意的是，如果我们是写代码的话，除了第一次初始化环境和内容第一次布生产环境直接 git push 到 master 分支以外，之后我们都要 checkout 一个 dev 分支出来，通过 pull request 的方式更新 master 分支，以确保开发环境的代码不会影响到生产环境。这一块可以通过系统性学习 git 相关知识补齐，本部分仅作说明。

首先在项目文件夹下面新建一个 develop 文件夹。

![](img/0e60d6314aa0170489592229506f9c09.png)

打开当前正在使用的 IDE（antigravity、cursor、vscode 均可），进入 develop 文件夹。在 develop 文件夹下用 pnpm 起一个项目。

在 develop 文件夹下打开 IDE，然后在 IDE 下打开终端，输入如下指令，回车。

Bash

```

pnpm create next-app@latest . --yes

接着把几组对开发很有帮助的 skill 装进项目：Vercel 官方的 React 最佳实践与网页设计规范、Anthropic 的前端设计技能、shadcn-ui 相关能力，以及一份 SEO 审计工具。命令如下：

```

过了一会之后，nextjs 脚手架就起好了。

![](img/f62e1452e69a078ee4eee9cf9c73e1a0.png)

接下来就是安装 skills 和 plugin。

先安装刚刚介绍的四个 skills。

Bash

```

npx skills add https://github.com/vercel-labs/agent-skills --skill vercel-react-best-practices

npx skills add https://github.com/vercel-labs/agent-skills --skill web-design-guidelines

npx skills add https://github.com/anthropics/skills --skill frontend-design

npx skills add https://github.com/giuseppe-trisciuoglio/developer-kit --skill shadcn-ui

npx skills add https://github.com/coreyhaines31/marketingskills --skill seo-audit

最后初始化 shadcn 组件体系，后续就能直接往项目里加组件了：

```

几个一下装，相互不耽误。

![](img/2934e8f0f5d2ca8539409ac29652583d.png)

装好了。

![](img/42f22667980275145bf1a5ecc7af0a64.png)

再来装 plugin。

plugin 的安装是 claudecode 独有的，codex 和 gemini-cli 都没有。当然我还知道一个人可以用，那就是 codebuddy，最近 claude 刚被封号，为了演示我们就改用 codebuddy 吧。有 claudecode 的同学可以继续使用 claudecode。

先打开 codebuddy，输入 /plugin 回车。

![](img/a7a13b6917fee798a7e567b7e7a976c2.png)

先装个 chrome devtool，空格选择。

![](img/fcb9518a1ddc7cf19aa139b2a2f9549f.png)

选完了，一个回车下去。然后选第二个装到仓库下面。

![](img/a16ee298bec679365bc0948fa94159be.png)

再装 ralph-wiggum，空格选择，回车。

![](img/f2a1b9453afcebae76c17325743035c3.png)

再装 context7，空格选择，回车。

![](img/ad9220aa2cca329fb2292d36b08054a9.png)

装完之后，tab 选择看看是不是都装了。好了，都装好了。

![](img/35da3d4e61500341e1057ea216cd0225.png)

然后我们就可以直接开始把页面里面的组建都先定好，让 AI 先画出来，然后再组装到 page 里。

首先/init，所有项目开始做之前都要进行初始化，这是必须做的，不要拉下。

![](img/aba96055c8a3380c3c7927d5f72429d7.png)

![](img/8886a9379535e1ebdd3611fde3d1a68d.png)

然后，[CODEBUDDY.md](http://CODEBUDDY.md)文[件就被创建在 de](http://CLAUDE.md)velop 的根目录下面了。如果你用的是 claudecode，那么创建的初始提示词就是CLAUDE.md。

![](img/b4612aea2f01c7c0904e19ff152c55d5.png)

[完事之后再把 skill](http://CODEBUDDY.md) 的指引信息写到CODEBUDDY.md文件里。

tips：通过在初始提示词内增加 skill using 的说明，可以有效规范模型使用 skill 的方式和步骤，一般来说我们都通过这个简易方式来规范模型的工作流程。

![](img/9f1d826befe4f2a6c9b62796ffd60702.png)

先把页面画了，我们把 stitch 的下载包复制过来。建一个 UI 文件夹。

![](img/0f21f41b0568392231ef2d1c8fdbe24b.png)

然后把 nextjs 的项目初始化搞完，之前搞好了脚手架，现在来装 shadcnUI，把暗黑模式也搞了。

先来把 shadcn 给安装一下。

Plain Text

```

pnpm dlx shadcn@latest init

这样一套下来，项目基础、设计规范、组件库和 SEO 检查都到位了。

```

![](img/54efdcd0e3891bd5bad71e1c57a604b3.png)

shadcn/ui 装好了，继续来做 darkmode。到 shadcn/ui 的 dark mode 界面，点击 copy page。

![](img/191aa6a10cf6691d439fbb461421e8ca.png)

然后告诉 claudecode 或者 codex，帮我安装一下 dark mode，这是材料，然后粘贴进去你复制的内容。

![](img/4ff546e62490a919e320ba7de3df4bcb.png)

过一会儿装好了。

![](img/77d16f16bbdd7b582d517e2f14aecac5.png)

现在就可以开始画页面了。

![](img/5e819ed6d00df18ad7ea0ec9d2174891.png)

对了，这个地方可以开 plan mode。plan 完了长这样。

![](img/b866cada0500b76c470602449bd5fed7.png)

至此前端就开始干活了。

过了一会干好了。

![](img/791f68aed1b766c1ed63f41d607d2173.png)

![](img/b9069f2d72ac0da0d9cbe16186fb305d.png)

![](img/916859e35ebcec1ccb6e01483546d65a.png)

里面还有很多问题，我们先不管，先把后端做了，到时候还要接数据还有存储桶，里面的问题到时候都能解决。

现在，来收拾后端的烂摊子。

可以看到，前端的精选行家里面的数据都是假的，然后数据本身也是假的。

核心的逻辑是让多维表格起一个工作流，当它更新了数据之后把数据推给我们的中间件，然后中间件将内容清洗之后推送给我们的后端数据库，然后前端再去读。

具体我们可以先和 AI 讨论出一个时序图，大概是下面这样：

具体的开发逻辑就是：

1.  先新建一个多维表格；

1.  然后做一个数据库，让 AI 跑数据库初始化把数据库的表建好；

1.  基于数据库的表结构，给多维表格的字段进行修改；

1.  建一个飞书应用，关联上多维表格，赋予相关的应用读取权限；

1.  给网站连上 cloudflare R2 存储桶，用于后续飞书应用将鉴权的头像还有模板缩略图放到指定域名下在公网可暴露；

1.  写好 webhook 接收完整的飞书应用推送的数据，更新数据库信息，包括专家信息和专家作品信息；

1.  将前端 mock 的数据接上数据库，这一步也可以提前做，问题不大。

接下来我们就一步一步做吧，这一块就和 skills 没啥关系了，全是配置，就硬配，然后调 API。

我们先把飞书多维表格做好。

起一个飞书多维表格，把表格建好，剩下的先不动。

![](img/64aa68438598290f87c30d0284fb1103.png)

然后让 AI 把后端写好。后端我习惯使用 codex。

我们的后端还是相对简单的。直接口喷让 AI 加功能。

![](img/bca7d7302f436011f3af4480af930cfe.png)

然后就写好了。

![](img/15c0ef9aa9ff5c4aca723a5b74cd7bd2.png)

接着我们来配 neon 的数据库，登录。

![](img/1322a850f885201a924bf49f0331de1c.png)

建一个新的项目，connect。

![](img/a561a2d8132d9ea923e9e9a1854526d1.png)

跟着 neon 的导航走，把 DATABASE_URL 放到环境变量里，然后连接。

可以考虑安装 neon 的插件，看一下是否 connect。

![](img/bed9955f9ff2d6642fc11d0d8a02774e.png)

接着我们把前端 mock 的假数据改成接数据库。

![](img/8843106f76f99d357ee5db40b5bdd78a.png)

改好了，跑一下 pnpm lint，修一下明显的 bug。

![](img/637252e539977b223224488fef50653c.png)

最后到页面上看一下是不是已经没数据了（因为数据库现在还没有数据），没有了就表示 OK 了。

![](img/8a15c0b73eb167fcb3dd0050b0ee3921.png)

然后我们来造一条数据通过跑 sql 的方式把东西放进去。

先到 neon 里看一下数据库表结构。

![](img/7ffff40b01e167181bc7616dd4efea79.png)

如果你安装了 neon 的插件，它会自动装上 mcp 工具，你就可以像我一样直接问 AI。

![](img/4fc30947860e6ca721749654e8a5de02.png)

然后我们按照这个信息原封不动地在多维表格里配一遍。

![](img/421d759e9bbefb23aa87c19e911af926.png)

![](img/c4f8dd7a5b69d26c7403a2708f4f4c6e.png)

一条数据配好了。

先注册一下存储桶。

![](img/87d6a9a89d86d14ec11692ff9f695bc7.png)

注册好了之后使用 S3 API 完成处理，把 AccountID、Access_key_id secret_access_key 都写到环境变量里。

![](img/63994cfd31c2b82ffc28e6c53fb5bc71.png)

最后放一个 url 用来接收请求，cloudflare 会自己加好 DNS 的。

![](img/8976c2263f88f24cce2d2003eb6c1e5e.png)

然后，让 AI 带我们去吧 R2 存储桶要用到的环境变量配进去。

![](img/823f46ad77a455aa44160f369fdb61eb.png)

一顿操作之后配好了。

![](img/e0073279dcb182495ea9742f352d5b38.png)

至此，我们就可以实现从飞书多维表格的附件图片拉取图片到存储桶里了。

那么，怎么把多维表格和我们的数据库还有存储桶连到一起呢？按照之前的说法，我们只需要做一个自建应用，让这个应用可以读表格数据，下载附件就可以了。

让我们在飞书开放平台创建一个企业自建应用。

![](img/81c2d457c9f2bb7538578e0cc3f85779.png)

建好了之后给它配上对应的权限，主要是多维表格读取的权限还有媒体下载的权限。

![](img/9ce0372a25705a00805ed74aa4deeb95.png)

接着，把应用凭证的 App ID 和 Secret 配置到环境变量里。

![](img/50dfdccf46d58730f08a22b4dea9a1fc.png)

然后直接开喷，让 AI 给我把数据连上。

![](img/bf6d14c38ae3cc28877a763a64a9641c.png)

然后一顿改，改完了，很快就改完了。

好，全部开发完了，跑一遍 vercel-react-best-practices skill。

![](img/6dc991f07202c03e88ba52d8b45f0d30.png)

然后收获了成吨的问题，让它自己改。

![](img/2ce2cdeb9a3106b4f1cfe94d99c19bd2.png)

全部改完了之后，再跑一遍 seo-audit skill。

![](img/a2ba6a85824193a5f70ab49c1106ca18.png)

再让它改一遍。

改好之后就可以打包扔到 vercel 上面去了。

在终端根目录启动 vercel cli。

![](img/608e62159df9dd517b973f4663291751.png)

回车。然后系统就会跳转到一个浏览器，直接 verify 就可以了。

![](img/044edc6cfed5a28434c8a74fbb7574b8.png)

一顿操作。记得把根目录选对，比如我的根目录是 。/develop

![](img/a9230ca0a20bd1a0b9d41a7d468f937e.png)

然后继续进行部署流程，根据提示完成操作，叫我们改的地方通通不改，全部默认。看到这里它就开始部署了。

![](img/3ec664841a691095793ece52c708c8fa.png)

过一会儿就看到了这个。

![](img/d649408eaf5f4e6be8fcf724f9bf21b5.png)

部署就成功了。

跳过去看看。完美！

![](img/b831a6585752b40091c0d0d5891f7578.png)

最后再去 vercel 官网检查一下。

![](img/10df60e12ba930ab774b354027bd7263.png)

换一下域名，直接输进去，到时候会报错，报错的时候选 configure automatically。它会自动帮我们指向 DNS 解析服务商的。

![](img/7640c8beb01285c136a96bd3ab6eff19.png)

就像这样。

![](img/6535e03805dd82da4f3e8d3e24a878e7.png)

但是你不要真信 vercel 这个大头鬼，那个糟老头子坏得很。回到 cloudflare，把proxy status 改回来。

回到 cloudflare 的 DNS records 位置。把 A 和 CNAME 的 proxy status 改回 Proxied。

![](img/de6600f321d3f76c5e69b06b87ab0bc9.png)

至此，整个网站从 0 到 1 的搭建全部结束。

累个半死，建议大家还是去用模板，这个网站搭出来至少花了 8 个小时，用模板估计 3 个小时就够了。

Skills 进阶路径 & 应用开发 Skills 汇总

• 一页图：7 阶段成长路径

![](img/dda98ac4120c730f0dd04a84c94cde89.png)

如果你想更好地

1.  通过官方文档学习 skills 基础概念

1.  试用官方仓库 skill 解决基本问题

1.  海量找 skills 应用到自己的项目（awesome-skills、skillsmp、x 社媒、微信公众号……）

1.  尝试理解完整的 skills 工作原理

1.  自主构建 skills

1.  结合 skills 进行组合构建（slash command、subagent、hooks、mcp、skills）

1.  试用 Claude Agent SDK 对组合构建成果封装上站（TS SDK - 上站；Python SDK - 数据处理）

• 资源包：本次演示的 skills 链接汇总

◦需求澄清阶段：

▪Brainstorming:

• npx skills addhttps://github.com/obra/superpowers--skill brainstorming

▪Doc-coauthoring

[• npx skills add](https://github.com/anthropics/skills)https://github.com/anthropics/skills--skill doc-coauthoring

◦原型设计阶段：

▪Web-design-guidelines

[• npx skills addhttps:/](https://github.com/vercel-labs/agent-skills)/github.com/vercel-labs/agent-skills--skill web-design-guidelines

▪doc-coauthoring

[• npx skills add](https://github.com/anthropics/skills)https://github.com/anthropics/skills--skill doc-coauthoring

◦开发实现阶段：

▪Web-design-guidelines

[• npx skills addhttps:/](https://github.com/vercel-labs/agent-skills)/github.com/vercel-labs/agent-skills--skill web-design-guidelines

▪Frontend-design

[• npx skills add](https://github.com/anthropics/skills)https://github.com/anthropics/skills--skill frontend-design

▪Shadcn-ui

[•](https://github.com/giuseppe-trisciuoglio/developer-kit) npx skills addhttps://github.com/giuseppe-trisciuoglio/developer-kit--skill shadcn-ui

▪Vercel-react-best-practices

[• npx skills addhttps:/](https://github.com/vercel-labs/agent-skills)/github.com/vercel-labs/agent-skills--skill vercel-react-best-practices

▪seo-audit

[• npx skills addhttps://gith](https://github.com/coreyhaines31/marketingskills)ub.com/coreyhaines31/marketingskills--skill seo-audit

```

### 02. 用多个 Agent 搭建电商短视频生产系统

1. 创意起点与设计思路

1.1 这套思路从哪来

在电商领域，想让一支带货短视频的策划质量在线，单打独斗往往很难搞定，通常得靠几个岗位依次接力：有人专门细看产品的外形、用料和设计感；有人负责摸清竞品的打法、买家的困扰以及行业风向；有人负责打磨出能与同行拉开差距的营销切入点；还有人负责把逐镜头的脚本写出来，并把怎么拍、怎么布景定下来。这几方必须环环相扣、信息一路传下去，最终才能拿出一份真正能执行的方案。

关键发现是：Claude Code 具备多个 Agent 一起干活的本事，刚好能把这种团队作战的方式复刻出来。

```text
一个主控Agent（总监）统筹调度
↓多个子Agent（专家）各司其职
↓输出标准化文档
↓整合成最终成果
```

整套设计思路，可以浓缩成四条：
1. 各司其职：每位 Agent 的职责范围都划得清清楚楚。
2. 步骤有章法：每一环该输入什么、该输出什么，都有规矩可循。
3. 质量能把关：每一道工序都设了核对清单。
4. 成果能上手：最终交付的东西拿来就能用。

1.2 整体结构一览

# 一套能让AI自动做电商视频的“公司化”架构

## 先认识这四类“角色”

```
┌─────────────────────────────────────────────────────────────┐
│                     .claude/ 目录结构                        │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  CLAUDE.md                    ← 主控Agent（视频策划总监）      │
│  │                                                          │
│  ├── agents/                   ← 子Agent定义目录             │
│  │   ├── visual-analyst-agent.md      （产品视觉分析师）      │
│  │   ├── market-researcher-agent.md   （电商情报研究员）      │
│  │   ├── selling-point-manager-agent.md（卖点策划经理）      │
│  │   └── script-director-agent.md     （视频脚本导演）       │
│  │                                                          │
│  └── skills/                   ← Skill定义目录               │
│      └── ecommerce-video-planner/                           │
│          ├── SKILL.md          ← Skill入口文件               │
│          └── references/skills/  ← 工具型Skill参考            │
│              ├── skill_1_image_analyzer.md                  │
│              ├── skill_2_keyword_searcher.md                │
│              ├── skill_3_data_integrator.md                 │
│              ├── skill_4_selling_point_generator.md         │
│              └── skill_5_script_writer.md                   │
│                                                             │

└─────────────────────────────────────────────────────────────┘
```

如果把Claude Code项目比喻成一家公司，那它的组织架构就藏在几个关键文件里：

- **CLAUDE.md**：项目级主控Agent，就是公司的CEO或总监，负责统筹全局。
- **agents/*.md**：子Agent的定义，相当于各个部门负责人，各管一摊。
- **skills/*/SKILL.md**：用户可直接调用的技能，比作对外服务窗口。
- **references/skills/*.md**：工具型参考文件，类似执行工具手册，为Agent提供具体能力。

这套结构来自一个做电商视频策划的Skill示范项目，项目压缩包在![](img/146fd4fc573a21232d7b02f6d31268dd.png)（电商.zip）中。

## 2. 为什么非要用这套分层架构？

很多人的第一反应是：一个Agent搞定所有事不行吗？我们逐一拆解。

### 2.1 主控Agent和子Agent为什么要分开？

如果把所有任务都压在一个Agent身上，会出现几个困境：Prompt变得很长，细节容易漏；角色定位模糊，既要做分析又要做创意；专业度被稀释，质量难以稳定。

分层设计之后，这些问题被化解：每个子Agent只深耕单一领域，Prompt精准度大幅提升；团队协作模拟真实公司，逻辑线清晰；每个环节还能独立测试和调优。

用一张图来看这个类比，会更直观：

```
主控Agent = 项目总监
- 不执行具体任务
- 负责统筹调度
- 校验工作质量
- 整合最终成果

子Agent = 部门专家
- 有明确的职责范围
- 有专业的知识背景
- 输出标准化文档
```

### 2.2 为什么需要工具型Skill参考文件？

子Agent在执行任务时离不开“工具”，例如：图片分析需要调用图像分析工具，市场调研要依赖搜索工具，脚本生成需要专门的内容生成工具。

工具型Skill有非常明确的共性：

1. 纯功能执行：声明“无自主决策能力”，只做工具该做的事。
2. 标准化输入输出：严格约定JSON或Markdown格式，保证接口一致。
3. 单一职责：一个工具只负责完成一个动作，不越界。

这背后的设计意图，可以用下面的示意说明：

```
如果Agent直接执行任务：
- 可能加入主观判断
- 输出格式不稳定
- 难以复用

使用工具型Skill：
- 输出格式固定
- 结果可预测
- 便于后续Agent解析
```

### 2.3 质量校验机制为什么必不可少？

在CLAUDE.md里，每一步都设置了质量校验清单：

```
质量校验：
- [ ] 是否识别出产品品类
- [ ] 是否提取了3个以上视觉卖点
- [ ] 是否提供了搜索关键词建议
- [ ] 报告格式是否完整
```

这个机制的出现，有三个现实原因：

1. AI的输出本身不稳定：同样的提示词，结果可能时好时坏。
2. 流程可靠性需要保障：一个不合格的输出，会影响后面所有环节。
3. 模拟真实管理：就像总监要审核下属提交的成果一样，Agent也需要把关。

如果校验不通过，会触发“打回重做”的处理逻辑：

```
不合格处理：驳回并要求重新分析，说明具体问题。
```

这其实就是现实工作中返工场景的AI版。

### 2.4 输出标准化能带来什么？

每个子Agent都定义了清晰的输出模板：

```
产品视觉特征报告

 基础信息
- 产品品类：[品类]
- 核心材质：[材质列表]

 视觉卖点分析
 卖点1：[卖点名称]
...
```

标准化不是教条，而是为了三个方便：

- 方便传递：下一个Agent能直接解析上一个Agent的输出。
- 方便整合：最终策划案需要汇总所有模块的信息。
- 方便用户阅读：统一格式会更显专业。

## 3. 从零开始搭建这套系统

### 3.1 环境准备

首先创建项目目录，在终端中执行：

Bash
```
mkdir ecommerce-video-planner
cd ecommerce-video-planner
mkdir -p .claude/agents
mkdir -p .claude/skills/ecommerce-video-planner/references/skills
mkdir output
```

创建好的目录结构如下图所示：

Plain Text
```
ecommerce-video-planner/
├── .claude/
│   ├── CLAUDE.md                     主控Agent
│   ├── agents/                       子Agent目录
│   │   ├── visual-analyst-agent.md
│   │   ├── market-researcher-agent.md
│   │   ├── selling-point-manager-agent.md
│   │   └── script-director-agent.md
│   └── skills/
│       └── ecommerce-video-planner/
│           ├── SKILL.md              Skill入口
│           └── references/skills/    工具参考
│               ├── skill_1_image_analyzer.md
│               ├── skill_2_keyword_searcher.md
│               ├── skill_3_data_integrator.md
│               ├── skill_4_selling_point_generator.md
│               └── skill_5_script_writer.md
└── output/                           输出目录
```

### 3.2 创建主控Agent（CLAUDE.md）

主控Agent放在哪？文件位置是：

Plain Text
```
.claude/CLAUDE.md
```

这套系统的大脑就是它，所以在CLAUDE.md里必须定义：人设定位、核心目标、工作流程、校验标准、异常处理。

核心代码框架：

```
电商视频全案策划系统

 人设定位

你是顶级电商代运营公司的视频策划总监，操盘过100+电商爆款单品...

 核心目标

接收用户输入，统筹全流程项目调度，协调4个子Agent完成各自任务...

 统筹的子Agent

| 子Agent | 职责 | 输出物 |
|---------|------|--------|
| visual-analyst-agent | 产品视觉分析师 | 《产品视觉特征报告》 |
| ... | ... | ... |

 标准工作流程

 步骤1：接收用户输入
...步骤2：调度产品视觉分析师
...步骤3：调度电商情报研究员
...步骤4：调度卖点策划经理
...步骤5：调度视频脚本导演
...步骤6：整合输出最终策划案
...步骤7：返回结果
...
```

#### （1）人设定位：给AI一个专业身份

```
人设定位

你是顶级电商代运营公司的视频策划总监，操盘过100+电商爆款单品，精通抖音、淘宝、小红书等全平台电商流量逻辑...
```

这样写有什么好处？它让AI能以专业人士的视角思考；“操盘过100+爆款”这句话能引导AI输出有经验沉淀的内容；同时把能力边界明确为“电商视频策划”，避免跑偏。

#### （2）工作流程：把任务切成清晰步骤

```
步骤2：调度产品视觉分析师

下发任务：
```

执行时，主控Agent会这样调用子Agent：

@visual-analyst-agent请分析以下产品图片，输出《产品视觉特征报告》。

Plain Text
```
接收输出：《产品视觉特征报告》

质量校验：
- [ ] 是否识别出产品品类
- [ ] 是否提取了3个以上视觉卖点
```

把流程步骤化的价值在于：每一步的输入、输出都有预期；质量标准可以提前设定并检查；单个环节出现问题时，修改成本更低。

#### （3）异常处理：给系统装上安全阀

```
异常处理

 图片无法识别
 搜索结果不足
 子Agent输出不合格
```

AI并非全能，容错机制是必需的。它既能兜底，也能给用户明确的下一步建议，整个系统的鲁棒性因此更强。

### 3.3 创建各个子Agent

#### 3.3.1 产品视觉分析师Agent

文件位置：`.claude/agents/visual-analyst-agent.md`

设计时要注意三点：设置专业背景（例如“8年经验”），划清能力边界（只负责视觉、不碰市场调研），以及定义输出格式。

```
---name: visual-analyst-agent
description: 产品视觉分析师Agent。8年电商产品视觉分析经验...
---子Agent1：产品视觉分析师

 人设定位
你是一位拥有8年电商产品视觉分析经验的资深专家...

 核心目标
深度解析产品图片，输出标准化、结构化的《产品视觉特征报告》...

 专属工具箱
- skill_1_image_analyzer：图片视觉特征提取器

 专业能力边界
- ✅ 从图片中提取客观存在的视觉特征
- ❌ 不进行市场竞品分析（由电商情报研究员负责）

 输出报告格式
[标准模板...]
```

#### 3.3.2 电商情报研究员Agent

文件位置：`.claude/agents/market-researcher-agent.md`

它的核心职责是：接收视觉分析师产出的报告，调用搜索工具做市场调研，然后把竞品信息、用户痛点、行业趋势整合成一份情报。

关键设计如下：

```
专属工具箱
- skill_2_keyword_searcher：电商关键词搜索器
- skill_3_data_integrator：电商数据整合器
```

这里之所以设置两个工具，是因为搜索器只负责获取原始数据，整合器负责提炼核心信息，分工清晰后输出质量更可控。

#### 3.3.3 卖点策划经理Agent

文件位置：`.claude/agents/selling-point-manager-agent.md`

它的职责是把视觉特征和市场情报结合起来，提炼出分层卖点：核心卖点、差异化卖点、情感化卖点。

分层体系的代码设计：

```
卖点分层设计

 核心卖点（1个）
最强的功能/价值主张

 差异化卖点（2个）
与竞品形成区隔的独特优势

 情感化卖点（1个）
击中用户心理需求，创造情感共鸣
```

为什么非要分层？因为30秒的视频承载不了所有卖点。核心卖点负责主打，差异化卖点建立竞争壁垒，情感化卖点刺激购买冲动。

#### 3.3.4 视频脚本导演Agent

文件位置：`.claude/agents/script-director-agent.md`

它要做的是：根据卖点清单确定视频类型，输出分镜头脚本，并整理拍摄执行清单。

30秒视频的框架结构：

```
30秒视频结构

| 时长 | 内容 | 目的 |
|------|------|------|
| 0-3s | 钩子 | 抓住注意力 |
| 3-12s | 核心卖点 | 传达价值 |
| 12-20s | 差异化 | 建立优势 |
| 20-27s | 情感共鸣 | 触发认同 |
| 27-30s | 转化引导 | 促进行动 |
```

为什么选择30秒？一是短视频平台的推荐逻辑更偏爱完播率高的内容，30秒刚刚好；二是信息密度适中，用户不容易产生认知负担。

### 3.4 创建Skill入口文件

文件位置：`.claude/skills/ecommerce-video-planner/SKILL.md`

YAML头部的定义：

```
---name: ecommerce-video-planner
description: 电商视频全案策划系统。用户上传产品图片后，自动完成「产品视觉解析→市场情报调研→核心卖点提炼→短视频脚本全案输出」全流程...
---
```

这里的description非常重要，Claude Code会根据描述判断何时触发这个Skill，所以关键词和触发场景必须写清楚。

接下来展示整套系统架构：

```
系统架构

用户上传产品图片
↓┌─────────────────────────────────────┐
│     电商视频策划总监（总控Agent）      │
└─────────────────────────────────────┘
↓┌───────────────────────────────────────┐
│          子Agent协同工作流              │
├───────────────────────────────────────┤
│ 1️⃣ 产品视觉分析师 → 《产品视觉特征报告》 │
│ 2️⃣ 电商情报研究员 → 《电商市场情报简报》 │
│ 3️⃣ 卖点策划经理   → 《分层卖点清单》    │
│ 4️⃣ 视频脚本导演   → 《电商视频落地执行案》│
└───────────────────────────────────────┘
```

给用户看架构图有三个好处：用户理解原理后会更信任；能够提前预知输出内容；整体体验更完整。

### 3.5 创建工具型Skill参考文件

工具型Skill遵循统一的设计原则，所有文件都具备相同的骨架：纯功能执行、标准化输入输出、单一职责。按照这三个规范，就能为子Agent配置出稳定可复用的工具集。

```
---name: tool-name
description: 工具描述
---工具名称

你是一个纯功能执行的[工具类型]，无任何自主决策能力。

 输入参数
| 参数名 | 类型 | 是否必填 | 描述 |
...执行指令
1. 步骤一
2. 步骤二
...输出规范
[严格的格式定义]

 执行原则
- 原则1
- 原则2
...
```
## 先说清：它只辅助，不拍板  
这套系统不会替你拿主意。它把读图、搜词、整理、写脚本等环节串起来，给出的是可参考的方案，最终取舍仍然由你判断。

```
普通Agent：
- 可以根据情况调整输出
- 可以添加主观判断
- 输出有一定灵活性

工具型Skill：
- 严格按格式输出
- 不添加额外内容
- 便于程序化解析
```
## 工具 1：商品图视觉特征抓取  
- 文件：skill_1_image_analyzer.md  
- 输入：商品图片  
- 输出：JSON 结构的视觉特征  

```
{&quot;category&quot;: &quot;产品品类&quot;,
  &quot;core_materials&quot;: [&quot;材质1&quot;, &quot;材质2&quot;],
  &quot;color_style&quot;: &quot;颜色+风格&quot;,
  &quot;visual_selling_points&quot;: [&quot;卖点1&quot;, &quot;卖点2&quot;, &quot;卖点3&quot;],
  &quot;usage_scenarios&quot;: [&quot;场景1&quot;, &quot;场景2&quot;],
  &quot;suggest_search_keywords&quot;: [&quot;关键词1&quot;, &quot;关键词2&quot;]
}
```
为何选用 JSON？因为结构化数据方便后续 Agent 读取；同时字段固定，关键信息不会漏。

## 工具 2：电商关键词检索工具  
- 文件：skill_2_keyword_searcher.md  
- 主要思路：三路搜索  

```
1. 竞品卖点搜索：搜索&quot;[关键词] + 卖点/特点/优势&quot;
2. 用户痛点搜索：搜索&quot;[关键词] + 痛点/问题/差评&quot;
3. 行业趋势搜索：搜索&quot;[关键词] + 趋势/新品/2024&quot;
```
为何要拆成三路？这样能看到更完整的市场情报；各路信息各有用途，方便后续对照和整合。

## 工具 3：电商信息归纳器  
- 文件：skill_3_data_integrator.md  
- 职责：把检索结果压缩到前三名  

```
输出结构

 1. 核心竞品卖点TOP3
| 排名 | 卖点描述 | 信息来源备注 |

 2. 用户高频痛点TOP3
| 排名 | 痛点描述 | 典型用户反馈 |

 3. 行业热门趋势
```
为何只取前三名？候选太多会干扰判断；把目光集中在最有价值的信息上，决策更高效；30 秒视频也放不下太多卖点。

## 工具 4：分层卖点生成器  
- 文件：skill_4_selling_point_generator.md  
- 设计原则：每一条卖点都要有依据  

```
| 卖点层级 | 卖点内容 | 支撑依据 |
|----------|----------|----------|
| 核心卖点 | [内容] | 图片特征：xxx；市场数据：xxx |
```
背后考量是什么？一是防止凭空编造；二是让卖点基于真实资料；三是便于日后核验。

## 工具 5：分镜脚本写作器  
- 文件：skill_5_script_writer.md  
- 设计原则：按平台调整脚本  

```
平台规则参考

- 抖音：前3秒必须有强钩子，30秒内
- 淘宝：45-60秒，重点展示细节
- 小红书：注重真实感和种草感
```
为何要按平台调整？因为各平台的推荐规则、观众偏好和审核尺度都不同，照搬难以见效。

## 3.6 搭建流程回顾  
**步骤回顾**  
整个流程按顺序串联：商品图分析 → 关键词检索 → 数据归纳 → 卖点生成 → 脚本写作。前一步的输出会作为后一步的输入。

```
1. 创建目录结构
   └── mkdir .claude/agents, .claude/skills/...

2. 编写主控Agent
   └── CLAUDE.md（人设、流程、校验）

3. 编写子Agent
   └── 4个专业Agent，各司其职

4. 编写Skill入口
   └── SKILL.md（触发条件、使用说明）

5. 编写工具参考
   └── 5个工具型Skill（标准化输入输出）
```
**文件依赖关系**  
文件之间也存在依赖：只有先拿到视觉特征和检索数据，后面的整合和脚本才有素材可用。

```
CLAUDE.md（主控）
    ├── 调用 → visual-analyst-agent.md
    │            └── 参考 → skill_1_image_analyzer.md
│├── 调用 → market-researcher-agent.md
    │            ├── 参考 → skill_2_keyword_searcher.md
    │            └── 参考 → skill_3_data_integrator.md
│├── 调用 → selling-point-manager-agent.md
    │            └── 参考 → skill_4_selling_point_generator.md
│└── 调用 → script-director-agent.md
                 └── 参考 → skill_5_script_writer.md
```
## 4. 输出结果示例  
### 4.1 最终产出  
系统运行结束后，output/ 目录下会生成结果文件。

```
output/
└── 电商视频策划案_20240315_1430.md
```
### 4.2 策划案结构示例  
策划案按固定结构输出，方便直接查看和用于拍摄。

```
电商视频全案策划案

产品：智能保温杯
平台：抖音
日期：2024-03-15

---一、产品视觉分析摘要

品类定位：智能保温杯
核心材质：316不锈钢 + 食品级PP
视觉风格：极简白色、商务风
核心视觉卖点：
- LED温度显示面板
- 双层真空结构
- 触控唤醒设计

---二、市场情报摘要

竞品主攻方向：
- 保温时长（12小时/24小时）
- 材质安全（304/316不锈钢）
- 容量规格（350ml/500ml）

用户核心痛点：
- 不知道水温容易烫嘴
- 清洗困难，杯盖藏污纳垢
- 外出携带不便，容易漏水

行业趋势：
- 智能化：温度显示、饮水提醒
- 健康化：抗菌材质、易清洗设计
- 颜值化：联名款、个性化配色

差异化机会：
- 温度可视化是痛点解决方案
- 触控唤醒比竞品的敲击唤醒更灵敏

---三、核心卖点策略

 🎯 核心卖点
一眼就知道水温，再也不怕烫嘴了

- 功能支撑：LED温度显示面板
- 用户利益：避免烫伤，随时喝到适温水
- 支撑依据：用户痛点&quot;不知道水温容易烫嘴&quot;排名第一

 ⚡ 差异化卖点1
触控即亮，比敲击唤醒灵敏3倍

- 与竞品差异：竞品需要敲击唤醒，触控更灵敏
- 用户利益：更便捷，单手操作

 ⚡ 差异化卖点2
一体成型杯盖，水洗不掉链

- 与竞品差异：传统杯盖结构复杂，藏污纳垢
- 用户利益：清洗方便，卫生


 ❤️ 情感化卖点
办公室的你，值得一杯&quot;懂你温度&quot;的水

- 情感触发点：被关爱、被理解
- 场景代入：忙碌工作中，它默默守护你的水温

---四、视频执行方案

 视频类型
痛点解决型 - 直接击中&quot;不知道水温&quot;的痛点

 分镜头脚本（30秒）

| 时长 | 画面 | 口播 | 重点 |
|------|------|------|------|
| 0-3s | 热气腾腾的水杯特写，手被烫到的惊恐表情 | &quot;每次喝水都像在赌博？&quot; | 钩子：痛点场景 |
| 3-12s | 手指轻触杯盖，LED屏幕亮起显示56℃ | &quot;这个保温杯，一触就知道水温&quot; | 核心卖点展示 |
| 12-20s | 分屏对比：敲击vs触控，触控响应更快 | &quot;触控唤醒，比敲击灵敏3倍&quot; | 差异化卖点 |
| 20-27s | 白领在办公室优雅喝水的场景 | &quot;忙碌的你，值得一杯懂你温度的水&quot; | 情感共鸣 |
| 27-30s | 产品全景+价格/优惠信息 | &quot;限时福利，点击下方链接&quot; | 转化引导 |

 流量配套

标题方案A（痛点型）：
&gt; 喝水总被烫？这个保温杯一眼就知道水温！

标题方案B（利益型）：
&gt; 316不锈钢+温度显示，这个保温杯太懂你了

视频标签：
保温杯 智能保温杯 办公室好物 喝水神器 温差显示杯

话题标签：
办公室必备 打工人日常

 拍摄清单

必拍镜头：
- [ ] 钩子镜头：热气+被烫到的表情特写
- [ ] 产品全景：45度角，展示LED面板
- [ ] 核心功能：触控唤醒+温度显示的特写
- [ ] 对比镜头：敲击vs触控的响应对比
- [ ] 使用场景：办公室桌面，搭配笔记本电脑
- [ ] 转化镜头：产品包装+优惠信息

拍摄注意事项：
1. 光线：自然光为主，侧光突出产品质感
2. LED屏幕：确保数字清晰可见
3. 节奏：快切配合音乐卡点
4. BGM：轻快节奏感强，建议BPM 120+

---五、执行建议

 拍摄要点
- LED屏幕是核心，务必确保清晰可见
- 触控唤醒需要特写，展示响应速度
- 情感场景要有代入感，避免过于营销

 避坑提醒
- 不要使用&quot;最好&quot;&quot;第一&quot;等绝对化用词
- 温度显示需要真实，不能后期合成
- 避免夸大保温时长

---附录：完整报告（折叠）

&lt;details&gt;
&lt;summary&gt;点击展开完整报告&lt;/summary&gt;

 产品视觉特征报告（完整版）
[...]

 电商市场情报简报（完整版）
[...]

 分层卖点清单（完整版）
[...]

 电商视频落地执行案（完整版）
[...]

&lt;/details&gt;
```
## 5. 操作指南  
### 5.1 快速开始  
先安装 Claude Code。  

```
如果尚未安装Claude Code CLI
npm install -g @anthropic/claude-code
```
进入项目目录。  

```
cd ecommerce-video-planner
```
启动 Claude Code。  

```
claude
```
在对话中触发 Skill。  

```
帮我策划一个电商视频
```
也可以直接上传商品图片，并在提示里说明需求。  

```
这是我的一款产品，帮我做个抖音带货视频策划
```
### 5.2 输入要求  
**必填项**  
- 商品图片：需清晰展示商品，支持 JPG/PNG。  

**可选项**  
- 商品品类：AI 判断不准时可手动指定，比如“智能保温杯”。  
- 目标平台：指定投放渠道，如“抖音”。  
- 目标人群：如“白领女性”。  
- 特殊要求：如“突出性价比”。  

![](img/8578043ca393de1f2b70a5831e09255f.png)
### 5.3 使用示范  
**示例 1：基础场景**  

```
[上传产品图片]
帮我策划这个保温杯的抖音带货视频
```
用户输入：提供商品图片，或直接输入指令。  
系统响应：返回一份基础策划。  

```
收到您的产品信息，我将为您策划一份完整的电商视频全案。

📋 输入确认
- 产品品类：智能保温杯
- 目标平台：抖音
- 补充信息：无

🚀 即将开始全流程策划
1. 产品视觉特征分析
2. 电商市场情报调研
3. 核心卖点提炼
4. 视频脚本全案输出
```
**示例 2：补充更多信息**  

```
[上传产品图片]
这是一款新出的护肤精华，主要成分是玻尿酸
目标平台：小红书
目标人群：25-35岁都市女性
```
用户输入：在图片之外，补充品类、人群、平台等。  
系统响应：输出更贴合需求的策划。  

```
收到您的产品信息，我将为您策划一份完整的电商视频全案。

📋 输入确认
- 产品品类：护肤精华（玻尿酸成分）
- 目标平台：小红书
- 补充信息：目标人群25-35岁都市女性

🚀 即将开始全流程策划
...
```
**示例 3：多平台需求**  

```
[上传产品图片]
这个产品要在淘宝和抖音同时推，帮我分别策划视频
```
用户输入：明确要投放抖音、淘宝、📕等多个平台。  
系统响应：分别给出适配版本。  

```
收到您的需求，我将为您生成两套策划案：

📋 输入确认
- 产品品类：[识别结果]
- 目标平台：淘宝 + 抖音

📊 将输出
1. 抖音版策划案（30秒快节奏）
2. 淘宝版策划案（45-60秒详细版）

🚀 即将开始全流程策划
...
```
### 5.4 输出文件说明  
**文件位置**  
结果保存在 output/ 目录。  

```
output/电商视频策划案_YYYYMMDD_HHMM.md
```
![](img/c8ef53720ffba280d37c8de272242c02.png)
**文件内容**  
策划案包含以下模块：  
- 商品视觉分析摘要：描述外观、材质、风格，用于认识商品。  
- 市场情报摘要：整理竞品、痛点、趋势，辅助判断市场环境。  
- 核心卖点策略：提供 4 个分层卖点，构成视频核心信息。  
- 视频执行方案：给出分镜脚本、标题和标签，可直接用于拍摄。  
- 执行建议：列出拍摄要点和常见坑，供执行时参考。  

![](img/d84292fdf213e61f381c6929de0aea5f.png)
### 5.5 高频疑问  
**Q1：图片识别不准怎么办？**  
处理方式：换更清晰的商品图；在输入里补充商品描述；或手动指定品类。  

**Q2：搜不到足够的搜索结果？**  
可能原因：商品比较冷门，或关键词选择不够准确。  
处理方式：补充更多商品背景；指定竞品品牌；系统也会在现有信息基础上继续完成策划。  

**Q3：想修改已生成的策划案？**  
直接在 Claude Code 中继续对话，提出调整要求即可。  

```
把核心卖点改成突出&quot;便携性&quot;
```
比如要求替换某个卖点。  

```
把视频时长改成60秒
```
或者换成另一种视频风格。  

```
再给我几个标题备选
```
也可以要求增加新的平台版本。  

**Q4：支持哪些平台？**  
- 抖音 ✅：30 秒快节奏，前几秒抓人。  
- 淘宝 ✅：45–60 秒详细讲解。  
- 📕 ✅：真实使用感受。  
- 快手 🔄：可沿用抖音版。  
- 视频号 🔄：可沿用抖音版。  

**Q5：如何单独调试某个环节？**  
如果某个阶段的输出不理想，可单独要求重跑该环节。  

```
重新分析产品图片，我需要更多视觉卖点
```
例如重新生成卖点。  

```
市场调研太少了，帮我补充更多竞品信息
```
或者重写分镜脚本。  

### 5.6 进阶用法  
以下为可扩展操作。  

```
给我提炼5个卖点，视频时长60秒
```
自定义卖点数量。  

```
这个产品适合走科技感风格，帮我调整脚本
```
指定视频风格。  

```
[上传多张产品图片]
帮我对比这三款产品，分别策划视频
```
对比多款商品。  

```
最近&quot;XX话题&quot;很火，帮我结合这个热点策划视频
```
结合近期热点。  

### 5.7 实操建议  
**上传图片建议**  
分辨率至少 1080P；多拍几个角度；用自然光或专业灯光；背景干净整洁。  

**补充信息建议**  
信息描述得越具体，策划结果就越贴合预期。  

```
[上传产品图片]
产品：便携式榨汁机
核心功能：30秒快速榨汁
目标人群：健身爱好者、上班族
核心卖点希望突出：便携+快充
竞品参考：XX品牌
```
**策划案使用建议**  
拍摄前熟读拍摄清单并备好道具；拍摄中按分镜脚本执行并留意要点；剪辑时参考节奏建议和 BGM 风格；发布时使用配套标题和标签。  

### 5.8 附录：文件清单  
项目文件按结构存放，可查看技能文件与输出结果的目录。

```
.claude/
├── CLAUDE.md                           主控Agent定义
│├── agents/
│   ├── visual-analyst-agent.md         子Agent1：产品视觉分析师
│   ├── market-researcher-agent.md      子Agent2：电商情报研究员
│   ├── selling-point-manager-agent.md  子Agent3：卖点策划经理
│   └── script-director-agent.md        子Agent4：视频脚本导演
│└── skills/
    └── ecommerce-video-planner/
        ├── SKILL.md                    Skill入口文件
        └── references/skills/
            ├── skill_1_image_analyzer.md        工具1：图片分析器
            ├── skill_2_keyword_searcher.md      工具2：关键词搜索器
            ├── skill_3_data_integrator.md       工具3：数据整合器
            ├── skill_4_selling_point_generator.md  工具4：卖点生成器
            └── skill_5_script_writer.md         工具5：脚本撰写器
```

**这些文件，各自负责什么？**

| 文件 | 类型 | 定位 |
| --- | --- | --- |
| CLAUDE.md | 主控 | 总览全局工作流 |
| *- agent.md | 子 Agent | 明确专家角色分工 |
| SKILL.md | 入口 | 设定触发规则与使用方式 |
| skill_*.md | 工具 | 统一输入输出格式 |

**最后的话**

恭喜你！当Claude code、Skills、Open Claw都被你顺利装好，并成功完成实战篇的第一个案例时，你已经正式站上了AI编程的起点。学习不会就此停止，更多精彩还在后面等着你去发现。接下来，不妨让这些AI工具走进你的日常业务，在一次次真实任务中与你并肩作战，你的成长会超乎预料。

一起把AI用起来，跟上这个大时代，一起龙哥盟！

![](img/60723d70ec2997b06a730b18390e0ea2.png)

```

```