# AI 编程入门（含 OpenClaw / Skills）

> 来源：[https://my.feishu.cn/docx/Fv3ldAuehoDvWuxMxdicmrSDnEf](https://my.feishu.cn/docx/Fv3ldAuehoDvWuxMxdicmrSDnEf)

<https://my.feishu.cn/sync/Lj5sd8APisk896bxImEcYvjMnlF>

# 引言：

## 开船第一课

### ⛵新手如何入门【AI 编程入门（含 OpenClaw/Skills）】项目？

1.  项目情况

随着 AI 的快速发展，现在一个不懂技术的人也可以借助 AI 工具做出产品。生财往期开过不少 AI 编程相关的航海，但我们观察到 AI 编程对新手来说还是有难度的。

所以这次航海，我们**决定带大家从最基础、最好用**的工具组合入手，通过Claude code、Skills以及近期非常热门的OpenClaw（小龙虾），帮大家扫清入门障碍，真正让 AI 工具为自己的业务赋能。

这一次航海的目标很简单：先把工具装起来，能用起来，做出 1 个实用的东西。

为什么是这三个工具？

**Claude Code**

是目前对新手最友好的 AI 编程工具。你不需要懂编程，只要能清楚描述需求，它就能帮你写代码、做产品。往期航海中，很多圈友用它做出了网站、小程序、app。

**Skills**

可以把你日常重复做的事情变成自动化流程。比如写公众号、发小红书、整理数据，以前需要在 n8n 里拖拽配置各种节点，现在直接用自然语言描述需求就能创建。

**OpenClaw**

是最近很火的 AI 助手。你创建好的 Skills 可以交给它去执行，它就像一个 24 小时不休息的员工，可以帮你监控邮件、定时发布内容、整理文件等。

等你深入掌握这三个工具后，就可以让 Claude Code 帮你做产品，Skills 帮你做自动化，OpenClaw 帮你 24 小时执行，三者结合起来，就是一套完整的 AI 工作流系统。

**考虑到很多人对这些工具完全**不了解，所以这次航海的重点是入门和上手。

必**修篇会带你完成环境配置、工具安装、基础操作，争取让大家把这三个工具**安装跑起来，同时能够在实际场景中去运用这些 AI 工具，比方说用 Skills 实现自媒体自动化、改编漫剧剧本，用 OpenClaw 打造个人专属知识库、实现个人 IP 型公众号自动化、搭建专属 AI 客服等

而选修篇会提供一些进阶玩法，如打造 AI 应用开发 skills、用 OpenClaw 生成 AI 漫剧等有难度的案例，让有能力的船员可以继续探索。

![](img/e3c47a8ff1f3510c149a297c671309af.png)

1.  项目完整操作思路

**2.1 项目完整操作思路**

完成 Claude Code 安装部署（关键）>掌握 Claude Code 入门实操案例> 完成 Claude Skills 安装部署（关键）> 掌握 Claude Skills 入门实操案例> 完成 OpenClaw 安装部署（关键）>掌握 OpenClaw 入门实操案例

![](img/26a3ab9060b3a8496ced6891260b5adb.png)

**2.2 操作重点**

本次手册会包含三个 AI 工具，Claude code、Claude Skills 和 OpenClaw ，但是大家不用觉得很复杂，当你安装好 Claude code 后，后面的两个工具安装和使用的难度会降低很多

**希望大家在这**个过程中，可以更好的培养“万事问 AI”的习惯，在跟着手册实操的过程中，遇到的任何问题和卡点，都可以截图问 Claude code，让 Claude code 帮你解决。

而大家在这个过程中，不仅学会如何使用 skills 和 OpenClaw ，更重要的是能够培养这样的一种 AI 思维，解决我们会遇到的各种问题，用 AI 为自己的业务赋能

**2.3 新手入门建议&避坑指南**

**新手入门建议：**

• 我完全不懂编程，可以学吗？答：可以。航海从安装环境、认识工具开始，用现成提示词和案例带你完成安装工具的部署和案例的学习，不要求你会懂代码，并且在每一个实操案例中，我们都提供视频+图文教程，方便你更好的学习。

• 需要付费订阅 Claude 官方吗？成本高吗？

**答**：不需要。本次航海主要使用国产模型**MiniMax2.7驱动 Claude Code，部分套餐是 50 元/月。相比 Claude 官方的 20 美元/月，成本降低了很多，而且没有网络限制。

• 搭建过程中遇到报错或不会的怎么办？

答：遇到报错很正常，别担心！我们会尽可能提供稳定的流程。在实操的过程中，遇到问题 ，可以向 AI 提问来解决，或者是群内举手向教练问题。

• Skills 和 n8n、Coze 有什么区别？

答：Skills 是【口喷式】，直接用自然语言描述需求就能创建；n8n 和 Coze 是【拖拽式】，需要配置节点、 连线。Skills 更简单、更智能，而且可以自动触发，不需要手动配置复杂的工作流。

**风险挑战和应对建议：**

挑战一：编程工具使用门槛与本地环境配置困难

建议：航海手册按 Windows 和 Mac 分步骤演示，从零带你安装 Git、VS Code、Claude Code，并准备常见报错截图对照表，遇到“没有权限/命令无效”等问题可以直接按示例排查，可以跟着航海手册的视频+图文教程学习。

挑战二：Skills 创建失败或效果不理想

建议：Skills 的质量取决于你的需求描述是否清晰。前期建议先跟着手册的步骤来搭建 Skills（如公众号自动生成、小红书自动发布等），熟悉流程后再自己创建。手册中提供了大量 Skills 案例，可以直接参考使用。

挑战三：实操过程中遇到的内容和手册写的不一样怎么办

建议：不用担心，因为每个人的电脑版本不一样，环境不一样，所以出现和手册不一样的情况也很正常，可以直接把你的实操结果截图像你的 AI 提问，问它这个截图是什么，为什么会这样，如果出现报错要怎么修改

风险一：AI 编程属于有难度的技能学习，需做好心理准备

建议：大家保持开放的学习心态，相信一分耕耘一分收获，每一次学习都是一个进步点，同时养成万事问 AI 的习惯，安装好 Claude code 后，遇到的问题都可以找 Claude code 询问答案

风险二：OpenClaw 部署门槛高，本地部署有风险

建议：OpenClaw 在 本次航海中主推荐使用云服务器部署（腾讯云/阿里云）。手册中会提供详细的云服务器部署教程，降低大家部署难度，我们先把 OpenClaw 安装用上，同时大家在使用 OpenClaw 的时候要注意风险问题，不要给 OpenClaw 那么大的权限，避免自己的资料被删除了也不知道

风险三：使用过程中 Token 消耗快，成本控制

建议：合理使用模型，不要频繁生成大量内容。OpenClaw 执行任务时会消耗 Token，建议设置好任务频率，避免无意义的重复执行。

**2.4 开船前必备工具**

• 需配置网络环境

• 飞书账号（用于 OpenClaw 集成）

• Claude 账号或 MiniMax/GLM-5/Kimi 等国内模型（部分模型最低 50 元/月）

• 云服务器（腾讯云/阿里云，用于部署 OpenClaw），最低套餐是 20 元/月起步

• 一台能正常使用的电脑（Windows 或 Mac 均可，推荐 Mac）

AI 时代，让我们从 AI 编程入手，实现普通人的跃迁，加油；

**我们相信，进一寸有一寸的欢喜，希望**大家能够享受自己的 AI 编程入门之旅！

![](img/eda5047bcedbb9e0ca507069411e1e59.png)

# 必修篇：

## 一、Claude code 的安装与部署

### 01.入门：全面认识 Claude code

1.  本章概要

💡在引言中，我们已经认识了 Claude Code 这个 AI 编程助手，相信你已经对它如何提升开发效率充满了期待。但再强大的 AI 工具，如果只停留在概念层面，也无法真正为你解决实际的难题。

现在，是时候动手把它真正安装到你的电脑中了。本章将带你跨过从理论到实操的第一道门槛，亲手搭建一个属于自己的 AI 编程环境。正所谓“工欲善其事，必先利其器”，完成基础环境的配置，是我们开启 AI 辅助编程之旅的基石。

在本章中，你将亲手实践：

• **搭建基础环境**：清晰了解并安装 Git、Node.js 和 VS Code 等必要组件，确保你的电脑具备运行 Claude Code 的底层能力。

• **完成工具部署**：学习如何在 Mac 或 Windows 系统中通过命令行正确安装 Claude Code，掌握基础的终端操作指令，让 AI 助手随时待命。

• **配置国产模型**：掌握使用 cc-switch 接入 国产模型的方法，解决网络限制与支付门槛，实现低成本、高稳定性的本地化运行。

• **AI 产品开发**：安装好 Claude code** 后，大**家可以根据案例的实操一步步把这个早读神器打造出来，感受 AI 开发产品的魅力

通过本章的学习，你将不再只是 AI 编程的旁观者，而是下场实战，能够安装你自己的 Claude code 工具，并且用 Claude code 打造出自己的产品。让我们一起动手，为你的 AI 编程之旅打下坚实的第一步。

💡

**本章航线图**

完成本章节的学习和实操，即可完成航线图的第一阶段。

第一阶段：Claude Code 的安装和部署（约 7 天）

完成 Claude Code 环境配置（约 5 天）

熟悉 Claude Code 页面和常见操作（约 0.5 天）

完成 Claude Code 第一个实战案例（约 1.5 天）

![](img/6a06080d13eddb134d98ef0b12e27437.png)

1.  Claude Code 是什么

**注意：使用 Claude Cod**e 需要【配置上网环境】，才能安装和使用

**一句话**

：Claude Code 是一个能“读懂你的代码库、用自然语言和你协作写代码”的智能编程助手。

**标准定义**

：它基于 Anthropic 的大语言模型，为编码任务做了专项增强（长上下文理解、项目级改写、自动生成/修复、解释与重构等），既能在命令行中工作，也能与编辑器/项目工具链配合，完成从 0 到 1 的构建与日常维护。

Claude code 作为**AI 编程工具的**一种，让我们普通人也有机会做出 AI 产品

过去要把想法变成能用的产品，要有专门的程序员去完成需求。但现在不一样了。

即使你对代码一窍不通，也能借助**AI 编程工具****快速把想法落**地。这种变化不是渐进式的改良，而是颠覆性的重构。

就在生财来说，这里有太多生动的例子，不少圈友从来没写过一行代码，却靠着Cursor、Claude Code这些工具，实实在在地做出了自己的应用。有人用它开发了海外工具站，有人搭建了自动化工作流，有人甚至做出了能赚钱的小程序。

这里面的差距已经不是效率高一点那么简单了。会用 AI 编程和不会用 AI 编程的人，生产力的差距可能是十倍、甚至百倍的量级。一个懂得如何和 AI 协作的人，可以在一天内完成过去一个小团队一周的工作量。更关键的是，这种能力正在重新定义"谁能创造价值”，技术不再是壁垒，想法和执行力才是。

有了 Claude code 这样的 AI 工具，你不再需要把 80%的精力花在写代码上，而是可以专注于真正重要的事情，那就是创意、产品设计、用户体验。代码实现？交给 AI。你负责想清楚"要做什么"和"为什么这么做"，AI 负责怎么做，极大解放你的时间精力。

2.为什么要用 Claude Code

过去要成为开发者，你得先翻厚厚的编程书，啃下复杂的专业术语和概念，再折腾各种框架配置。学习周期动辄半年起步，投入的时间成本高得惊人。很多人就是在这个阶段放弃了，不是因为不够聪明，而是因为这条路实在太陡峭。

但 AI 时代彻底改写了这个游戏规则。现在的核心能力不再是记住编程**语法，而是学会和 AI** 对话。你需要做的是清晰地描述你的需求，用最自然的语言告诉Claude code这样的 AI 工具 你想要什么。AI 会基于你的描述生成代码，给出多种实现方案。你的工作变成了从这些方案中挑选最合适的那个，然后继续对话，比如："这里的逻辑能不能调整一下""能不能加个导出功能"。就这样一轮轮迭代，项目在你和 AI 的协作中逐渐成型。

对于不同阶段的人，Claude code 发挥的用处也不同

**对新手**

• **上手快**：不会写也能“跑起来”——把需求讲清楚，它给出能运行的初稿。

• **学得快**：让它逐行解释、对比写法、指出 bug 的成因，“边用边学”比死记语法高效。

• **错误不恐惧**：报错时直接请它定位并给修复方案与测试样例。

**对有经验开发者**

• **效率倍增**：样板/重复工作交给它，人专注架构、边界与质量。

• **原型极致快**：半天做完过去一周的雏形；可以并行尝试多条技术路径。

• **质量护栏**：让它做代码走查、补注释与测试，减少“技术债”。

**对团队/项目**

• **知识对齐**：把隐性经验外化为对话、注释与脚本，降低新人融入成本。

• **沟通收敛**：在对话里固化需求、接口与验收标准，减少往返。

下面对传统编程和 AI 辅助编程进行一些维度对比：

| 维度 | 传统编程 | AI 辅助编程 |
| --- | --- | --- |
| 定义 / 驱动方式 | 开发者手动编写代码、设定逻辑、定义流程，代码主要由人决定“做什么、怎么做”。 | 开发者更多地借助人工智能工具（如大语言模型、代码生成/补全助手）来生成、建议、优化代码，变成“人 + AI” 人机协同的形式完成一个项目。 |
| 编码工作量 | 程序员需要从头定义算法、流程、结构、接口、细节。 | 很多重复、模板化或样式化的编码任务可由 AI 自动完成，人主要负责提需求、验证、监督。 |
| 专注点 /技能要求 | 强调编程语言熟练、逻辑思维、数据结构、算法、架构能力。 | 除了传统技能，还越来越强调如何与 AI 协作、如何给出「好的提示词」、如何验证 AI 产出的代码、如何管理 AI 生成的系统。 |
| 速度／效率 | 在可预见、结构化明确的项目中效率较高，但面对大量重复或模板化任务耗时。 | AI 辅助可显著提高开发速度，尤其在 boilerplate、重复逻辑、原型阶段表现强。 |
| 代码质量／可维护性 | 代码结构、逻辑可被开发者理解、维护责任清晰。 | 生成速度快，对于大型的项目 AI 生成代码可能带来可读性差、结构重复、隐藏缺陷或安全风险。 |
| 学习门槛／入门 | 学习编程语言、算法、工程思维需要一定时间；新手可能起步慢。 | 借助 AI 辅助，新手可以更快产生可运行代码，降低起步门槛。我们可以以学代练，在 AI 编程的过程中掌握编程 |
| 适用场景 | 适合高复杂度、需求模糊、需创新、对质量有高要求的项目。 | 适合重复性任务、快速原型开发、标准模块生成、初稿编写、提高开发效率的场合。 |
| 工具／生态变化 | 传统 IDE + 手写/模板代码模式。 | 大量 AI coding 工具（比如代码生成、补全、生成、语义搜索、错误检测、自动测试等）正在普及。 |

![](img/4d49429355050ff555a3a01439d7b112.png)

1.  安装 Claude code 时常见的概念

在开始安装 Claude code 之前，我们需要先理解几个会反复出现的核心名词。它们听起来陌生，但其实各自扮演着非常清晰的角色。理解这些，就相当于理解了 Claude Code 运行的底层逻辑新手

**⚠**️注意：以下都是名词概念解释，方便大家在安装 Claude code 时，对这个名词有基本了解，不做重要学习内容

3.1 Git 是什么

Git 是一个**代码版本管理系统**，可以记录你对代码的每一次修改，就像“时间机器”。你写的每一段代码都能被追溯、回退或对比，不管团队协作还是个人项目，都能防止“手滑改崩”或“忘了昨天改了啥”。

在 Claude Code 的世界里，Git 的作用非常重要：当你让 Claude 修改、生成或重构代码时，它能自动帮你记录改动历史，让你随时对比 AI 修改前后的版本。Claude 甚至可以直接读取 Git 提交记录，帮你理解整个项目的变更脉络。可以这样理解：Git 负责记忆，Claude Code 负责思考。两者配合，你的开发就既安全又高效。

![](img/d97bc650d728af3f68b0d71c67c76412.png)

如果你想学习入门 Git 是什么， 可以看看下面的这个视频。对于新手的普及还是不错的。

[https://www.douyin.com/video](https://www.douyin.com/video/7459207071368629516)/7459207071368629516

3.2 VS Code 是什么

VS Code 是由微软推出的一款轻量、免费的代码编辑器。它是目前全球最受欢迎的开发工具，支持几乎所有主流语言，拥有成千上万的插件生态。

它的优势是“既简单又强大”：界面清晰，启动快，还能直接调试、预览、运行代码。Claude Code 生成的代码你都可以在 VS Code 里查看、修改、运行。

可以把 VS Code 理解成“写作软件”，只是写的不是文章而是程序。Claude Code 是帮你写稿的 AI，而 VS Code 是你用来编辑稿子的 Word。

如下图， 这个是 VS Code 的默认打开的一个界面

其实就是跟普通的软件一样， 只不过，菜单按钮可能会稍微多一些

![](img/9f0590869d56353e5506e9d548781322.png)

3.3MiniMax2.7是什么

MiniMax 2.7 就是一个编程很强的模型，他的母公司是稀宇科技（这个名字你可能没听过，比起智谱/月之暗面等公司）。

你可以理解 Claude Code 是工具，如果需要工具干活，那么就需要一个大脑，这个大脑就是模型，我们这次讲的就是 MiniMax 2.7 的模型

对于国内用户来说，它最大的优势是：能稳定使用，不受国外网络限制。Claude Code 可以切换“驱动模型”，用MiniMax2.7代替 Claude 官方模型，依然保持强大的编程能力。

简单理解：Claude Code 是外壳，MiniMax2.7是大脑。Claude 断网时，你可以让它用国产大脑继续思考。

![](img/90d6a699cee7eac3ea5bf64998b9c6c0.png)

其实还有 GLM5，属于智谱公司推出的模型

还有月之暗面公司推出的 kimi for code 专门用于编程的模型

目前就这三家适配 Claude Code 上体验和质量还算不错的

3.4 终端（Terminal）是什么

终端是电脑里最基础的“命令窗口”，可以用文字和电脑对话。我们平时用鼠标点开软件，而程序员更习惯在终端里用命令来操作电脑，比如创建文件夹、安装程序、运行项目。终端的出现早于图形界面，是所有系统的“底层入口”。

在 Claude Code 的学习中，终端是你和 AI 打交道的舞台。因为 Claude Code 是一个命令行工具，它没有可视化界面，所以我们要在终端里输入命令来安装它、启动它、登录账号，甚至和它对话。你可以把终端理解为“AI 的语音通道”，你在这里发出指令，它就在这里响应。

每个系统都有自带的终端：macOS 的 Terminal、Windows 的 PowerShell 或 CMD。只要掌握一些最基础的命令，你就能操控整个编程世界。

**终端（Terminal）**

是一种命令行界面（Command Line Interface，简称 CLI），用于直接与操作系统交互。你可以通过输入命令来执行操作，比如：

创建文件夹

启动服务器

安装软件

查看系统信息

**它不像图形界面（G**UI）那样用鼠标点，而是用文字命令驱动系统。

**常见终端：**

| 系统 | 常见终端软件 |
| --- | --- |
| macOS | Terminal、iTerm2、Warp |
| Windows | PowerShell、Windows Terminal、CMD |
| Linux | GNOME Terminal、Konsole、Alacritty |

比如 windows 的 PowerShell 长下面这个样子

![](img/c2f2667f46f3cea04eb962caa800e465.png)

![](img/69d963f6b9facc313167aff566f5c266.png)

3.5 命令行（Command Line）是什么

命令行指的不是一个软件，而是一种“操作方式”——用文字告诉电脑你想做什么。比如在终端输入node -v是查看 Node.js 版本，cd project是进入某个文件夹。

命令行的核心优势是：**精准、快速、自动化**，特别适合开发环境下的批量操作。

Claude Code 的全部操作都建立在命令行之上。你安装、登录、调用 AI、运行项目，甚至创建文件，都要用命令行完成。虽然刚开始会觉得有些“原始”，但你会很快发现——只要掌握几个常用命令，命令行的世界比任何图形界面都自由高效。

简单来说，终端是房间，命令行是你在房间里说的话。我们学会这门“语言”，Claude Code 才能听懂你的请求。

3.6 GitHub 是什么

GitHub 是一个基于 Git 的“云端代码仓库平台”，也是全球最大的程序员社区。你可以把 Git 理解成“本地保存系统”，而 GitHub 是“放在云端的备份库”。

它不仅能帮你远程存储代码，还能让全世界的开发者协作、开源、复用。Claude Code 也能直接读取 GitHub 上的仓库内容，比如“分析一个开源项目结构”“帮我修改某个仓库里的文件”。

在使用 Claude code 的过程中，如果你想把自己的代码保存、共享或部署，GitHub 是最安全、最标准的选择。Git 是笔记本，GitHub 是云端保险箱。

具体内容可以看这个文档详细了解：https://docs.github.com/zh

![](img/c5557aa2e0ce29ea4c2e0c61353604a3.png)

Git + GitHub 的关系

可以这样理解：Git 是一套工具，而 GitHub 是一个网站。

Git 是你在电脑本地操作的“版本控制引擎”；GitHub 则是你把这些代码放到云端，和别人一起协作的“仓库平台”。Claude Code 可以在本地配合 Git，也可以与 GitHub 云端仓库交互。

它们就像 Word 和百度网盘的关系——一个负责编辑，一个负责存放；两者结合，才构成现代开发的完整工作流。

Github 的通俗理解

[https://www.douyin.com/video](https://www.douyin.com/video/7460057392470887699)/7460057392470887699

3.7 Node.js 是什么

Node.js 是一个让电脑能运行 JavaScript 代码的环境。过去，JavaScript 只能在浏览器中运行，而 Node.js 把它带到了电脑上，让 JavaScript 能做服务器、桌面程序、命令行工具等各种事情。

Claude Code 是一个使用 Node.js 构建的、需要在命令行中运行的开发工具。如果电脑里没有安装 Node.js，Claude Code 就像没装引擎的汽车——无法启动。

![](img/14976741161f885d3e2fc247dafce5c6.png)

💡Claude Code 的运行，就像一场合作演出：

**终端**

是舞台，**命令行**是你发出的指令；

**Node.js**

是引擎，提供 Claude Code 运行的动力；

**Claude Code**

是演员，负责理解你的需求、生成和修改代码；

**VS Code**

是后台工作室，用来查看、编辑和测试这些代码；

**Git / GitHub**

是记录员，保存每次修改，让项目可追溯、可协作；

MiniMax2.5/GLM 5 / Claude 模型

是大脑，让 Claude Code 具备智能思考与编程能力。

对于他们的关系，一句话总结

**你通**过终端发出命令 → Claude Code 借助 Node.js 运行 → 调用 AI 模型生成代码 → 在 VS Code 编辑 → 用 Git/GitHub 保存与协作

### 02.准备开发环境并安装 Claude Code

0.安装前必看：电脑基础知识

主要讲解电脑的一些基本常识，比如如何识别自己的电脑的 CPU 型号、以及一些电脑操作系统的基本常识。

**电脑分类**

目前，电脑基本上分为家用电脑和服务器。家用电脑就是我们经常用的笔记本、家里的台式机，就是自己个人使用的，包括在公司里面用的笔记本，这种都属于家用电脑。

服务器放在机房的机柜里，一般大家都看不到。如果是有运维去过机房的，应该都知道。服务器属于 24 小时工作，它需要的能耗和稳定性要求都极高。

**操作系统**

那我们有了电脑以后，只有硬件，我们需要安装微信，安装 QQ，安装浏览器。那在硬件和我们需要用的这些日常的应用软件中间会有一层应用。那这个应用比较复杂，我们通常叫做操作系统。

操作系统有很多分类，像日常我们用的最多的那就是 Windows 系统，还有 Mac 苹果系统，还有服务器上使用的，大部分都是 Linux 系统。

很简单，基本上你买的台式机、联想电脑，那基本都是 Windows 系统。如果你买的是苹果电脑，那就是 macOS 系统。如果你是装的虚拟机，比如 Ubuntu，以及服务器上安装的 SUSE 常见的都属于 Linux 系统。

**Linux 系统**

Linux 系统是一个很复杂的分支，它源于 UNIX 系统。UNIX 系统是商务收费的。那么 Linux 的作者 Linus Torvalds 为了开源精神，然后就写了 Linux 系统。那我们常说的 Linux，只是一个 Linux 内核，你可以理解成只是一个 SDK 工具。那为了服务上层的微信、QQ 这些软件，还需要做一些比如图形化界面这种的操作，那就有了 Ubuntu、CentOS、Red Hat Linux 等各类分支的 Linux 系统。

**CPU**

这里要说的一个重点就是在我们的电脑硬件里面会有一个大脑，那就是 CPU。CPU 属于硬件，那么 CPU 的发展过程中里面有两大指令类型，一类是 x86 类型，一类是 ARM 类型。那么软件我们上层使用的软件是需要跟操作系统，然后再跟底层的 CPU 去打交道的。因为 CPU 负责计算，负责指挥。所以 CPU 的指令类型也涉及到下载软件的类型。

经常我们使用的 Intel 处理器都是属于 x86 类型的指令 CPU。这类 CPU 我们下载的安装包基本都是 x86_64 类型的软件安装包。

那比如像现在的 mac OS 系统使用的 M 芯片，这就属于 ARM 指令系列以及鸿蒙操作系统，使用的都是 ARM 的芯片。所以我们需要下载 ARM 的安装包。

怎么确定自己的 CPU 类型是什么？

💡辨别自己电脑的 CPU 属于 ARM 芯片，还是 X86_64 芯片是很重要的，会涉及到下载安装包的选择。

当然，这里如果你没有看懂，也不需要担心。后面如果需要选择有类型的安装包，回到这一小节，再确定自己的电脑 CPU 芯片的型号也可以。

**Windows 电脑**

右键我的电脑选择属性就可以看到电脑的基本信息。

![](img/1a7b144bd1dda1198070a0e96e4e7c32.png)

看到如下的界面有处理器名称

比如我的这里是在 Mac M 芯片装的虚拟机，所以它属于 ARM 类型处理器。

如果大家看到的是 intel 这样的字母，那就属于 x86_64 的机器。

![](img/e3f868ca4bbc1d050ec89f824a80be53.png)

**Mac 电脑**

Mac 就点击左上角苹果的图标，然后会看到一个“关于本地”或者“About this Mac”字样，点击选择。

![](img/89fc7f2db81b35dc14126fe270dba3e7.png)

然后会看到芯片那一栏，如果显示的都是 M4 类似的，那就属于 ARM 芯片。

如果看到的是 intel 字母的字样，那就属于 X86_64 型号。

![](img/40c65c9438c4af88f5273109da072003.png)

![](img/035568fb2e7d8210c8ff3af33ed300d2.png)

1.安装开发环境

**在开始使**用** Claude **Cod**e 之前，我们需要搭建**好开发环境，包括开发工具，基础环境 git，以及Claude Code的配置

1.1 安装 Git 环境

Git 是一个**代码版本管理系统**，可以记录你对代码的每一次修改，就像“时间机器”。你写的每一段代码都能被追溯、回退或对比，不管团队协作还是个人项目，都能防止“手滑改崩”或“忘了昨天改了啥”。

1.1.1 Windows 版本

💡Q：为什么需要安装 Git

A:

1.  **Claude Code 在所有系统上****都需要识别、**管理、保存代码项目的版本记录，而这项能力是 Git 提供的，Windows 系统默认是没有 Git的，必须手动安装，否则 Claude Code 无法识别项目的版本信息。

1.  后面代码的存档管理，也是需要**Git**，开发基础环境必备，有了**Git**，Claude Code 才能安全、完整地理解并管理你的项目。

PS：注意，**装 Git 的时候按默认路径装，不**要自己改安装目录，一旦改了，后面就会报错

**零：视频版教程**

**视频学习链接：**

安装 Git 环境-Windows 版本

视频位置如下方截图

![](img/22db047f953e9df5be11d6c07a0f1dd2.png)

**第一步：下载**

直接点击官网下载地址即可：https://git-scm.com/

然后点击网页中间有个红色的按钮「Install for windows」

![](img/b6098a87e48db7676be5307b7c2490d7.png)

⚠️注意：虽然软件只有 64 兆不到，但官网下载速度很慢，需要等待。

当然也可以去网盘下载也可以

夸克网盘链接：https://pan.quark.cn/s/7f9f6e363612提取码：FVCm

百度网盘链接：[h](https://pan.baidu.com/s/1cRFbfyA-D1wdJX-KMvirdQ?pwd=xg8w#list/path=%2F)ttps://pan.baidu.com/s/1cRFbfyA-D1wdJX-KMvirdQ?pwd=xg8w提取码： xg8w

就会跳转到下面的页面，点击「Click here to download」就可以开始下载了

![](img/5497ead46e127cda7a82201573f28666.png)

点开浏览器的下载按钮，就可以看到开始下载了

![](img/2dc189a4628917710ae010204f585624.png)

**第二步：安装**

直接打开，下一步

![](img/d88b7d13d72f8a32932c32f5d0684cf7.png)

**选择安装目录**

💡这里的安装目录强烈建议使用默认

后面涉及到环境变量识别的问题，还需要单独设置。

并且 git 不占用 c 盘多大空间

![](img/d985e1b54428bf3771f4fc1049e61781.png)

保持默认

![](img/3485dc4612176d927a9d965816dcb3e4.png)

继续

![](img/37ddd5f6cbffa44b75bb68a5905ba727.png)

保持默认

![](img/d242bfe3b3568732771d1b8aa8af5d15.png)

下一步

![](img/e77d27a2a53d45f590d0e7e5cc7454f9.png)

下一步

![](img/ddf0d4a9a0436d856b8a786c432e84c0.png)

下一步

![](img/2b7b06314e7366ac1192998b15d7bf1e.png)

下一步

![](img/ac3b7ebf80e329f1585409fc5fabcf75.png)

下一步

![](img/6e1e20016dd5fbd49729bfd3fec393a4.png)

下一步

![](img/b1fe56af8c3d5796c52814bd48f81692.png)

下一步

![](img/c8369fbf563eb84e9cea9824ca8ee127.png)

下一步

![](img/32f17aaba7de35e29694adc7b53542cb.png)

安装

![](img/bec8c3b9b7fda95ff160a70abb51b2b7.png)

等待完成安装

![](img/e7958ec678ea1ecad543191cbbb62ab5.png)

完成就行

![](img/8892c18892c633c0b63503b66e4afb16.png)

然后就会弹出如下界面，就表示已经安装成功了。

**注**意：因为电脑型号不一样，所以显示的紫色字体也不一样，依据自己的电脑型号来，如果不确定可以截图问 AI 是否安装成功

下图是 ARM 处理器，显示 CLANGARM64 ～

![](img/331aba6e53cf624d086bf52b330aa9b3.png)

如果电脑是 Intel 或者 AMD 处理器，紫色字体会显示 MINGW64 ～

![](img/70748a7ba45e8de11d9c8eede2a672f5.png)

![](img/21a6123193475997a7a760cd5016d1bb.png)

1.1.2 Mac 版本

这里看到的都是 brew 的安装，因为安装 brew 完后， Git 就安装完成了，一举多得

💡为什么需要安装 brew / git

1.  mac 的很多软件都可以通过 brew 来安装

1.  安装 brew 的同时，git 默认就会安转，不用额外再安装

**第零步：视频版教程**

**视频学习链接：**

安装 Git 环境（Mac 版本）

视频位置如下方截图

![](img/cb08df4aa93c2eb4a21ed7e28586785e.png)

**第一步：打开终端**

通过 Launchpad（启动台） 或者 spotlight（聚焦搜索）找到「终端」这个软件

通过启动台找到「终端」

![](img/97482bcb4d07fdf36885f7ed8668d4a3.png)

打开后，默认的终端如下：

黑色的一个竖线那个地方就是输入命令的地方。

![](img/c3fdbcf9b046b4965e730ad19ba78a90.png)

好，我们进入下一步，开始安装 brew

如果对 brew 不熟悉的话可以问豆包、问 GPT，了解 brew 的作用

**第二步：开始安装 brew**

参考链接：https://gitee.com/iamzhihuix/HomebrewCN

把下面的整条命令，复制拷贝到终端，执行

Shell

```
/bin/zsh -c &quot;$(curl -fsSL https://gitee.com/happyaicoder/HomebrewCN/raw/master/Homebrew.sh)&quot;
```

执行如下图。

**有些地方如果显示 Password：形式的，**输入你电脑的登录密码就可以，注意不要输错

注意：输入密码的时候，密码本身在终端是不显示的，直接输入完回车即可

![](img/df8c625f0f7454fdfcbaad53af9ba719.png)

选择 1 后，会出现这个内容，需要继续输入电脑密码

![](img/62d126513519200f72aad6737ba2d630.png)

**输入 Y**

![](img/5c5955dc59fb16d2807d96fc8aa5c4fb.png)

**直接回车**

![](img/e8566cbe916daff7200caf4454972df5.png)

**输入电脑密码**

![](img/f7715843c77d7f4b989b49abfcaeea3f.png)

**选择 2**

![](img/b8d4dd4818bfaf4cb6c6d587b21bed45.png)

**到这里就安装成功了**

![](img/e137fe304013c2acf971a0a56375637c.png)

**按照提示执行。**

需要执行的命令每个人的都不一样，需要从终端界面复制

终端界面会有显示执行什么命令，就像下图中框出来的部分就是需要复制到终端的部分

![](img/8766f5cda88d2dcabc05f00f4274baed.png)

![](img/9e1ca8e7e81aa03e6158810c99e8af5f.png)

**第三步：确认是否安装成功**

验证 brew 是否安装成功

Shell

```
brew -v
```

![](img/50befa777bff17222e38a4c6f314f799.png)

再校验 git 是否安装成功

Shell

```
git --version
```

![](img/8df30bbef7cdd99ab3f98d38a32e43e1.png)

![](img/958ed644711b0fef0cf0a07ad3c07b42.png)

1.2 安装 Node.JS 环境

💡Q：为什么需要安装 Node.JS

A:

前端复杂项目开发（网页/H5）等在浏览器可以打开的网页形式的开发环境依赖于 Node.JS，比如需要用到 ReactJS、nextjs 框架的时候

**注意：NodeJS 需要的版本是 18+，也就是版本号大于** 18 的都可以， 比如 20、 22。

1.2.1 Windows 版本

**第零步：视频版教程**

**视频学习链接：**

安装 Node.JS 环境（Windows 版本）

视频位置见截图

![](img/87a745734e3498fac046bcaf40aef41e.png)

**第一步：下载安装包**

官网地址：https://nodejs.org/

1、直接下载

![](img/fc68f7f70a01d63a86703ce00e05b808.png)

选择安装程序

![](img/a43a0416a265ce52fb2cbc1b2e506c5c.png)

下载后的大概差不多如下：

![](img/daa3c1e7d692bf5ef8a6777788f85c31.png)

也可以直接下载这里提供好的

你现在下载的版本可能会跟我这里的不一样，版本会一直更新的。

[

![](img/1d4d08197a829073653d1f8b55ab4839.png)

node-v24.14.0-x64.msi](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/DlPbbuChmonpzKxc5CNcURslnXJ?response-content-disposition=attachment%3B%20filename%3D%22node-v24.14.0-x64.msi%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260526%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260526T134056Z&x-oss-expires=86400&x-oss-signature=2cd4ed55a9c3517d802c294f4c5f221e44690f9a00856f3e8608c8bd1dc8faf1&x-oss-signature-version=OSS4-HMAC-SHA256)

直接双击打开安装就可以

**第二步：安装**

2、直接打开

下一步

![](img/b587591801fe9bae0bcb5a938aa454ca.png)

**勾选同意**

![](img/b26fb020cf21b638803da4983faacd0b.png)

**修改安装目录**

![](img/f19819cce0a604c8cddd564a0461360c.png)

**下一步**

![](img/5fcbae2352cd15f3e6e5909074dae67d.png)

**下一步**

![](img/2a27e91cb970b484626cd305954ef67a.png)

**安装**

![](img/f072cc78ff0fee373362b39a088d8a42.png)

如果弹出来是否对设备更改的通知，点击「是」就可以了

![](img/1985ffc83052f18e46b28bb8f44a3037.png)

**等待完成安装**

![](img/403c9865e81b957e45c5296367c6d78d.png)

**完成就可以**

![](img/e901933c58c49b7a04891f6ffa8bd24c.png)

**第三步：验证**

3、打开 PowerShell

打开命令提示符

然后输入下面的命令

Shell

```
node -v
```

![](img/56a456fc1ee0e853c8041a21a510c033.png)

Shell

```
npm -v
```

![](img/5da95ecb60076685de56b3e1ddb43198.png)

看到下面的输出正常的版本好，就表示可以用了。

截图安装的时间，2025-06-13 号，你可能的版本号比这个大，或者版本好可能跟我的不太一样，关系不大，能出来版本好就表示可以用的。

如果有下面的报错

![](img/e6a8fd53f61d049872bca1278cb084ed.png)

可以执行下面的语句

Shell

```
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

选择 Y 就行

![](img/7b5ebd7059a8371a91ff2ea799956edc.png)

再次执行npm -v的时候就可以了

Plain Text

```
npm -v
```

![](img/2da6a8ac4b13239f49185f4e9d5c2a40.png)

1.2.2 Mac 版本

**第零步：视频版教程**

**视频学习链接**

安装 Node.JS 环境（Mac 版本）

视频位置如下方截图

![](img/27f772dc06af288bac56607cdbdc45f6.png)

**第一步：安装**

教程地址：https://gitee.com/iamzhihuix/nvm-install-cn

直接复制下面的安装命令

注意，不要自己手敲，一定要复制

Markdown

```
/bin/bash -c &quot;$(curl -fsSL https://gitee.com/iamzhihuix/nvm-install-cn/raw/main/install.sh)&quot;
```

然后打开苹果的「启动台」，搜索一个叫「终端」的应用

![](img/df9fd2af68a5a740b6db409af9fe6d12.png)

![](img/fdba2bb3d4bdfd4b163dca7234ca3e91.png)

等待下载完成

![](img/7e7a09c65e676020fb98419f61c7f5ea.png)

看到下面的提示就表示已经安装成功了

![](img/8c032ca030fca4712813c68ffa8820c1.png)

**第二步：验证**

分别执行如下命令

Markdown

```
node -v
```text
npm -v
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

Plain Text

```
powershell
```

**以管理员身份运行**

![](img/807b00b02db66fdaed2de8de5dfff260.png)

执行下面的命令

Shell

```
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned
```

![](img/62ad2745ca5cfcd087c41ad0b372aa9b.png)

**注意：有些电脑会弹出执行策略更改这个选项，需要按照下方步**骤操作一下，不然后面的步骤是进行不下去的

解决办法：

输入 Y 然后回车后，就到下一词输入命令行的地方，就表示成功了。

![](img/ff956ea81722b9a3462dc1350104cfb6.png)

验证：

然后接着复制命令，拷贝到 PowerShell 上，回车执行。

Shell

```
Get-ExecutionPolicy -List
```

看到「CurrentUser」的选项是「RemoteSigned」就行

其他选项的值无所谓

![](img/33f68e59dcd0939825535d234bcd2484.png)

执行安装的命令

Markdown

```
npm install -g @anthropic-ai/claude-code  --registry=https://registry.npmmirror.com
```

![](img/defdd96ee1a319f88252d4222acd4176.png)

如果出现如下的几行字，是 notic 警告信息

并不是 Claude Code 安装有问题

![](img/42172b1230c4f89d1794b53d6c8e17f3.png)

验证

Markdown

```
claude -v
```

打印版本就表示已经安装成功了

![](img/d89d697d96d8fbc970564fdd9cd7100b.png)

![](img/d48aca86f64b333f536480220181b9bc.png)

2.2 Mac 版本安装

**视频学习链接：**

安装 Claude code（Mac 版本）

视频位置如下方截图

![](img/f07aac0646ed55be356ce63fb13979e9.png)

**第一步：安装**

复制下面的命令，直接粘贴到终端

Markdown

```
npm install -g @anthropic-ai/claude-code  --registry=https://registry.npmmirror.com
```

终端显示的可能跟我的不一样，只要没有红色的字样就可以

一般都是显示其他信息，如果不懂的可以截图发给 AI 让他给你解释

![](img/4e987cf2c4d654d65bb5f8e7c0e07772.png)

**第二步：验证是否安装成功**

Shell

```
claude -v
```

如下方截图（苹果电脑）：

![](img/521365db7674089ddef072a681f0fbec.png)

![](img/54d6ad3e853c3872d430a9899ee019e0.png)

2.3 安装时可能出现的问题

问题一：终端出现报错，如何把报错的内容直接复制出来

解决办法：终端里面的复制粘贴，就是在选中报错内容之后，点鼠标右键，即可复制

问题二：执行 npm -v 或者 claude 命令时候报错

windows 如果有下面的错误

执行命令：

![](img/c68af2242527f958f6109c84f0eb27c7.png)

执行命令：Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser

Plain Text

```
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

![](img/f2cbbed271b8c647e21a4a9f6689f01d.png)

问题三：出现 git 相关字样报错

![](img/953801c9216933b05ba9747aa9c8045c.png)

解决办法：

1、重新安装 git，使用默认路径

2、设置CLAUDE_CODE_GIT_BASH_PATH变量的值，值就是 git 的安装路径（windows 环境变量设置的地方）

问题四：Mac 电脑出现红色的报错

Plain Text

```
sudo npm install -g @anthropic-ai/claude-code
```

💡

**⚠️注意**

：如果安装的时候报以下错误（图片见下方），说明你需要用到管理员权限，我们直接添加一个 sudo，再次执行

复制这个到终端页面即可：sudo npm install -g @anthropic-ai/claude-code

**然后在终端输入**电脑开机密码（注意这里输入的开机密码，在终端中不会显示，所以直接输入即可，如开机密码是 1234，那就在这个钥匙🔑标志的后面输入 1234，然后按回车键即可）

图片如下：

![](img/1b4c94be5f6cf360336e0a2b4492445c.png)

![](img/673091eefc6e2f8273f617cd1a90ebd5.png)

**⚠️注意：可能出现错误的地方：**

如果我们**本地没有配置全局代理**，可能会出现下面这种：Unable to connect to Anthrpic services，please check your internet connection and network setting。 等类似的字样的错误提醒。

如果我们后面要使用**智谱等国内的模型**驱动 cc，这个错误可以先**忽略**

如果我们是**官网原版****的 Cl**aude Code，请查看下面的解决方案。

![](img/158e76a61dbe0b984e4a3760138d6c0a.png)

**网络错误解决方案**

出现上述网络错误，我们可以通过修改 Claude Code 配置文件解决。

配置文件的路径是

Mac 是： /Users/[电脑用户名]/。claude/settings.json

Windows 是： C:\Users[电脑用户名]\。claude\settings.json

比如 Mac 中我的用户名是 limo，那么配置文件则是 /Users/limo/。claude/settings.json

如果不存在的话则新建同名的配置文件

：

![](img/e5d36a3d56a9b80d50ff451357978e5a.png)

我们使用直接双击打开 settings.json 进行编辑，在该配置文件中新增我们下面的代理信息：

注意！！ 下面的端口要根据自己的代理端口决定，比如你使用的代理软件的 http 端口为 7890，端口则设置为 7890，如果是 7897 则要改为 7897

JSON

```
{&quot;env&quot;: {
    &quot;HTTP_PROXY&quot;: &quot;http://127.0.0.1:7890&quot;,
    &quot;HTTPS_PROXY&quot;: &quot;http://127.0.0.1:7890&quot;
}}
```

![](img/d2d11ac419b940cc308cb24a75331eb0.png)

3.**使用国产模型**MiniMax2.7**驱动**Claude Code

Claude Code 我们可以使用两种方式**，第一种是官方版，第**二种是使用国内模型如MiniMax2.7驱动 Claude Code。

使用官方版需要我们在[Claude.ai](http://Claude.ai)进行**订阅，目前 Claude 官方有 Pr**o、5x MAX、20x MAX 三种套餐形式，对应的价格分别为 20 刀、100 刀、200 刀，另外因为 Claude 一直对国内进行封锁，所以想使用 Claude 官方版本需要突破网络和海外信用卡支付两个关卡，门槛较高。

本次航海，**我们主要推荐大家使用国内的模型**MiniMax2.7**驱动 Claude Code**

💡来一段科普解释，大家先听个响。也是下面我们经常会说到的几个词

1、**cc-switch 是一个用来快速切换 Claude Cod**e 工具中不同模型 API 配置的工具。

2、**MiniMax2.7**是模型 ，由MiniMax公司训练而来

3、**Claude Code****是个编程工具**，平常大家说的官方使用，或者封号，需要网络环境，其实是用的 Claude 模型（公司是 Anthropic，不仅出模型 Claude 模型，还出编程工具 Claude Code）

在后面的实操中会让大家看到他们之间的关系

3.1 视频版教程

cc-switch 在 mac 电脑上需要安全设置，所以以 mac 为例

其他设置 windows 是一模一样的

**视频学习链接：**

[安装 cc-switch](https://shengcaiyoushu01.feishu.cn/docx/Qr2NdoezHo87gIxcMy9c1vs6nIf)

视频位置如下方截图

![](img/e3b72ed90198ff52e006f0c1d8a58d64.png)

3.2 如何配置MiniMax2.7（使用 cc-switch 来配置）

3.2.0 学习资料

套餐购买地址：

https://platform.minimaxi.com/subscribe/coding-plan?code=G4YsAHUVMT&source=link

使用这个链接可以打 9 折进行购买

这个链接是MiniMax2.7**注册账号和充值**的地方。因为MiniMax2.7 模型是 MiniMax 公司提供的服务，通常是付费使用的。这个链接指向MiniMax2.7的官网注册或邀请页面，你需要在这里注册账号，并购买相应的 Token 额度或会员套餐，才能有资格使用该模型。

![](img/bfe77697c28bacc0446066e6921e741e.png)

API-KEY 设置地址：https://platform.minimaxi.com/user-center/basic-information/interface-key

这是链接是获取MiniMax Token Plan Key的地方。当你有了账号和余**额后，不能直接**把账号密码填给软件（cc-switch）。你需要在这个页面生成一个API Key（一串很长的字符密钥）。这个 Key 就像是专门给软件用的“专用密码”，把它填入你的软件配置中，软件就有权限代表你去调用 AI 模型了。

💡这里一定要注意是使用的“Token Plan Key”的地方，不是上面的普通的 API Key

不要选错了。

![](img/13ac5c7178ea47fd70d0c42bb35f403b.png)

MiniMax2.7官方配置文档参考：https://platform.minimaxi.com/docs/coding-plan/claude-code

**这个链接是**MiniMax2.7的官方操作说明书。它会详细告诉你，在你的软件（这里指的是 cc-switch）里，具体的参数应该怎么填（比如 API 地址填什么、模型名称填什么等）。大家可以先点击链接自行学习。

![](img/577820c66751610efac0ed43f5dff4ca.png)

3.2.1 购买模型套餐

MiniMax2.7是MiniMax（一家中国的 AI 模型公司）提供的商用大语言模型，使用这种模型时：模型的运行需要计算资源（GPU、显存等），智谱提供这些算力服务，需要收费，所以用户要先“购买套餐”，获得调用额度

**（1）点击链接打开大模型官网**

https://platform.minimaxi.com/subscribe/coding-plan?code=G4YsAHUVMT&source=link

**如果是第一次**访问，是需要登录的**，**直接使**用手机号注册**就可以**，登录后即可看到这个页面**

点击特惠套餐后直接跳到下一页付费套餐界面

****如果你注册过大模型官网，点**击上方链接，就会出现下面类似的套餐选择页面

**（2）选择自己合适的套餐就可以**

**对于新手**观望期/想尝试的 Claude Code 功能的：建议选择29**/月的先上手**，推荐使用 49 的套餐**

对于确认后期大量使用/需要上线产品功能的：建议选择119/月

如果对生成速度有要求（3 倍生成速度），可以选择对应量套餐的极速版

![](img/e29d57fde047c0b3c2c08ee6243ddc13.png)

💡注意：默认是按月会继续给你订阅，如果你不想下个月继续使用，几个在支付宝里取消订阅，取消后，这个月还是可以使用的

3.2.2 获取 API KEY

API Key 是一串独一无二的“身份凭证”，是工具自动帮你登录智谱系统的“钥匙”，系统用它来识别“你是谁、你买了什么套餐、你有多少额度”。每次你调用MiniMax模型（比如让它写代码、回答问题），你的电脑或工具（如 cc-switch）都会把这个 Key 一起发送给服务器。

打开https://platform.minimaxi.com/subscribe/coding-plan?code=G4YsAHUVMT&source=link这个地址，就可以看到如下界面

![](img/7a525b7f14a9edf4705bb09d09e6183e.png)

**复制 API key**

我这里是已经配置过的，并且看到，配置过后，会有一个「复制」的按钮

💡切记保存好 Key

避免泄露，导致一些不必要的安全问题

![](img/ce0ea80e3e71ace7f53ef1adb68dfb58.png)

3.2.3 用 cc-swith 来配置API Key

**AI 模型本身没有聊天窗口，必须配合 cc-switch 这种**软件才能填入 API Key 进行对话。

这款软件的好处是界面直观，能让你在 ChatGPT、MiniMax2.7等多种模型之间一键切换。

这次我们使用 cc-swith 来配置 api-key，使用MiniMax2.7的模型，对新手上手程度更友好。

注意事项：如果你已经是有官方的 Claude 的账号，那么就不需要使用 CC - Switch，直接进入 Claude Code 终端，使用**/login （这是在Claude Code对话框中使用的）**登录就可以。

第一步：下载 cc-switch

这里我们使用一个简单的模型切换工具，cc-switch，这是 github 的开源项目，可以帮助我们更快地切换不同的模型驱动 Claude Code，原地址是：https://github.com/farion1231/cc-switch

下面是 windows 版本的和 Mac 版的软件，开箱即用。

Windows 版本下载这个：

[

![](img/6fd875464dc7f048121278d2bc55d619.png)

CC-Switch-v3.12.3-Windows.msi](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/UxmTbcWTQoR19FxZMCkcw0HJndh?response-content-disposition=attachment%3B%20filename%3D%22CC-Switch-v3.12.3-Windows.msi%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260526%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260526T134056Z&x-oss-expires=86400&x-oss-signature=8cd2adefaa862a13e11240b77379c6f25908630517e99f2c6df940580afab7f9&x-oss-signature-version=OSS4-HMAC-SHA256)

Mac 版本下载这个：

[

![](img/81eada940d20530688f7ebd8c0d30e16.png)

CC-Switch-v3.12.3-macOS.dmg](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/LxWqb0wRJotGMLxJ0hhcULDGnwc?response-content-disposition=attachment%3B%20filename%3D%22CC-Switch-v3.12.3-macOS.dmg%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260526%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260526T134056Z&x-oss-expires=86400&x-oss-signature=a1c74d9cce5f9b55c99749f9253a762226e5c3631de70df625f56d5f5a55203b&x-oss-signature-version=OSS4-HMAC-SHA256)

也可以直接在这里下载：https://github.com/farion1231/cc-switch/releases（网络慢的话下载上面直接提供的安装包）

如果访问有超时等问题，可以到国内 gitee 镜像仓库下载

https://gitee.com/iamzhihuix/cc-switch-mirror

如果是 windows 安装有如下类似错误，可以下载下面的免安装版本：

![](img/0486a89fe7cd81c7a5f3422a0446e2c8.png)

这里是免安装下载的安装包

[

![](img/b732ce0c8999a9ccd03b2832004bc6e6.png)

CC-Switch-v3.12.3-Windows-Portable.zip](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/XvYKbUJIco4LBVx04PecsX8Lnxb?response-content-disposition=attachment%3B%20filename%3D%22CC-Switch-v3.12.3-Windows-Portable.zip%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260526%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260526T134056Z&x-oss-expires=86400&x-oss-signature=66864f124e6eb666df9bfefe3be2c4754cc95fc6c4ed0aa303800e37c3b4edd5&x-oss-signature-version=OSS4-HMAC-SHA256)

1.  直接解压到一个目录，不要删除这个目录

1.  最好右键以管理员身份运行

1.  可以右键发送到桌面快捷方式

💡⚠️注意：CCswitch 版本更新比较频繁。

如果你从 GitHub 下载的版本跟当前文档里的版本不一致，那可以下载最新版本，大致安装流程都差不多；

也可以选择从这个文档的安装包下载。

这个链接点击后，windows 电脑会显示这个**页面，点击第一个 3**.12.3标题进去，然后把页面拉到最下面，看到这个 Assets，这个是软件下载的地方，选择下方的安装包即可

⚠️注意：如果网络下载慢是正常的

![](img/7a36835b1093ad6130d678ec21b724e8.png)

页面往下滑会看到 Assets

就会有下载安装包的地方

![](img/5e38d28e9be3a456d0f1f5bd266705fc.png)

如果是发现没有的包

可以点击页面上的有个「Show all 17 assets 」的链接，就可以看到所有的安装包了

![](img/3288646ee21b4675e6ca7c9cd0c9fc24.png)

**windows 安装包如下：**

![](img/31ad22052e804dd8ba2042dfcf4b6c55.png)

mac 的安装包如下，下载完后是个压缩包

安装方法，直接双击就会解压缩，然后拖拽到「应用程序」就可以

![](img/71568c4f319f74af45213702dcca6682.png)

**⚠**️注意：如果是 mac 打不开，有提示你「移除到垃圾篓」或者「文件损坏」之类的，看 3.3 常见问题解决

第二步：安装 cc-switch

windows 的安装步骤：

windows 如果遇见这种弹窗，选择「运行」按钮

![](img/7cdcc74008c5917f6dfc9c7b118a3b35.png)

就可以看到下面界面

![](img/9592203b1db3cbe29518a4978e113c43.png)

选择安装路径

![](img/816fa2b3d4a00bdcf98a20aac7089de6.png)

安装，等待完成即可

![](img/d02e232d804ff462ddfdc98531022397.png)

![](img/c44d1d896846e1200d763dd1fd65d01b.png)

![](img/dc7f40755d0973ad35ce640548a145c7.png)

3.2.4 配置MiniMax2.7

使用MiniMax2.7接口 等于真正让你的工具和模型开始对话，让指令能发给模型、拿到回应

安装完成 cc-switch，打开后如图所示：

第一次安装点进去是这个页面，点击右上角【添加供应商】即可

![](img/61f4c506e769bc2686bb4b0eaa036337.png)

把上面在 MiniMax 页面复制的 Coding Plan Key，粘贴到下面的框里就行

如果你已经不记得了在哪里，那么这里再给你看下截图

再给你个链接：https://platform.minimaxi.com/user-center/basic-information/interface-key

![](img/9ad89bdfd7edadd3655f7db18070fb01.png)

最后点击添加就行

![](img/3d2996f03da55d4bc3577ba3797bb1d8.png)

如下图，鼠标移上去配置的 MiniMax 模型，如果显示的是“使用中”，就表示配置成功

![](img/49217f4171766f65e5e33ffa06b7189c.png)

**如果**是，有如下界面，最后记得别忘记点击「启用」

![](img/0c944d4dae65681ecef6f97c8f4c920e.png)

3.3 安装 cc-swtich 常见问题

Q1：VSCode 插件如何使用自定义 API key

A：打开 CC-switch 的设置

![](img/06d832fa6d4c7bfd87cb90a0ec72c23b.png)

勾选上，保存就可以

![](img/65c040fc6f359645e9aefbbaace881c6.png)

如果配置了上面的还是不行，那么继续下面的配置

![](img/9fa4c4246ca25671414072c35608e59a.png)

![](img/ff328deaa15e4dc27fadd9df32e0e385.png)

**Q2：套餐余额不够**

A：冲套餐就行

![](img/9c288f80c202cedec415c4cc0538120f.png)

Q3：在 Mac 上安装 cc-switch 的安全问题

现在最新版本 3.12.4 没有这个问题了

苹果电脑上打开 cc-switch 会有如下提示：

![](img/41da9498a4beb1563a2230ada5bf99b0.png)

莫慌，打开设置，找到「隐私与安全性」的设置项

翻到最下面，选择「仍要打开」

![](img/0216dae1a418724d730b52dc0ce69e3a.png)

再弹出这个框，一定要选择「仍要打开」

不要选择错了，然后弹出输入密码的框

![](img/1e413958933719b4131f0b62688fdce4.png)

![](img/8065b99c502d0871573349893b558ac4.png)

下面就可以正常打开了

![](img/96aef687bb68bdae8d67793fe8977d38.png)

至此开发环境配置完毕。接下来，我们将了解 Claude code 的界面

Q4：终端启动还是连接官方接口，网络错误

推荐大家先看下视频教程

因为修改的配置文件和修改的配置都是一样

只不过由于系统的差异，会导致目录位置可能稍微不同

**mac 视频版教程：**

![](img/bd88f6eee3884d7876140367a6fc1198.png)

claudecode-network-mac-12月19日.mp4【在线播放】

![](img/8c179ad8041b4f53ecebd6e0cdc2d59e.png)

**windows 视频版教程：**

![](img/dc1cd91cdd64b2991b7ad29f933b992f.png)

claudecode-network-windows-12月19日.mp4【在线播放】

![](img/1f585f0ebf331f3c8a7879692893d318.png)

如果配置了 CC Switch 还出现下图的类似的错误。

![](img/91841b12358cb5ae64944d381f2f6802.png)

那么首先确认如果在 settings.json 配置了 KEY 和 URL

windows 的进入目录：C:\Users\用户名.claude

注意， 需要打开 Windows 的隐藏目录。

确保有下面的 settings.json 文件，使用记事本编辑打开

![](img/196f8f738763408583b3c83a7b00a121.png)

至少确认有ANTHROPIC_AUTH_TOKEN和ANTHROPIC_BASE_URL两个配置，否则去 cc-swith 重新配置

![](img/d8661ede7346d4afa09d638043b08521.png)

如果确认有了上面的配置以后， 还是不能进入 Claude 的终端， 那么需要修改.claude.json文件的配置。

文件位置：用户目录下，如下图所示

![](img/e2788365287c160d57fa0bc3276e0c15.png)

使用记事本编辑打开。

找下关键词hasCompletedOnboarding有没有这个配置

其他的配置不用管，不一样没关系

![](img/02e0c8fbf5ae0d00b31a0b0d2066b4d3.png)

如果没有搜到这个配置， 那么需要在这个 js**on 文**件里面添加这个配置， 注意后面的英文逗号。

所有都是英文字符，不能出现中文字符

这是一个完整的 JSON 配置文件，修改后仍需符合 JSON 语法。如果存在错误，该配置文件将无法生效。因此，请确保修改后的 JSON 仍然是合法的。可以去https://www.json.cn/类似的网站格式化下，可以验证 json 格式是否有问题

Plain Text

```
{// ... 其他配置
  &quot;hasCompletedOnboarding&quot;: true,
}
```

### 03.Claude code 界面导览与常见操作

1.  Claude code 如何启动

**新手建议选择**方式一，功能完整**

**方式二可选学**

**视频版教程**

**视频学习链接：**

Claude code 如何启动

视频位置如下方截图

![](img/a44b30836ae9b1042b1a333b7c50cb2a.png)

**1.1方式**一**：VSCode 终端使用 claude code**

1.1.1 打开**VSCode**，点击左上角文件夹图标，选择打开文件

![](img/6db2b27589ddf1a31e7b512cdb317567.png)

1.1.2 新建文件夹，打开项目，选择信任项目

![](img/45031a33ec65519245c098b4c6f7cdd4.png)

![](img/e89e8cd50d9ab7f4ecdd783e402db1de.png)

1.1.3 打开终端

打开 VSCode，点击右上角的类似的图标

![](img/b972f0715cc3ba3f6fea93800cb32548.png)

也就是中间这个

![](img/e03efacfa9c39f1359b606b5d319ba2c.png)

点开后，就可以看到下面的绿色的区域

默认就是打开的终端

![](img/9d8a1c68c952f4ab7930af40c2b22b9d.png)

下面就可以在终端里面使用 Claude Code 了

直接输入claude这个命令就可以

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
请帮我在终端配置一个别名，使得输入claude时自动执行claude --dangerously-skip-permissions命令
```

这样我们发现执行 claude 进入中断后左下角也有 YOLO 模式的提醒了

相信到这里，你已经安装上 Claude code，并且可以在 VS code 中运行啦，现在也对 Claude code 的基本内容有了简单了解，让我们在下一章开启实操学习吧

```
### 04.实战：用 Claude Code 制作早读神器

1.视频版教程

在小红书上面，有一类 AI 虚拟产品是销量很不错，如我们下面这个早读神器的案例，能够很好的用产品满足用户的需要，且这种 AI 产品有一定的技术门槛，会让你在虚拟产品赛道中拥有自己的优势；

当你能亲手做出这类产品时，你拥有的就不只是一项技能，而是一个可以在小红书上**直接变现的商品**

**注意：这一小节的案例为了让大家更好的上手掌握使用 Claude code 做产品的能力，对 Claude Code 有个简单的认识和了解，更多的编程案例可以参考 2025.1**2**月份的 Claude Code 航海**

[https://scys.com/course/detail/98](https://scys.com/course/detail/98)

**视频学习链接**

：[用 Claude Code 做一个早读神器](https://shengcaiyoushu01.feishu.cn/wiki/SEtTwjUuBiIcGkktTcFchFAEnvf)

视频位置如下图所示：

**推荐先看视频学习，然后结合图文内容去实操**

![](img/60f01e426a882e1b64c3caef00b45ee2.png)

2.产品需求挖掘

从小红书上可以发现这类教育小神器很多种类都可以做

![](img/650025e139b6d34bfa9a406089f5bf37.png)

这次我们找到的就是一种早读神器，具体是「早读动物园」

产品内容是：设定一个分贝值，如果学生们读书的声音达到分贝值以上，屏幕上就会出现很多的小动物，并且分贝值保持的话，动物就会越来越多。

可以在小红书上直接搜索「早读动物园」，就能发现很多类似的早读工具

**大家可以先根据我们的案例，一步步把这个产品做出来，再尝试开发自己感兴趣的其他早读工具**

![](img/8c3c336f18f56c01b8f638040a51a685.png)

3.项目实操步骤

**3.1 截图让 AI 工具给我们写好提示词**

在小红书上面找到对应产品的图片，直接截图

![](img/f56a05d0bb3f7f1be6bd4a7186468ac6.png)

找不到的船员们，也可以直接用下面的截图（2 张）

![](img/ec757a528b26e7016643ac5fe1d48521.png)

![](img/b5f9b24aebc5e41b5f34acac2fc85fda.png)

3.2 把截图给 AI 提要求

然后通过提示词，截图，到 AI 对话框里，说清楚我们的要求

这里如果你没有 GPT 或者 claude 的客户端，因为这些对网络有要求，可以使用国内的豆包来平替

可以直接使用下一步中的写好的提示词，直接发给 claude code/AI 工具对话框

Markdown

```text
这张图里面是什么内容，我想使用 html 复刻的话怎么弄了？先不写代码，我去 claude code 里面实现，请给我具体的提示词就行.
```

![](img/a7df0a45d4e76c4e90f91686d055ff7a.png)

![](img/1865644bbfd1b256c1a87d70886fa54d.png)

3.3 用 Claude code 开发

3.3.1 在 VS Code 中打开新目录

通过菜单栏打开目录

1.  打开 VS Code

1.  点击顶部菜单栏的**“文件” （File）**。

1.  选择**“打开文件夹...” (Open Folder...)**.

1.  在弹出的窗口中，浏览并选中你要打开的目录，点击“打开”。

![](img/b0d4771a33f8bdf19b1fc1e1dae5e215.png)

3.3.2 在 VS code 中启动 claude code

在 VS code 的终端里输入 claude，然后回车即可启动成功

Markdown

```
claude --dangerously-skip-permissions
```

![](img/ec611effff19524ce4b11df3aa6efe9a.png)

3.3.3 让 Claude code 帮你开发

在 vscode 里面新建[prd.md](http://prd.md)[文件，把前面](http://prd.md)问 AI 得到的提示词复制到prd.md文件中，最后在 claude code 对话框中@这个文件实现这个功能（如下图所示）

💡记得一定要保存文件。

windows 使用 Ctrl + s

mac 使用 Cmd + s

[问 AI 给](http://prd.md)**到的详细**提示词如下（需要放到prd.md文件中）

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

需要发给 Claude code 的提示词，让它开发

具体的开发过程，大家可以视频学习

Markdown

```
@prd.md 实现这个功能
```

![](img/030405969c5713d5ca3fc869ed047615.png)

![](img/4eb426c89d05e74da4541e3cf8cf8506.png)

3.3.4 成品展示

当 Claude code 开发完成后，我们在这个项目目录这里右键

然后选这个 Reveal in File Explorer，在浏览器里面打开 index.html 文件

我们选择用谷歌浏览器的方式打开它

![](img/0ef84ace7bc864893475e628d3ae8f3c.png)

然后选择需要允许麦克风访问

![](img/ee44d66feba313d81ff56551c48bc29e.png)

调整阈值后就可以进行声音测试

随便说内容，就可以看到页面上显示小动物

声音分贝一直保持就不停的有小动物显示

![](img/40a811e75a0c59eeddef140531c49b9a.png)

**这个产品主要的功能如下：**

1.  调整网页收到声音的分贝的阈值。

1.  超过声音的分贝阈值以后，如果声音一直都有，界面上的小动物也会越来越多。

1.  这个小产品达到的功能， 就是让学生们早上大声朗读课文，不会显得很枯燥

4.总结

本次做的是一个早读神器，主要实操重点是：

1.  从小红书挖掘需求

1.  Claude Code 做基本的网页的案例，使用的技术是：HTML/CSS/JavaScript

1.  掌握基本的 Claude Code 提示词沟通技巧，不要畏惧终端编程工具

💡本期的航海内容涉及比较多，所以 Claude Code 的案例就放了一个

大家感兴趣的可以看上一期的 Claude Code 航海

案例比较多、丰富

## 二、Claude Skills 的入门和实战

### 01. 入门：全面认识 Claude Skills

0.本章概要

💡本章会带你正式进入 Claude Skills 的入门与实战阶段，重点不是停留在“知道 Skills 是什么”，而是让你真正学会：怎么安装、怎么挑选、怎么安全使用，以及怎么亲手做出第一个可落地的 Skill。

首先，你会建立一个关键认知：Skills 本质上就是给 Claude 用的 SOP 手册。它的作用不是让 AI“更聪明”，而是让 AI 在特定任务上输出得更稳定、更专业、更符合你的工作标准。

接着，你会学习 Skills 的实际安装与管理方法，包括如何一键把 GitHub 上的 Skill 安装到 Claude Code 项目中，以及安装时必须注意的几个原则。

在此基础上，本章还会带你进入**两个实战场景**

第一个是**自媒体的自动发布 Skills**。这里有**公众号和小红书**两个场景，这里只需要任意选择一个实战案例完成即可，如果是新手推荐公众号全自动 skills 搭建，小红书难度较大；

第二个是**AI 视频制作 skills**。在进阶篇也有两个场景，同样只需要选择一个进阶案例**完成即可，不需要全部做完，新手**推荐第一个小说改编漫剧剧本 skills，第二个难度较大；

学完这一章，你真正收获的，不只是装好几个 Skill，而是掌握一种新的工作方式：把自己的经验、流程和标准，沉淀成 Claude 能反复调用的自动化能力。

💡

**本章航线图**

完成本章节的学习和实操，即可完成航线图的第一阶段。

第二阶段：Claude Skills 的入门和实战（约 7 天）

完成 Claude Skills 安装部署（约 1 天）

**完成** Claude Skills 的一个实战案例（约 3 天）

**完成** Claude Skills 的一个进阶案例（约 3 天）

1.Skills 是什么

💡⚠️注**意：**第二章的 skills 都是基于 Claude code 去安装和运行的，如果你现在还没有 Claude code，需要回到第一章安装部署 Claude code 后再去学习第二章 skills

skills 是 Claude Code 在 2.0.20 版本新加入的功能，与其说是 Claude Code 拥有，不如说是 Claude 体系拥有。因为 Anthropic 家的产品都支持，比如 Claude Desktop 也可以。

到现在更是成为了一个标准，各个厂商都已经支持 Skills 了，有点当年 MCP 的趋势。

一句话：Skills 就是给 Claude 看的 SOP 手册。

怎么说这句话了，下面都是文字解释来诠释这句话。大家看的懂就看，看不懂就当小说看完

后面大量实战，用起来就会慢慢知道 skills 是个什么东西了

SOP（标准操作流程）你肯定不陌生。麦当劳为什么全球几万家店，每家做出来的巨无霸味道都差不多？不是因为每个店都有大厨，而是因为有一套极其详细的 SOP——肉饼煎几秒、酱挤多少克、生菜放几片，全部写死了。任何一个新员工，照着 SOP 做，出品就能达标。

Skills 对 Claude 来说，就是这套 SOP。

没有 Skills 的 Claude，就像一个聪明但没经过培训的新员工。你说"帮我做份年度汇报 PPT"，他凭自己的理解去做，做出来能用，但可能字号不统一、配色不协调、排版乱七八糟——因为没人告诉他"应该怎么做"。

有了 Skills，就等于你给他发了一本《PPT 制作标准操作手册》——用什么字体、标题多大、每页放多少内容、图表怎么配色，全写得清清楚楚。他按手册执行，出品就稳定、专业了。

技术上看，Skills 的本质是Markdown 格式的指令文档，就像一份数字化的 SOP，里面打包了三样东西：

• **操作步骤**：先做什么、再做什么，按什么顺序来

• **工具配置**：该调用哪些工具、怎么调用

• **质量标准**：做成什么样算合格，有哪些注意事项

跟现实中的 SOP 一模一样的逻辑——把专家的经验变成可执行的标准流程，让执行者不需要自己摸索，照着做就行。

**Skills 的价值**

理解了"Skills = SOP"，它的价值就很好懂了。

想想你去过的连锁品牌——海底捞的服务、星巴克的咖啡、胖东来的陈列——它们的核心竞争力不是"碰巧招到了好员工"，而是把最佳实践写成了 SOP，让每个人都能稳定输出高水平。

**Skill**s 做的就是同一件事，核心价值三个字：稳、准、专。

💡•

**稳：每次都有保障，不靠运气。**没有 SOP 的餐厅，菜好不好吃全看厨师今天状态。没有 Skills 的 Claude 也一样，同样的任务，有时候做得不错，有时候就差点意思。有了 Skills，就像有了标准化流程，每次输出质量都在线。

• **准：不用反复交代，一句话搞定。**以前你可能要写一大段提示词："用这个字体、标题要加粗、表格要有边框、最后加个目录……"现在这些全写在 Skill 里了，你只需要说"帮我做个 PPT"，Claude 就知道该按什么标准来。就像你不需要每次都跟麦当劳员工说"肉饼要煎熟、要放两片生菜"——SOP 里都有。

• **专：装的是反复验证过的最佳实践。**Anthropic 官方提供的 Skills，都是经过大量测试和打磨的。比如做 Word 文档的 Skill，里面写着怎么处理页眉页脚、怎么生成目录、怎么控制段落间距——这些都是踩了很多坑之后总结出来的经验。你自己摸索可能要半天，用 Skill 一步到位。

更关键的是：你可以写自己的 SOP

这才是 Skills 最强大的地方。

官方的 Skills 是"通用 SOP"，适用于大多数场景。但每个人、每个公司都有自己的工作方式。比如：

• 你们公司写周报有固定模板——你可以写一个"周报 Skill"

• 你做前端项目有一套命名规范——你可以写一个"代码规范 Skill"

• 你写公众号文章有特定的排版风格——你可以写一个"排版 Skill"

写好之后，以后每次只要说一句话，Claude 就会按你定义的 SOP 来执行。相当于你把自己的工作经验和习惯，"教"给了 Claude。

这就像连锁品牌的加盟手册——你把自己的方法论写成标准流程，Claude 就变成了一个完全按你的方式工作的"虚拟员工"。

**总**结一下：Skills 就是 AI 时代的 SOP。它让 Claude 从"我能做"变成"我能按最高标准、稳定地做好"。

**它的**

**目录结构规范**：

• SKILL.md：定义技能的元数据、触发条件和核心逻辑（大脑指令）。

• scripts/：可选的可执行脚本（自动化工具）。

• templates/：领域特定的代码或文档模板；（理论上来说，任何文件夹，例如references/或者/API都可以，只要 SKILL.md 里面写清楚了引用就行。

Skills 和 MCP/Hooks 的区别

💡到这里，你肯定是还没弄明白 skills 是个啥的

没关系，接着往下看就行

就像数学题一样，老师讲的时候一堆的公式推导，你是记不住，也不知道干嘛的

那就是疯狂做题

所以后面就是疯狂地练习，不停地实践

![](img/3d84df49f152283f7f9f6229c01cd51d.png)

1.  如何安装 skills

其实每个 skills 仓库的 README 介绍文档目录都有安装教程

但是这里给大家隆重介绍一个神级 skills 安装工具！

💡相当于是安装 skills 的工具

因为当前有很多工具 Claude Code，还有 Codex、Gemini-CLI，以及 Cusor 等工具

大家现在多支持了 skills，但是每个平台的安装方法又不一样，导致大家的学习成本比较高

那么有没有一种方式，我就一直用这个工具来安装 skills，而不用管我用的是那个编程工具

那就是下面介绍的 vercel 出品的 skills

地址：[https://github.co](https://github.com/vercel-labs/skills)m/vercel-labs/skills

Plain Text

```
https://github.com/vercel-labs/skills
```

vercel最新出的skills安装工具，一键安装，支持通过命令行直接在 30+种 coding agnet 里安装 skills，无论你用的是 claudecode、opencode、codex、gemini-cli、codebuddy、cursor、antigravity、kilo、droid，通通直接安装！

vercel 一家公司的部署产品，不知道没关系，反正你认为就是一个靠谱的公司吧

教练嘀咕：这直接导致我写了 2 个小时截了一大堆图的教程，全！部！白！写！惊喜不惊喜？意外不意外？哈哈哈哈呜呜呜呜呜～

vercel 的 这个安装skills的 skills这个工具很简单，让我们看一下它的 README。

README 就是告诉我们怎么安装 skills，有很多方式

大家可以先看看，不用都执行，有个大概的认知就行

这个里面的都是命令，需要在终端运行的

苹果电脑可以用自带的「终端」软件

windows 电脑可以用 PowerShell

![](img/162bdafd534e23bb834d217f79115a09.png)

比如说你看到了一个你喜欢的 skills，我就拿宝玉老师的这个 skills 为例吧。

[https://github.com](https://github.com/JimLiu/baoyu-skills)/JimLiu/baoyu-skills

![](img/7d8d65d949ce143764a526e204744047.png)

宝玉老师的 skills 包里有很多 skill，大家可以自行浏览。

[h](https://github.com/JimLiu/baoyu-skills/blob/main/README.zh.md)ttps://github.com/JimLiu/baoyu-skills/blob/main/README.zh.md

![](img/36be362b322b3c22584dec8f019ae278.png)

现在我们新建一个文件夹，比如我准备做小红书家装号了，我起一个新的项目文件夹叫 xiaohongshu-jiazhuang。

![](img/114f1249e3eb2b53cf2843653abe4553.png)

双击进入这个文件夹，然后右键，选择“在终端中打开”。

![](img/1b32c95a68ff05705f135c8976e4c416.png)

按照 skills 工具的使用方法，我们只需要在终端里输入：

Plain Text

```
npx skills add jimliu/baoyu-skills
```

回车

![](img/1ca40833281f17e8f31f66974cdbb505.png)

然后 skills 就会爬整个仓库里面所有的 skill。这个过程中，如果遇到问题，可以直接截图问 Claude code

![](img/ab8b17ea659e49aed06c938165b67274.png)

这里面每个 skills 宝玉老师都写了使用方法。

比如我现在是做小红书家装博主，那么我需要的应该是：

• baoyu-xhs-images：这个是小红书的头图生成器

• baoyu-infographic：信息图生成器

• baoyu-url-to-markdown：把网站爬下来变成 markdown

那么，我只需要上下选择，**按空格选中，然后回车**就行了。

![](img/119abd84d6df5068c7596284c388db44.png)

回车之后会让你选择安装到哪个 coding agent 里面，建议手工选择，不要一股脑全选。比如我写文章的时候用 gemini-cli，那么我就选择 gemini-cli。

这里有三个选项，第一个是和上次一样，如果你第一次使用 skills 的话是不会有这个提示的；第二个是所有 agents，只要你电脑装的 agent 全部都安装，第三个是自己选择。我这里为了演示给大家选择自己选择。

![](img/7c4ead932e69edc476dd2a9ab0b89286.png)

同样的，也是上下键选择，空格选中，回车进入下一步。

![](img/85543a97f9a30d05fa336a612d2a7bb0.png)

我这里选择 gemini-cli，回车。然后它会让我选择安装在哪。这里强烈推荐大家安装到当前的项目文件及下，也就是第一个 project。回车。

![](img/f68dc96acc2c44c312586b61dea0e76a.png)

安装方式，选择默认的 symlink。

![](img/ab64f26afebacc2398119213a3448259.png)

再次回车。这个时候会告诉我们安装到哪里了，我们现在可以看到安装在根目录下了。然后最后一步就是安装确认了，选择 yes，回车。

![](img/f660bc9c433810ac4bb41929e1a92154.png)

安装完成！

![](img/bb0f878cde0836718f0eff93a3d645bd.png)

就这么简单！

💡然后再说明一些注意事项。在安装 skills 的时候，我们需要谨记以下几个核心要求：

1.  尽量不要全局安装 skills，特别是带有特定业务场景下才使用的 skill，防止模型跑任务的时候乱激活；

1.  同一个项目内不要安装超过 10 个 skills，容易串；

1.  尽量不要做 skill 激活 skill 的流程，容易套娃引用，推荐在 AGENT.md 或者 CLAUDE.md 里声明已安装 skills 的使用场景及使用流程。

! ! 注意事项！！

**另外现在 skills 有点泛滥**的味道，特别是 OpenClaw 火爆后

爆出很多 skills 留后门，出现一些安全事故

所以大家安装 skills 的时候一定要确认来源

**不要安装不知道来源的 skills，以防对自己的**电脑、账号 token 带来不必要的伤害

![](img/57c84d63532ac183b498bdf89f601402.png)

3.到哪找好用的 skills

这里推荐一些 skills 门户和 gith**u**b 上比较火爆的 skills 仓库。这部分内容仅给大家了解使用，不需要你全部下载，如果已经安装了 skills，可以进入到 1.4 的实操部分

• **vercel 官方做的网站**

网址：https://skills.sh/

![](img/c202f47696d85fddbfeae05d4a74dfd8.png)

非常推荐大家使用 vercel 的 skills 市场，因为上面有统计使用 npx skills 安装的次数，安装次数越多表明用的人越多。值得注意的是，find-skills 这个 skill 在每一次使用 npx skills add 安装的时候都会被推荐，有些人没看清楚就直接装进去了，所以这个次数是没意义的。主要看下面的 skills 安装次数。

![](img/8c4f622a16ba0751b6cdbfc6bb4caa4e.png)

[直接在这里输入需要](http://skills.sh)搜索的 skills，注意，skills.sh里面本身是不带语义识别的，所以不适合在这里找你想要的 skill，这里只适合去看一下最近有什么 skill 火了。

![](img/4c34d8d9d98508671668c692eb62dec9.png)

这里就可以看到排名，比如 azure 系列的 skills 排名上升特别快。

![](img/ca5852ff2d6c49c2798970b09a48b56a.png)

点一个你感兴趣的，比如这个 remotion-best-practices。这是一个做网页动画的 skill。

![](img/1935313fef7da10b122ca46ca1226202.png)

进来之后点右边的复制按钮，然后打开 cli 就可以安装了，具体可以看 1.2 节。

• **一个韩国小哥做的网站**

网站地址：[skillsmp.com](http://skillsmp.com)

![](img/5ba08bc39d64916239a46ec670797435.png)

这个网站什么 skill 都有，基本上属于全收录，但是也没有官方背书，所以你得自己精挑细选。

![](img/bc2252404b8acbc296dba02656cb13a1.png)

进来之后直接搜索就可以，支持语义搜索，比如我想搜一个自动写作，我就输入写作。

![](img/5a1e0e2fb3ed2449617e4508e085282a.png)

这样就出来了，然后点进去看看。

![](img/e11b6c745b3cd427c86fdfd14e23e12b.png)

直接点击右边[skills.sh](http://skills.sh)的安装指令，到终端安装就行，具体看 02 部分。

![](img/27c2cf8cc17c77916b406f6c1e3820c5.png)

下面也会有很多说明和相关的内容，可以随意浏览。

![](img/40a8e5b475e7a920b09d6cedef0882a3.png)

下面就是一些 skill仓库的介绍。

**Github**

Github 上的 skills 才是真正的一手资料，这里推荐几个仓[库，大家自由去学习](http://skills.sh)和安装。安装的方式也很简单，找到了你喜欢的 skill，你就到skills.sh去搜它，然后使用 npx skills add 安装就可以了。

• Anthropic 官方仓库

◦地址：[https://github.c](https://github.com/anthropics/skills)om/anthropics/skills

◦这个是 anthropic 官方做的 skills 案例，基本上把一些最常用的 skills 都植入进来了。如果想要学习 skill 怎么写，一定要 clone 这个仓库然后向 claudecode 刨根问底，一定能找到好东西，学到制作 skills 的终极技巧。

![](img/64678eaeaaf0c3bbb769de3ecdc7b72b.png)

• **官方 plugin**

地址：[h](https://github.com/anthropics/claude-plugins-official)ttps://github.com/anthropics/claude-plugins-official

◦plugin 是一个具体的 claudecode 插件，目前只有 claudecode 能用，不像 skills 那么普及。主要原因是 plugin 自带了 skills、mcp、subagents、hooks 等多种功能，相当于一次安装一个组合。

![](img/51de9412470bbe1596d1642b012367f9.png)

◦比如这个 ralph loop plugin，就自带了 command、hooks、scripts，是一个特别厉害的功能开发循环。但是它不是普通的 skills，它实际上是有自定义提示词、hooks 和自动化脚本组成的一个完整插件。

• **Awesome-skills**

地址：[https://github.com/ComposioHQ/a](https://github.com/ComposioHQ/awesome-claude-skills)wesome-claude-skills

![](img/9af3aca7ea76504d62e7fe9aa5373aff.png)

◦这是一个高星 github 仓库，我一开始做的 skills 指北丢进 notebookLM 的材料就是从这个仓库提取的，里面基本上涵盖了 80% 以上的用户场景，不过作者最近没怎么更新了。

• Marketing-skills

地址：[https://github.com/coreyhain](https://github.com/coreyhaines31/marketingskills)es31/marketingskills

介[绍：这是一个做独立](http://skills.sh)站的市场营销 skills 组合，非常适合搞网站的人去做。seo 到定价策略到社媒运营全部都有，可以去skills.sh一个个看。

![](img/29c0bb4f853ccd892123c489a68007eb.png)

• **superpowers**

地址：https://github.com/obra/superpowers

介绍：这也是一个做网站用的 skills 集合，我特别喜欢 brainstorming 这个 skill，我有很多点子都是靠这个玩意帮我做的。

![](img/3fccc1a13bf2a2542fc84ee72335b2bd.png)

**全平台常用 skills**

值得注意的是，绝大多数高星 skills 或者安装次数多的 skills 全部都是面向 AI 变成的 skill，所以搞 vibe coding 的那群人 skills 用的很多也很勤，也会写很多 skills 来开源。我这里介绍一些我常用的 skills。

• Brainstorming

来源：superpowers

说明：头脑风暴 skill，能提出很多好点子；

使用场景：如果觉得自己不太有想法，可以使用这个

Markdown

```
npx skills add https://github.com/obra/superpowers --skill brainstorming
```

•

Doc-coauthoring

来源：Anthropic 官方

文档撰写 skills，先出大纲，然后分章书写，写的老好了，基本都在你的控制范围里；

Markdown

```
npx skills add https://github.com/anthropics/skills --skill doc-coauthoring
```

•

Web-design-guidelines

来源：vercel

做网页设计的时候使用，会有更好的布局思路；

Markdown

```
npx skills add https://github.com/vercel-labs/agent-skills --skill web-design-guidelines
```

•

Frontend-design

来源：Anthropic 官方

前端设计，可以和 web-design-guidelines 联合使用；

Markdown

```
npx skills add https://github.com/anthropics/skills --skill frontend-design
```

•

Shadcn-ui:

说明：如果你的网站使用了 shadcn/UI，可以考虑装这个 skill，它会自动根据你的网页布局写 shadcn 的组件并嵌入到网站里，不会直接在页面上写死内容；

Markdown

```
npx skills add https://github.com/giuseppe-trisciuoglio/developer-kit --skill shadcn-ui
```

•

Vercel-react-best-practices

说明：网站写完了之后用这个 skill 检查，可以查出来很多结构问题、布局问题以及样式问题，效果还是很不错的，推荐使用 codex 跑这个 skill；

Markdown

```
npx skills add https://github.com/vercel-labs/agent-skills --skill vercel-react-best-practices
```

•

seo-audit:

seo 审查 skill，网站全部做完了之后跑一遍 seo-audit，这个 audit 审计 skill 能帮你检查 metadata、robots.txt、sitemap，还有网站内页的 keywords、标题等等，总之跑两边循环把该改的改了。

Markdown

```
npx skills add https://github.com/coreyhaines31/marketingskills --skill seo-audit
```

如果你不做 AI 应用出海，你可以根据自己实际的业务考[虑其他的 skills，例如大家所熟](https://github.com/JimLiu/baoyu-skills)**悉**的baoyu-skills（地址：https://github.com/JimLiu/baoyu-skills），这个里面内容生成，做自媒体的就比较多。

• baoyu-post-to-wechat

如果你是公众号内容创作者，那这个肯定必不可少。这个就是去发布微信公众号文章的

Markdown

```
npx skills add JimLiu/baoyu-skills --skill baoyu-post-to-wechat
```

•

baoyu-xhs-images

生成小红书信息图系列（1-10 张），支持 11 种视觉样式和 8 种布局

Markdown

```
npx skills add JimLiu/baoyu-skills --skill baoyu-xhs-images
```

•

baoyu-post-to-x

发布内容到 X （Twitter），支持文章和带图/视频推文

Markdown

```
npx skills add JimLiu/baoyu-skills --skill baoyu-post-to-x
```

•

baoyu-cover-image

生成文章封面图（支持 2.35：1、16:9、1:1 等比例）

Markdown

```
npx skills add JimLiu/baoyu-skills --skill baoyu-cover-image
```

•

baoyu-comic

知识漫画创作，支持多种艺术风格（Logicomix/Ohmsha 风格）

Markdown

```
npx skills add JimLiu/baoyu-skills --skill baoyu-comic
```

![](img/24d04d4597a350f5ae75ba3b0dcd31c3.png)

1.  做一个自动配图的 skills（小试牛刀）

💡我们日常写文章的时候都需要自己去找配图，很麻烦。无论是公众号文章、博客内容还是其他文本创作，都需要手动搜索、筛选、下载合适的配图，这个过程往往会打断创作思路，降低工作效率。

我们可以做一个配图 Skill，让 Claude Code 根据文章内容自动生成匹配的插画风格配图。这个 Skill 自动化程度很高，只需输入文章内容就能自动生成配图，适用范围也很广，公众号、博客、文档等各类文本内容都可以用。更重要的是成本可控，我们可以通过限定生成数量来控制 API 调用成本，还能预设插画风格，保持视觉一致性。

完成这个 Skill 的搭建后，你会掌握如何向 Claude Code 清晰表达一个带有 API 调用的 Skill 需求，如何获取和配置第三方 AI 图像生成服务的 API 密钥，如何在需求描述中设定合理的限制条件（比如生成数量、风格要求），以及如何让 Claude Code 自动完成 Skill 的创建和配置。

预计完成时间是 5 到 10 分钟。

4.1 与 Claude Code 沟通需求

在让 Claude Code 创建 Skill 之前，我们需要明确几个关键信息：

Skill 的功能定位是什么（自动为文章生成配图）；使用的 API 服务是哪个（gemini-3-pro-image-preview，通过 APImart 平台调用）；有什么限制条件（生成图片数量、风格要求）；以及 Skill 的名称（便于后续管理和调用）

**需求描述操作（如下图所示）：**

步骤 1：打开 Claude Code 对话界面

打开 Claude Code 的对话界面，在终端或 IDE 中启动 Claude Code，确保当前工作目录是你希望创建 Skill 的位置，这一步是为了让 Skill 文件保存在正确的地方。

![](img/39c2e7c3be48a0835b4772227aa7fc78.png)

**步骤 2：输入需求描述**

向 Claude Code 输入以下内容（可根据实际需求调整）：

因为要调用 API 接口，使用 nanobanana pro 生成的话不便宜，所以限定生成 3 张。因为是配图要有插画感，所以限定了一些细节。最后给 skill 取好了名字，因为 cc 自己取的名字大多相似，容易搞混，最好还是自己取个名字为妙

Plain Text

```
我需要你帮我设计一个skill，这个skill主要是用来帮我实现文章配图。当我写完一篇文章之后，就可以调用这个skill，帮我文章配图。我的api是apimart，调用模型选择gemini-3-pro-image-preview（Nano Banana 2），这是模型调用的文档：https://docs.apimart.ai/

然后我的要求是：
每篇文章只要生成3张图片，前30%、中间30%、最后30%各一张图片。

图片中如果有文字的话，都需要使用中文；
图片风格固定成手绘漫画风格，温暖、亲和、有故事感，不偏写实、不偏赛博朋克，适合内容平台配图（横向或方形构图，画面干净，主体清晰）

这个skill的名字叫&quot;插画风格配图生成skill&quot;。
```

PS：注意，这个时候可能Claude code读取不到网站文档，你可以把文档里面的页面直接一键复制，发给CC

Plain Text

```
https://docs.apimart.ai/
```

![](img/55d369fc477d583723d2872a98ef8990.png)

![](img/184deb12a94ff2ba6eab9d13fb751f12.png)

步骤 3：按下 Enter 键，提交需求

输入完成后按下 Enter 键，这一步是为了让 Claude Code 开始理解你的需求并准备创建 skill。

**注**意：这一步后，Skill 已经创建好了，但还没有配置 APImart 的 API 密钥，需要进入到下一步里面，配置你的 API

![](img/d52bc69f10c72a8eaaaf9cc4b671ae3f.png)

4.2 获取 APImart API 密钥

APImart 是一个专业的 AI 模型 API 聚合平台，提供了包括 gemini-3-pro-image-preview（Nano Banana 2）在内的多种 AI 图像生成模型。

**选择 APImart 的原因：**

接口稳定可靠，调用成功率高；按使用量付费，成本透明（每次生成 0.05 美元）；支持多种主流 AI 模型；文档完善，易于集成；支持 4K 输出、图像编辑、专业工具，适合商业用途。

API 密钥获取操作（如下图所示）：

步骤 1：注册并登录 APImart

先打开浏览器访问[https://apimart.ai/zh/mod](https://apimart.ai/zh/model/nano-banana-2-api)el/nano-banana-2-api，这一步是为了进入 APImart 的注册登录页面。

Plain Text

```
https://apimart.ai/zh/model/nano-banana-2-api
```

点击页面右上角的【注册】或【登录】按钮，如果是第一次使用需要先注册账号，可以使用邮箱或第三方账号（如 Google、GitHub）进行注册，完成注册后使用账号密码登录，这一步是为了创建你的 APImart 账户，后续所有的 API 调用都会关联到这个账户。

注册成功后，系统可能会发送一封验证邮件到你的邮箱，打开邮箱找到这封邮件，点击邮件中的验证链接完成邮箱验证，这一步是为了确认你的邮箱地址是真实有效的。

验证完成后，使用你的账号密码登录 APImart，这一步是为了进入 APImart 的管理后台。

![](img/8bba23b14e3e16283fe5155efdae926d.png)

![](img/96dbb253e27ecbc3cca263b178b24b50.png)

![](img/821e336e964c1bc5570cd8bc4c1ae8f6.png)

**步骤 2：进入账号设置页面**

登录成功后，在页面点击进入【API 密钥】，这一步是为了找到 API 密钥管理的入口，在这里可以创建和管理你的 API 密钥。

![](img/24f3be9137ed6a5d4609aca7584081f5.png)

如果你想创建一个新的 API Key，点击【创建 API 密钥】按钮，系统会弹出一个对话框，要求你输入 API Key 的名称（比如"Claude-skill"），输入名称后点击【确定】或【创建】按钮，系统会自动生成一个新的 API Key 并显示在页面上，点击【复制】按钮将 API Key 保存好，这一步是为了创建一个新的 API Key。

![](img/7567061ba6404630f9b80e46fa87f270.png)

**重要提示：**

API Key 是调用 APImart 服务的身份凭证，必须严格保密。不要将 API Key 分享给任何人，不要将包含 API Key 的配置文件上传到公开的代码仓库（如 GitHub）。如果 API Key 泄露，别人可以使用你的账户调用 API，消耗你的余额。

**步骤 3：充值账户余额**

在个人中心或账户管理页面中，找到【账单】选项并点击，这一步是为了进入充值页面，给账户添加余额。

APImart 采用预付费模式，需要先充值才能调用 API。在充值页面中，你会看到多个充值金额选项（比如 5 美元、10 美元、20 美元、50 美元等），选择一个合适的金额，建议首次充值 5 到 10 美元，足够测试和初期使用，这一步是为了选择充值金额。

![](img/5374e16c340f7dcbc8d51c4e96bcdae9.png)

选择充值金额后，点击【充值】或【支付】按钮，页面会跳转到支付页面，根据页面提示选择支付方式（信用卡、PayPal、支付宝等），完成支付，这一步是为了完成充值，给账户添加余额。

**注意：**

APImart 支持国际支付，如果你使用信用卡支付，需要确保你的信用卡支持国际支付（VISA、MasterCard 等）。如果你没有国际信用卡，可以使用 PayPal 或其他支持的支付方式。

充值成功后，页面会显示你的账户余额，比如"账户余额：$10.00"，这说明充值已经到账，可以开始使用 API 了，这一步是为了确认充值成功。

**目的说明：**

充值是使用 APImart API 的前提条件。APImart 采用预付费模式，需要先充值才能调用 API。gemini-3-pro-image-preview 模型的调用成本是每次生成 0.05 美元（生成 3 张图片），充值金额会根据实际 API 调用量扣除，未使用的余额会保留在账户中，可以随时查看余额和消费记录。

步骤 4：将 API 密钥提供给 Claude Code

拿到 API key 后，你可以直接把它发给 Claude Code，在 Claude Code 的对话界面中，当它询问 API 密钥时，直接粘贴刚才复制的 API token，Claude Code 会自动将其配置到 Skill 中

这一步是为了让 Claude Code 将 API 密钥配置到 Skill 中，并确保 Skill 能够正确调用 APImart 的图片生成服务。

Plain Text

```
我已经获取了APImart的API密钥，现在需要配置到刚才创建的&quot;插画风格配图生成skill&quot;中。

我的APImart API Key是：[粘贴你的API Key]

同时请确保skill能够正确调用https://apimart.ai/zh/model/nano-banana-2-api这个模型

请帮我：
1. 将API密钥配置到skill的配置文件中
2. 确保skill能够正确调用gemini-3-pro-image-preview模型
3. 配置完成后测试一下skill是否可用
```

或者手动添加 API 密钥（更安全的方式）

如果你知道怎么手动添加到 skill 配置文件中的话，也可以手动添加。等待 Claude Code 创建完 Skill 后，找到 Skill 的配置文件（通常在。claude/skills/插画风格配图生成 skill/目录下），在配置文件中找到 API 密钥配置项，手动填入 API Key，保存文件，这样更安全，可以避免 API 密钥在对话记录中留存。

[注意，给 Claude Code 提供 API K](https://apimart.ai/zh/model/nano-banana-2-api)ey 的时候，记得把https://apimart.ai/zh/model/nano-banana-2-api这个官方的调用页面也一起发给它，这一步是为了让 Claude Code 知道如何调用相关接口，了解 API 的参数格式和调用方式，减少调试时间，提高 Skill 创建的成功率。

Plain Text

```
https://apimart.ai/zh/model/nano-banana-2-api
```

这是 gemini-3-pro-image-preview 模型的官方调用页面，包含了 API 调用的详细说明、参数配置、示例代码等信息。提供这个链接可以帮助 Claude Code 了解 API 的调用方式和参数格式；正确配置请求和响应处理；减少调试时间，提高 Skill 创建的成功率。

**注意事项**

**关于 API 密钥安全**

不要将 API 密钥分享给他人，不要将包含 API 密钥的配置文件上传到公开的代码仓库，如果怀疑密钥泄露，立即在 APImart 后台删除该 API Key 并创建新的。

**关于余额监控**

定期检查 APImart 账户余额，可以在账户管理页面查看余额和消费记录，避免余额不足导致 API 调用失败。

**关于成本控制**

gemini-3-pro-image-preview 的调用成本是每次生成 0.05 美元，每次生成 3 张图片的成本是 0.05 美元（按次计费，不是按张计费），通过限定生成数量来控制成本，建议在测试阶段先小批量调用，确认效果后再大规模使用。

![](img/8eec542cd4aa207f627d6ae9cef01897.png)

4.3 等待 Skill 生成完成

当你完成需求描述和 API 密钥配置后，Claude Code 会自动开始创建 skill。这个过程通常需要 3 到 5 分钟，具体时间取决于 skill 的复杂度、API 文档的解析时间、网络连接速度。

![](img/4299c13af64ff56f82b03be74bc8300e.png)

Claude Code 在后台会做这些事情：先分析你的需求，理解功能要求和限制条件；然后设计 skill 结构，规划输入输出和处理流程；接着编写核心代码文件；再配置 gemini-3-pro-image-preview 的 API 调用逻辑；然后生成 skill 的配置文件；最后进行基本的语法检查和逻辑验证。

五分钟后，配图 skill 就完成了！就是这么简单高效。

当你看到类似以下的提示信息时，说明 Skill 已经创建完成：

Plain Text

```
✓ Skill &quot;插画风格配图生成skill&quot; 创建成功
✓ 配置文件已生成
✓ API调用已配置
```

4.4 验证 Skill 是否可用

步骤 1：查看 Skill 列表

先在 Claude Code 中输入命令/skills list查看 skill 列表，你应该能在列表中看到刚才创建的【插画风格配图生成 skill】，这一步是为了确认 skill 已经成功创建并注册到系统中。

Plain Text

```
/skills list
```

如果你是在 VS Code 插件使用 Claude Code，那么这个命令应该是不会有任何显示的结果，可以直接使用提示词。

提示词如下：

列举下现在可以用的skills列表

步骤 2：测试 Skill 功能

然后测试一下 skill 功能，输入命令调用这个 skill，比如/插画风格配图生成skill "这是一篇关于春天的文章，描述了花开的美景和温暖的阳光。"

如果 skill 正常工作，它会分析文章内容，调用 gemini-3-pro-image-preview API，按照你设定的要求生成 3 张插画风格的配图，这一步是为了验证整个流程是否打通，从输入到输出是否符合预期。

Plain Text

```
/article-image-generator &quot;这是一篇关于春天的文章，描述了花开的美景和温暖的阳光。&quot;
```

Plain Text

```
手绘漫画风格插画，展现传统编程与Vibe Coding的对比。左边是程序员对着满屏代码抓狂，头发凌乱，桌上堆满技术书籍，标注&#x27;传统编程:痛苦敲代码&#x27;。右边是轻松的人在和AI聊天，屏幕显示&#x27;我想要一个网站’，AI回复&#x27;马上为您生成&#x27;，标注&quot;VibeCoding:动口不动手’。温暖的色调，简洁明了的中文标注。
```

Plain Text

```
手绘漫画风格插画，展现&#x27;点菜式编程&quot;的概念。画面中央是一个友善的AI厨师机器人，戴着厨师帽，面前有一个菜单显示&quot;软件菜单:网站、APP、小程序&#x27;。旁边站着一个普通人指着菜单说&#x27;我要一个蓝色风格的登录网站，要简洁的&#x27;。AI厨师回答好的，马上为您制作’，手里端着一个发光的网页模型。背景是温馨的厨房环境，中文标注清晰。
```

**步骤 3：检查生成结果**

最后检查生成结果，查看生成的图片是否符合预期，图片风格是否为手绘漫画风格，图片内容是否与文章主题相关，图片质量是否满足使用需求。如果结果不理想，可以调整需求描述中的风格要求，修改 skill 配置文件中的参数，或者重新生成 skill。

![](img/23567a0698e2c345afc2c8e2b3ef007e.png)

![](img/b7326df943d00b510a63e564e2184fa6.png)

**总结与延伸**

完成这个 skill 的搭建后，你已经学会了如何向 Claude Code 清晰描述一个带有 API 调用的 skill 需求，如何获取第三方服务的 API 密钥并配置到 skill 中，如何通过设定限制条件来控制 API 调用成本，以及如何命名、测试和验证自己创建的 skill。

这个 skill 的实际应用场景很广。可以用于公众号文章配图，写完文章后一键生成配图，提高发布效率。可以用于博客内容配图，为技术博客、个人博客生成视觉化配图。可以用于社交媒体内容，为微博、小红书等平台的内容快速配图。可以用于演示文稿配图，为 PPT、Keynote 等演示文稿生成插画。还可以用于文档美化，为技术文档、产品文档添加视觉元素。

如果你想进一步优化这个 skill，可以考虑增加风格选项，支持多种图片风格（写实、抽象、卡通等）。可以实现智能数量控制，根据文章长度自动调整生成图片数量。可以支持图片尺寸定制，适配不同平台的图片尺寸要求。可以实现批量处理，支持一次性为多篇文章生成配图。还可以增加本地保存功能，自动将生成的图片保存到指定文件夹。

**4.5 常见问题解答**

Q1：如果 API 密钥配置错误怎么办？

可以通过以下方式修正。找到 skill 的配置文件（在。claude/skills/插画风格配图生成 skill/目录下），打开配置文件找到 API 密钥配置项，修改为正确的 API 密钥，保存文件后重新测试。

Q2：生成的图片不符合预期怎么办？

可以尝试在调用 skill 时提供更详细的文章描述，修改 skill 配置中的风格参数，调整 prompt 模板增加更具体的风格描述。如果多次调整仍不理想，可以考虑更换其他图像生成模型。

Q3：APImart 余额不足会怎样？

当余额不足时，API 调用会失败，skill 无法生成图片，Claude Code 会返回错误提示，需要登录 APImart 后台充值后才能继续使用。

Q4：可以使用其他图像生成服务吗？

可以。你可以选择其他支持 API 调用的图像生成服务（比如 Replicate、DALL-E、Midjourney API 等），在需求描述中指定使用的服务和 API，按照相应服务的文档获取 API 密钥，让 Claude Code 重新创建 skill。

Q5：如果配件网络错误的问题，请打开tun模式（增强模式）

目前推荐使用 clash.verge 的客户端，不推荐老版本的 clashx 等版本了

英文：一般叫 tun 模式

中文：增强模式，虚拟网卡模式

![](img/2acdc7a93286ff7fb8c658b3e09a6f70.png)

### 02. 实战：自媒体自动发布 Skills

1.公众号自动生成与发布 Skills

💡所有流程化的东西都可以用 skills 来做，推荐大家学习，通过 skills 发推、发公众号、发小红书，没有能力边界，并且可以同时进行，比方说同时用 skills 生成公众号、小红书、视频脚本。

过去我们写公众号需要花费大量的时间，找选题，写内容，配图，发布，一套流程下来，可能一个上午就没了。有了 Skill 之后，我们就可以实现一键完成找选题、写文章、配图再发布的全工作流了。

完成这个 Skill 的搭建后，你会掌握如何让 Claude Code 自动搜索 AI 热点、生成文章内容、调用 API 生成配图、上传图片到微信服务器、将文章发布到公众号草稿箱的完整流程。这是一个相对复杂的 Skill，涉及多个 API 的集成和调用，但按照步骤操作，你也能搭建完成。

预计完成时间是 30 到 60 分钟。

**重点必看：实战篇只需要完成一个 Skills 案例实操即可，我**们是在案例中掌握 Skills 的用法；

**在实**战篇中，公众号难度低于小红书，建议新手先把公众号的 Skills 做出来，然后就可以进入到进阶篇的 AI 视频创作 Skills 了，通过这一个案例，能够先把 skills 上手；

**用起来在实操过程中，遇到的任何问题都可以截**图丢给 Claude code，帮你解决

1.1 重点提前了解

（一）公众号全自动 Skill 的完整工作流程

让我们先理解一下这个 Skill 的完整工作流程，这样你就能明白每个步骤在做什么：

第一步：搜索采集 AI 热点资料

使用 Exa 或 Tavily 这两个专业的 AI 搜索工具，搜索 24 小时内关于指定主题（比如"open claw"）的最新资讯，包括技术突破、市场反应、行业影响等信息，然后将这些信息结构化整理，为后续的文章生成提供素材。

**第二步：撰写文章**

基于搜索到的资料，使用 AI 生成一篇 Markdown 格式的文章。文章会根据你设定的风格（技术深度、通俗易懂、行业分析等）来撰写，同时会在文章中插入图片标记，标注需要配图的位置和图片的描述。

**第三步：生成配图**

解析文章中的图片标记，提取出每张图片的描述（prompt），然后调用 APImart 的 gemini-3-pro-image-preview 模型生成高质量的插画风格配图。生成的图片会符合你预设的风格要求（手绘漫画风格、温暖、亲和、有故事感）。

**第四步：上传图片到微信服务器**

将生成的图片上传到微信公众号的素材库，获取每张图片的 media_id（微信服务器上的图片标识），这样才能在文章中引用这些图片。

第五步：转换为 HTML 并发布到草稿箱

将 Markdown 格式的文章转换为微信公众号支持的 HTML 格式，替换图片占位符为微信服务器上的图片 URL，然后调用微信公众号 API 将文章发布到草稿箱。

**第六步：提示用户检查**

Skill 会返回一个预览链接，提示你去微信公众号后台检查文章。你可以在后台查看文章效果，如果满意就直接发布，如果需要修改可以在后台编辑后再发布。

**（二）涉及的技术和工具**

这个 Skill 涉及多个技术和工具的集成，让我们先了解一下每个工具的作用：

**Claude Code**

这是我们的核心开发工具，用于创建和管理 Skill。Claude Code 可以理解自然语言描述的需求，自动生成代码，配置 API 调用，是整个 Skill 的"大脑"。

**Skill Creator**

这是一个辅助工具，帮助我们快速创建 Skill 的基础结构。它可以自动生成 Skill 的配置文件、代码模板、文档结构等，让我们不需要从零开始搭建。

**微信公众号 API**

微信公众号提供的官方接口，允许我们通过程序的方式管理公众号内容。这是整个 Skill 的核心，因为我们的最终目标是将文章发布到微信公众号。

微信公众号 API 提供了一系列接口，允许我们通过程序的方式管理公众号内容，包括上传图片、创建草稿、发布文章、管理素材等。没有这个 API，我们就无法实现自动发布功能，只能手动在后台操作。

**APImart**

一个 AI 模型 API 聚合平台，提供 gemini-3-pro-image-preview（Nano Banana 2）图像生成服务。用于生成文章配图。虽然我们可以从图库网站下载图片，但那样需要手动搜索、筛选、下载，非常耗时。

使用 AI 图像生成服务，我们可以根据文章内容自动生成匹配的配图，而且可以控制图片的风格、尺寸、内容，确保配图与文章完美契合。

**Exa MCP**

一个专业的 AI 搜索工具，擅长深度搜索和内容理解。我们使用它来搜索和采集 AI 热点资讯。

**Tavily MCP**

另一个专业的 AI 搜索工具，擅长实时热点追踪。我们使用它来补充搜索结果，提高资讯的覆盖面。

**（三）学习目标**

完成这个 Skill 的搭建后，你会掌握：

如何创建一个复杂的多步骤自动化工作流 Skill，如何集成多个第三方 API 服务（微信公众号 API、APImart API、Exa MCP、Tavily MCP），如何处理数据的采集、转换、上传、发布等完整流程，如何配置和管理 API 密钥，如何调试和优化 Skill 的性能。

**1.2**安装 Skill Creator 和两个工具**

在开始创建公众号自动发布 Skill 之前，我们需要先安装 Skill Creator 这个工具。

Skill Creator 是一个帮助我们快速创建和管理 Skill 的辅助工具，它可以自动生成 Skill 的基础结构、配置文件、代码模板等，大大简化 Skill 的创建过程。

（一）什么是 Skill Creator？

Skill Creator 本身也是一个 Skill，但它的作用是帮助你创建其他 Skill。你可以把它理解为一个"Skill 工厂"，它知道如何搭建一个标准的 Skill 结构，如何配置各种参数，如何集成不同的 API 服务。

使用 Skill Creator 的好处是：

• 不需要手动创建文件夹和配置文件，Skill Creator 会自动生成标准的目录结构

• 不需要从零开始写代码，Skill Creator 会根据你的需求生成代码模板

• 不需要担心配置错误，Skill Creator 会按照最佳实践来配置 Skill

• 可以快速迭代和修改，Skill Creator 支持增量更新和版本管理

（二）Skill Creator 和两个工具安装操作（如下图所示）

步骤 1：打开 Claude Code 对话界面

先打开 Claude Code 的对话界面，在终端或 IDE 中启动 Claude Code，确保 Claude Code 已经正常运行，这一步是为了准备好创建 Skill 的环境。

![](img/8b19f7c7eb43e1fd5b48aee550f2a32d.png)

此处提前安装 Exa 和 Tavily 这两个 MCP

这**两**个 MCP 是 Skill 获取外部信息的关键，在后面 skills 运行中会用到，所以我们先安装了。核心逻辑是：你需要先去各自的官网注册账号并获取 API Key，然后把配置指令发给 Claude Code，让它帮你自动修改配置文件。

**科普介绍**

**关于 MCP**MCP 的全称是 Model Context Protocol（模型上下文协议），它是一种让 AI 模型能够访问外部工具和数据源的标准协议。你可以把 MCP 理解为 AI 的"插件系统"，就像浏览器可以安装扩展插件一样，Claude Code 也可以通过 MCP 来扩展它的能力。

默认情况下，Claude Code 只能处理你直接提供给它的信息，无法主动去互联网上搜索资料。但通过安装 MCP，Claude Code 就可以调用外部的搜索服务、数据库、API 等，获取实时的、最新的信息。

在我们这个 Skill 中，MCP 的作用是让 Claude Code 能够搜索 24 小时内的 AI 热点资讯。没有 MCP，Claude Code 只能根据它的训练数据来生成文章，无法获取最新的新闻和动态。有了 MCP，Claude Code 就可以实时搜索互联网，获取最新的资讯，生成的文章内容才会是最新的、最相关的。

如果不使用 MCP，我们只能手动搜索资料，然后把搜索结果复制粘贴给 Claude Code，让它基于这些资料生成文章。这样就非常耗时，也无法实现自动化，但**使用 MCP 后，这些工作都可**以自动完成。你只需要告诉 Skill** 一个主题关键**词，Skill 就会自动搜索、筛选、整理资料，然后生成文章，整个过程完全自动化。关于 Exa 和 TavilyExa 和 Tav**ily 都是专业的 **AI** 搜索工具，但它**们各有特点和优势：Exa 的特点Exa 擅长深度搜索和内容理解。它不仅仅是简单地匹配关键词，而是能够理解搜索意图，找到真正相关的内容。Exa 还擅长内容质量评估。它会自动过滤低质量内容（如广告、垃圾信息、重复内容等），只返回高质量的、有价值的内容。这样可以确保生成的文章基于可靠的信息源，而不是基于不准确或误导性的信息。Tavily 的特点Tavily 擅长实时热点追踪。它专门针对新闻和热点事件进行优化，可以快速找到 24 小时内的最新动态。比如你搜索"AI 最新新闻"，Tavily 会优先返回最近几小时或几天内发布的新闻，而不是几个月前的旧新闻。

Tavily 还擅长多源整合。它会从多个新闻网站、社交媒体、技术博客等渠道采集信息，然后整合成一个完整的视图。这样可以确保你获取的信息是全面的，不会遗漏重要的动态。**为什么需要两个搜索工具？**这是因为它们的优势是互补的。Exa 擅长深度搜索，可以找到高质量的、有深度的内容，但可能不够实时。Tavily 擅长实时追踪，可以找到最新的动态，但可能深度不够。

同时使用两个工具，可以结合它们的优势：用 Tavily 找到最新的热点新闻，用 Exa 找到相关的深度分析文章。这样生成的文章既有时效性（基于最新的新闻），又有深度（基于专业的分析）。可以只用一个吗？

可以。如果你的预算有限，或者觉得配置两个 MCP 太麻烦，也可以只使用其中一个。建议优先使用 Tavily，因为它更适合追踪 AI 热点。但如果只用一个，生成的文章质量可能会略有下降，因为信息来源会更单一。

**安装 Tavily MCP**

步骤 1：访问 Tavily 官网并注册

先打开浏览器，在地址栏输入https://tavily.com并按回车键访问 Tavily 官网，这一步是为了进入 Tavily 的注册登录页面。

Plain Text

```
https://tavily.com
```

页面加载完成后，在页面右上角找到【Sign up】或【Get Started】按钮并点击，这一步是为了开始注册流程。

在注册页面中，你可以选择使用 Google 账号快速注册（推荐），点击【Sign up with Google】按钮，然后在弹出的窗口中选择你的 Google 账号并授权登录，这一步是为了快速完成注册，不需要填写复杂的表单。

如果你没有 Google 账号或不想使用 Google 账号，也可以选择使用邮箱注册，输入你的邮箱地址和密码，然后点击【Sign up】按钮，这一步是为了使用传统方式注册账号。

注册成功后，系统可能会发送一封验证邮件到你的邮箱，打开邮箱找到这封邮件，点击邮件中的验证链接完成邮箱验证，这一步是为了确认你的邮箱地址是真实有效的。

![](img/cdbcba526f0128d31956a2199790258e.png)

**步骤 2：获取 API Key**

验证完成后，登录 Tavily，页面会自动跳转到 Dashboard（仪表板）页面，这一步是为了进入 Tavily 的管理后台。

在 Dashboard 页面中，找到【API Key】或【API Keys】选项，通常在页面的左侧菜单或顶部导航栏中，点击进入 API 密钥管理页面，这一步是为了找到 API 密钥管理的入口。

在 API 密钥管理页面中，你会看到一个默认的 API Key（Tavily 在注册时会自动生成一个），这个 API Key 通常以"tvly-"开头，比如"tvly-abc123def456"，找到这个 API Key 后，点击旁边的【Copy】按钮将它复制到剪贴板，然后粘贴到一个安全的地方保存好，这一步是为了获取 Tavily 的 API 密钥。

**注意：**

Tavily 提供免费额度，通常每月可以免费调用 1000 次左右（具体额度以 Tavily 官方为准）。如果免费额度用完了，需要升级到付费计划。对于测试和初期使用，免费额度通常是足够的。

![](img/fbf8ade47adf4590e8e59895a4c853e6.png)

步骤 3：让 Claude Code 安装 Tavily MCP

拿到 Tavily 的 API Key 后，回到 Claude Code 的对话界面，向它发送以下内容：

请帮我安装 Tavily MCP。我的 API Key 是 tvly-xxxxxx（替换为你刚才复制的 Key）

Plain Text

```
请帮我安装Tavily MCP。我的API Key是tvly-xxxxxx
```

这一步是为了让 Claude Code 自动配置 Tavily MCP，将 API Key 写入配置文件，完成 MCP 的安装和激活。

Claude Code 会执行以下操作：检查系统中是否已经安装了 Tavily MCP，如果没有安装，会自动下载并安装；找到 MCP 的配置文件（通常在。claude/mcp/目录下）；将你提供的 API Key 写入配置文件；重启 MCP 服务，使配置生效；测试 MCP 是否可以正常工作。

整个过程通常需要 1 到 2 分钟，Claude Code 会显示进度信息。当你看到"Tavily MCP 安装成功"的提示时，说明安装已经完成。

![](img/51b9ed246c9be31716375a77527679dd.png)

**安装 Exa MCP**

步骤 1：访问 Exa 官网并注册

先打开浏览器，在地址栏输入[https://exa.ai](https://exa.ai)并按回车键访问 Exa 官网，这一步是为了进入 Exa 的注册登录页面。

Plain Text

```
https://exa.ai
```

页面加载完成后，在页面右上角找到【Sign up】或【Get Started】按钮并点击，这一步是为了开始注册流程。

在注册页面中，你可以选择使用 Google 账号或 GitHub 账号快速注册（推荐），点击对应的按钮，然后在弹出的窗口中授权登录，这一步是为了快速完成注册。

**步骤 2：获取 API Key**

注册并登录后，页面会自动跳转到 Dashboard 页面，在 Dashboard 页面中找到【API Keys】或【Developer】选项并点击，这一步是为了进入 API 密钥管理页面。

![](img/17952fd08c311cf64c6c0068b92e1cc9.png)

在 API 密钥管理页面中，点击【Create API Key】或【Generate Key】按钮，系统会生成一个新的 API Key，点击【Copy】按钮将 API Key 复制到剪贴板，然后保存好，这一步是为了获取 Exa 的 API 密钥。

**注意：**

Exa 也提供免费额度，通常每月可以免费调用一定次数（具体额度以 Exa 官方为准）。如果免费额度用完了，需要升级到付费计划。

步骤 3：让 Claude Code 安装 Exa MCP

拿到 Exa 的 API Key 后，回到 Claude Code 的对话界面，向它发送以下内容：

请帮我安装 Exa MCP。我的 API Key 是 xxxxxx（替换为你刚才复制的 Key）。

Plain Text

```
请帮我安装Exa MCP。我的API Key是xxxxxx
```

这一步是为了让 Claude Code 自动配置 Exa MCP，将 API Key 写入配置文件，完成 MCP 的安装和激活。

Claude Code 会执行类似 Tavily MCP 的安装流程，整个过程通常需要 1 到 2 分钟。当你看到"Exa MCP 安装成功"的提示时，说明安装已经完成。

![](img/d03bb468201e1e6ea00815e7a75e9c49.png)

**步骤 2：向 Claude Cod**e 请求安装 Skill Creator

然后另开一个窗口，在 Claude Code 的对话界面中输入以下内容：

Plain Text

```
请帮我安装Skill Creator这个工具。我需要用它来创建一个复杂的公众号自动发布Skill。
```

这一步是为了让 Claude Code 知道你需要安装 Skill Creator，Claude Code 会自动从官方仓库或推荐的来源获取 Skill Creator 并进行安装。

![](img/669e6254388ad971bdf0cf5f9830c641.png)

**步骤 3：等待安装完成**

Claude Code 会开始下载和安装 Skill Creator，这个过程通常需要 1 到 2 分钟，具体时间取决于网络速度。

安装过程中 Claude Code 会显示进度信息，包括下载文件、创建目录、配置环境等步骤，这一步是为了将 Skill Creator 安装到你的系统中，让它可以被 Claude Code 调用。

当你看到类似以下的提示信息时，说明 Skill Creator 已经安装成功：

Plain Text

```
✓ Skill Creator 安装成功
✓ 配置文件已生成
✓ 工具已就绪
```

![](img/df85380470bcb938a4335f895198cffc.png)

步骤 4：验证 Skill Creator 是否可用

安装完成后，我们需要验证一下 Skill Creator 是否真的可以使用。在 Claude Code 中输入以下命令：

Plain Text

```
/skills list
```

如果你是在 VS Code 插件使用 Claude Code，那么这个命令应该是不会有任何显示的结果，可以直接使用提示词。

提示词如下：

列举下现在可以用的skills列表

这一步是为了查看已安装的 Skill 列表，确认 Skill Creator 是否在列表中。

![](img/1b302baf18025bb4ba44f3dc2af6248f.png)

你应该能在列表中看到【Skill Creator】或类似的名称，这说明 Skill Creator 已经成功安装并注册到系统中。如果没有看到，可能是安装过程出现了问题，需要重新安装。

步骤 5：测试 Skill Creator 功能

为了确保 Skill Creator 能够正常工作，我们可以做一个简单的测试。在 Claude Code 中输入：

Plain Text

```
@skill-creator 帮我创建一个测试Skill
```

![](img/2adf341658a69b793bf5cfa0cede1e73.png)

如果 Skill Creator 正常工作，它会开始询问你关于这个测试 Skill 的一些问题，比如 Skill 的名称、功能描述、需要的 API 等。这说明 Skill Creator 已经可以正常使用了。你可以输入"取消"来终止这个测试，因为我们现在还不需要真的创建测试 Skill。

**（三）常见安装问题和解决方案**

问题 1：安装完成但在 Skill 列表中找不到

这可能是因为安装路径配置错误或者 Claude Code 没有刷新 Skill 列表。解决方案是：重启 Claude Code，让它重新扫描已安装的 Skill，在 Claude Code 中输入/skills refresh命令刷新 Skill 列表，检查 Claude Code 的配置文件，确认 Skill 安装路径是否正确。

**问题 2：提示"权限不足"**

这可能是因为当前用户没有足够的权限在系统目录中创建文件。解决方案是：在 Mac 或 Linux 系统中，尝试使用sudo命令提升权限，在 Windows 系统中，以管理员身份运行 Claude Code，或者将 Skill 安装到用户目录而不是系统目录。

![](img/d08d620d5583f44a37e0da8842480d72.png)

1.3 和 Claude Code 捋清楚思路

在开始创建 Skill 之前，我们需要先把需求告诉 Claude Code，让它思考如何实现我们的需求。这一步非常重要，因为复杂的需求如果不先梳理清楚，直接让 Claude Code 创建 Skill 容易出错，可能会导致 Skill 功能不完整、逻辑混乱、或者根本无法运行。

**（一）为什么要先梳理思路？**

你可能会想，为什么不直接告诉 Claude Code"帮我做一个公众号自动发布 Skill"就可以了？为什么还要花时间梳理思路？

这是因为"公众号自动发布"这个需求其实非常复杂，它包含了多个子功能：搜索热点、生成文章、配图、上传、发布等。如果直接让 Claude Code 实现，它可能会：

设计一个过于复杂的方案，包含很多你不需要的功能，导致开发时间长、调试困难。或者设计一个过于简单的方案，缺少关键功能，导致 Skill 无法满足实际需求。

或者没有考虑到技术限制，设计的方案在实际中无法实现。或者没有考虑到成本问题，设计的方案调用 API 的成本过高。

所以我们需要先和 Claude Code 一起梳理思路，明确需求的边界，确定技术方案的可行性，然后再开始实际的开发工作。这个过程就像建房子之前先画设计图，虽然多花了一些时间，但可以避免后期返工，最终反而更快。

（二）需求沟通操作（如下图所示）

步骤 1：向 Claude Code 描述初步需求

先打开 Claude Code 的对话界面，向它描述你想要实现的功能。这里有一个技巧：在描述需求时，加上"ultrathink"这个关键词，可以让 Claude Code 进入深度思考模式，给出更详细、更全面的分析。

你可以这样输入：

Plain Text

```
我要做一个全网自动做AI热点，自动写文章，自动配图，自动上传发布的skill，先不要直接写这个skill，我们先梳理一下思路，怎么样才能高质量的实现这个功能，ultrathink
```

这一步是为了让 Claude Code 先进行深度思考，给出一个完整的实现方案，而不是直接开始写代码。"先不要直接写这个 skill"这句话很重要，它明确告诉 Claude Code 现在是规划阶段，不是实现阶段。

![](img/a1963767bdc4e20f01307b567dbefc65.png)

步骤 2：查看 Claude Code 给出的初步方案

Claude Code 会进入深度思考模式，分析你的需求，然后给出一个详细的解决方案。这个方案可能会非常详细，包含多个模块和复杂的架构设计。

比如 Claude Code 可能会提出这样的方案：

**核心架构设计**

核心架构设计四大核心模块：

热点发现引擎 - 多源数据采集 + 智能评估

内容生成引擎 - 结构化写作 + 质量控制

配图生成引擎 - AI 图片生成 + 风格统一

多平台发布引擎 - 差异化适配 + 自动发布

关键质量保证点热点筛选质量：

多维度评估（热度趋势、时效性、受众匹配）

内容过滤（避免低俗、重复、过时内容）

智能去重（避免同质化热点重复处理）内容生成质量：

结构化模板（标题优化、逻辑框架、SEO 布局）

深度控制（背景补充、多角度分析、数据支撑）

原创性保证（事实核查、语言润色、重复度检测）系统可靠性：

微服务架构 + 事件驱动

多层审核机制（AI 初审 + 人工抽检）

风险控制（法律、平台、技术风险管理）

实施路径建议

MVP 阶段：单源抓取 → 基础生成 → 简单配图 → 单平台发布优化阶段：多源整合 → 质量提升 → 高质量配图 → 多平台适配

高级阶段：智能预测 → 个性化生成 → 互动功能 → 商业化

技术栈推荐：Python + FastAPI + Redis + PostgreSQL + Docker

这个系统的成功关键在于质量控制和风险管理，而不是单纯的自动化。建议先从 MVP 开始验证核心逻辑，再逐步优化各个环节。

这个方案看起来非常完整和专业，但对于我们来说太复杂了，像这种复杂的需求最好还用多个 skill 来完成，单个 skill 去跑的话容易出错。实现这样一个完整的系统可能需要几天甚至几个周的时间，而且涉及很多复杂技术，对于新手来说难度太大。

所以我们需要简化方案，聚焦在核心功能上，先实现一个可用的 MVP（最小可行产品），然后再根据实际使用情况逐步优化和扩展。

步骤 3：要求 Claude Code 简化方案

向 Claude Code 发送简化需求，明确告诉它我们的实际需求范围和限制条件：

Plain Text

```
我感觉这个操作流程太复杂了，我们的热点来自x，24小时内容热AI内容，发布平台暂时就限制在公众号，使用公众号的API进行发布，你简化一下这个方案，整体的逻辑实现按照这个逻辑来实现&quot;1. Exa/Tavily 搜索采集 AI 热点资料 → 2. 撰写文章（Markdown 格式）  →  3. 调用 nanobanana API 生成配图 → 4. 上传图片到微信服务器  → 5. 转换为 HTML 并发布到公众号草稿箱  → 6. 提示用户去微信公众号后台检查文章&quot;
```

![](img/07e1058a9decacafc5da9e2839db2763.png)

这一步是为了让 Claude Code 明确我们的实际需求范围，避免设计过于复杂的方案，聚焦在可实现的核心功能上。

注意这里我们明确了几个限制条件：

• 热点来源：只从 x（Twitter）搜索，不需要多源采集

• 内容范围：只关注 24 小时内的 AI 热点，不需要其他领域

• 发布平台：只发布到微信公众号，不需要多平台适配

• 发布方式：发布到草稿箱，由用户最后检查，不需要自动发布

这些限制条件大大降低了系统的复杂度，让我们可以快速实现一个可用的版本。

**步骤 4：确认简化后的方案**

Claude Code 会给出一个更加实用和可操作的方案。让我们详细看看这个简化后的方案：

XML

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

这个简化后的方案就相对可行很多了。它聚焦在核心功能上，去掉了不必要的复杂设计，技术实现也更加简单直接。我们就让 Claude Code 按照这个方案来实现。

**数据流转图解**

让我们用一个简单的流程图来理解数据是如何在各个模块之间流转的：

Plain Text

```
用户输入主题 → Exa/Tavily搜索 → 获取热点资讯 →
AI生成文章（Markdown） → 解析图片标记 →
APImart生成配图 → 上传到微信服务器 →
获取media_id → Markdown转HTML →
替换图片URL → 发布到草稿箱 →
返回预览链接 → 用户检查 → 发布
```

每个箭头代表数据的流转，每个步骤都有明确的输入和输出。这样的设计让整个流程清晰可控，任何一个环节出问题都可以快速定位和修复。

![](img/322eb04527f1b8690a099cd3e7afb8e3.png)

1.4 整理 Claude Code 需要的 API 等资料

确定了 skill 的逻辑后，我们需要问一下 Claude Code 需要哪些资料，然后去收集这些资料。如果不会操作就让 Claude Code 给出详细的步骤一步步进行。

**（一）询问所需资料**

先向 Claude Code 询问需要准备哪些资料：

Plain Text

```
ok，这个逻辑没问题，接下来我们要进行实现了，你看看我需要你给哪些资料，比如API等。
```

这一步是为了明确我们需要准备哪些 API 密钥、配置信息等资料，避免在创建 Skill 的过程中因为缺少资料而中断。

![](img/f6b22a2d99057ffcb053d036900b957b.png)

Claude Code 会告诉你需要准备以下资料：

微信公众号 AppID 和 AppSecret：

用于调用微信公众号 API，这是身份认证的凭证。

APImart API Key：

用于调用 gemini-3-pro-image-preview 生成配图，这是付费服务的凭证。

（二）获取微信公众号 AppID 和 AppSecret

微信公众号的 AppID 和 AppSecret 是调用微信公众号 API 的核心凭证，就像你的账号和密码一样重要。没有这两个凭证，我们就无法通过程序的方式操作公众号。

**AppID（应用 ID）**

这是你的公众号在微信开放平台上的唯一标识，就像你的身份证号码一样。每个公众号都有一个唯一的 AppID，通过这个 ID，微信服务器可以识别是哪个公众号在调用 API。AppID 是公开的，可以在代码中明文使用。

**AppSecret（应用密钥）**

这是你的公众号的密钥，就像你的密码一样。AppSecret 必须严格保密，不能泄露给任何人，也不能上传到公开的代码仓库。如果 AppSecret 泄露，别人就可以冒充你的公众号调用 API，可能会导致内容被篡改、数据被窃取等严重后果。

AppID 和 AppSecret 的关系

AppID 和 AppSecret 必须配对使用，就像用户名和密码一样。当你调用微信公众号 API 时，需要同时提供 AppID 和 AppSecret，微信服务器会验证这两个凭证是否匹配，只有匹配成功才会允许 API 调用。

微信公众号 API 获取操作（如下图所示）

步骤 1：进入微信公众号开发者平台

先打开浏览器，在地址栏输入[https://developers.we](https://developers.weixin.qq.com/platform)ixin.qq.com/platform并按回车键访问微信公众号开发者平台，这一步是为了进入微信公众号的开发者后台，在这里可以获取 API 调用所需的凭证。

Plain Text

```
https://developers.weixin.qq.com/platform
```

页面加载完成后，你会看到一个登录页面，使用你的微信扫描页面上的二维码进行登录，这一步是为了验证你的身份，确保只有公众号的管理员才能获取 API 凭证。

扫码后在手机上确认登录，然后页面会自动跳转到开发者平台的主页，这一步是为了完成身份验证，进入开发者后台。

**步骤 2：进入公众号管理页面**

登录成功后，在页面顶部找到【我的业务】菜单，点击它会展开一个下拉菜单，在下拉菜单中找到并点击【公众号】选项，这一步是为了进入公众号管理页面，在这里可以管理你的公众号的各种开发配置。

![](img/e663f4482ce406c13f262c03b06ea8b9.png)

**步骤 3：获取开发密钥**

进入公众号管理页面后，在页面左侧或下方找到【开发密钥】或【开发设置】选项并点击，这一步是为了进入密钥管理页面，在这里可以查看和生成 AppID 和 AppSecret。

![](img/36f20b82994d2b646cdaf2b2b4876602.png)

在开发密钥页面中，你会看到两个重要的信息：

**AppID（开发者 ID）**

这个通常会直接显示在页面上，是一串以"wx"开头的字符串，比如"wx1234567890abcdef"。找到 AppID 后，点击右侧的【复制】按钮将它复制到剪贴板，然后粘贴到一个文本文件中保存好，这一步是为了保存 AppID，后续配置 Skill 时需要用到。

AppSecret（开发者密钥）

这个通常不会直接显示，而是显示为一串星号（**）。找到 AppSecret 旁边的【重置】或【生成】按钮并点击，这一步是为了生成或重置 AppSecret。

点击后系统会弹出一个确认对话框，提示你"重置密钥后，旧密钥将立即失效，使用旧密钥的应用将无法调用 API，是否确认重置？"，点击【确定】按钮，这一步是为了确认生成新的 AppSecret。

系统会要求你进行身份验证，可能需要你用微信扫码或输入验证码，完成验证后，页面会显示新生成的 AppSecret，这是一串随机字符，比如"a1b2c3d4e5f6g7h8i9j0k1l2m3n4o5p6"，这一步是为了确保只有公众号管理员才能获取 AppSecret，防止密钥被盗用。

**重要提示：**

AppSecret 只会显示一次，关闭页面后就无法再查看。所以你必须立即点击【复制】按钮将它复制到剪贴板，然后粘贴到一个安全的地方保存好（比如密码管理器或加密的文本文件）。如果你忘记保存，就需要重新生成，旧的 AppSecret 会立即失效。

步骤 4：配置 API IP 白名单

API IP 白名单是微信公众号的一项安全机制。它的作用是限制只有特定的 IP 地址才能调用你的公众号 API，即使别人获取了你的 AppID 和 AppSecret，如果他们的 IP 不在白名单中，也无法成功调用 API。

这就像你家的门锁，即使别人有钥匙（AppID 和 AppSecret），但如果他们不在允许进入的名单中（IP 白名单），门也不会打开。

如果不配置 IP 白名单，当你的 Skill 尝试调用微信公众号 API 时，会收到"IP 地址不在白名单中"的错误提示，导致 API 调用失败，Skill 无法正常工作。所以配置 IP 白名单是使用微信公众号 API 的必要步骤。

在开发密钥页面下方，找到【API IP 白名单】或【IP 白名单】选项，这一步是为了配置允许调用 API 的 IP 地址，只有在白名单中的 IP 才能成功调用微信公众号 API。

如何查看自己的公网 IP 地址？

在配置 IP 白名单之前，你需要先知道自己电脑的公网 IP 地址。这里提供几种查看方法：

**方法一：使用在线工具（最简单）**

打开浏览器，访问[https://ip.cn](https://ip.cn)或https://www.ip.cn，页面会自动显示你当前的公网IP 地址，比如"36.112.123.45"，这一步是为了快速获取你的公网 IP 地址。

Plain Text

```
https://ip.cn
https://www.ip.cn
```

**方法二：使用搜索引擎**

在百度或 Google 搜索框中输入"我的 IP"或"my ip"，搜索结果的第一条通常会直接显示你的公网 IP 地址，这一步是为了通过搜索引擎快速查询 IP 地址。

方法三：使用命令行（适合技术人员）

[在 Mac 或 Lin](http://ifconfig.me)u[x 系统中，打开终端，](http://ifconfig.me)输入命令curlifconfig.me并按回车，终端会显示你的公网 IP 地址。在 Windows 系统中，打开命令提示符（cmd），输入命令curlifconfig.me并按回车（需要先安装 curl 工具）。

**注意：**

这里获取的必须是公网 IP，不是局域网 IP。局域网 IP 通常是 192.168.x.x 或 10.x.x.x 这样的格式，这种 IP 是无法访问互联网的，也无法用于 API 白名单。

**IP 白名单配置操作**

找到【API IP 白名单】选项后，点击旁边的【修改】或【添加】按钮，这一步是为了进入 IP 白名单编辑页面。

在弹出的输入框中，输入你刚才查到的公网 IP 地址，比如"36.112.123.45"，然后点击【确定】或【保存】按钮，这一步是为了将你的 IP 地址添加到白名单中，允许这个 IP 调用 API。

系统可能会要求你进行身份验证（扫码或输入验证码），完成验证后，IP 地址就添加成功了，这一步是为了确保只有公众号管理员才能修改 IP 白名单，防止被恶意篡改。

**重要提示：**

微信公众号的 IP 白名单最多可以添加 5 个 IP 地址。如果你的 IP 地址经常变化（比如使用家庭宽带，运营商会定期更换 IP），建议使用云服务器（如阿里云、腾讯云）来运行 Skill，云服务器的 IP 地址是固定的，不会变化。

**动态 IP 的处理方案**

如果你使用的是家庭宽带或移动网络，IP 地址可能会经常变化。每次 IP 变化后，你都需要重新登录微信公众号开发者平台，更新 IP 白名单，否则 API 调用会失败。

这里提供几种解决方案：

**方案一：定期更新 IP 白名单**

如果你的 IP 变化不频繁（比如几周或几个月才变一次），可以选择每次 IP 变化后手动更新白名单。虽然麻烦一些，但成本最低。

方案二：使用动态域名解析（DDNS）

如果你有一定的技术能力，可以使用动态域名解析服务（如花生壳、Cloudflare DDNS 等），将一个固定的域名绑定到你的动态 IP 上。虽然 IP 会变化，但域名不变，可以通过域名访问你的服务。但微信公众号的 IP 白名单不支持域名，所以这个方案需要配合其他技术实现。

**方案三：使用云服务器**

购买一台云服务器（阿里云、腾讯云、AWS 等），将 Skill 部署到云服务器上运行。云服务器的 IP 地址是固定的，不会变化，只需要配置一次 IP 白名单就可以长期使用。云服务器的成本不高，最便宜的配置每月只需要几十元。

**方案四：使用代理服务器**

购买一个固定 IP 的代理服务器，让你的 Skill 通过代理服务器访问微信公众号 API。这样即使你的本地 IP 变化，代理服务器的 IP 是固定的，不需要频繁更新白名单。

（三）获取 APImart API Key

因为在 1.5 节做自动配图 ski**l**ls 的时候，我们已经用详细步骤获取了APImart API Key 了，所以这里直接使用即可，如果你没有，也可以回到 1.5 的内容，按照步骤来生成

注意：这里使用其他网站 API 也可以，只要能用 nanobanana pro 就行

将 API 密钥提供给 Claude Code

**开始创建 Skill**

当所有资料都准备好后（微信公众号 AppID 和 AppSecret、APImart API Key、Exa MCP 和 Tavily MCP 都已配置完成），我们就可以开始创建 Skill 了。

向 Claude Code 发送创建 Skill 的指令：

Plain Text

```
我感觉这个操作流程太复杂了，我们的热点来自x，24小时内容热AI内容，发布平台暂时就限制在公众号，使用公众号的API进行发布，你简化一下这个方案，整体的逻辑实现按照这个逻辑来实现“1. Exa/Tavily 搜索采集 AI 热点资料 → 2. 撰写文章（Markdown 格式）  →  3. 调用 nanobanana API 生成配图 → 4. 上传图片到微信微信服务器  → 5. 转换为 HTML 并发布到公众号草稿箱  → 6. 提示用户去微信公众号后台检查文章”
```

这一步是为了让 ClaudeCode 按照我们确定的简化方案开始创建 Skill，明确每个步骤的执行顺序和逻辑。

![](img/a80a6e24cf62651a2046939489ffd9e1.png)

Claude Code 会开始创建 Skill，这个过程可能需要 5 到 10 分钟，具体时间取决于 Skill 的复杂度和网络连接速度。

![](img/cb2e42755634364e2cf481b661328cc7.png)

![](img/135e4a14f9c16a8f739cda598ef33bf6.png)

![](img/34e9784c0dae6b86ac52e99d13f9d70d.png)

![](img/50ef2351804635318c1b97912ddf2326.png)

1.5 完成白名单添加和 Skill 测试调用

当 Claude Code 完成 Skill 创建后，我们需要进行最后的配置和测试，确保 Skill 能够正常工作。

**依赖检查**

确保系统已安装 jq 和 curl 这两个工具。如果没有安装，可以使用以下命令安装：

在 Mac 系统中：brew install jq curl

Plain Text

```
brew install jq curl
```

在 Linux 系统中（Ubuntu/Debian）：sudo apt-get install jq curl

Plain Text

```
sudo apt-get install jq curl
```

在 Windows 系统中，需要先安装 Chocolatey 包管理器，然后运行：choco install jq curl

Plain Text

```
choco install jq curl
```

这一步是为了确保 Skill 运行所需的依赖工具都已安装，jq 用于处理 JSON 数据，curl 用于发送 HTTP 请求。

**测试 Skill 功能**

现在让我们完整地测试一下 Skill 的功能，确保每个环节都能正常工作。

**步骤 1：发送测试指令**

在 Claude Code 中输入以下命令调用 Skill：@ai-wechat-publisher 写一篇关于 open claw 的文章

这一步是为了测试 Skill 的基本功能，让它自动搜索 open claw 相关的热点资讯，生成文章，配图，并发布到公众号草稿箱。

Plain Text

```
@ai-wechat-publisher 写一篇关于open claw的文章
```

Skill 会使用默认配置（技术深度风格、3 张配图、搜索 24 小时内的资讯）来生成文章。

**步骤 2：观察执行过程**

Skill 开始执行后，你会看到一系列的进度提示。

**步骤 3：检查发布结果**

当 Skill 执行完成后，登录微信公众号后台（https://mp.weixin.qq.com），进入【素材管理】-【草稿箱】，查看刚才生成的文章，这一步是为了确认文章是否成功发布到草稿箱，内容和配图是否符合预期。

![](img/f0a161b835b3d9c1186c5854a7f2ac01.png)

在草稿箱中，你会看到刚才生成的文章，包括标题、正文、配图等。点击文章可以预览效果，检查以下内容：

文章标题、文章内容、配图质量、排版格式

如果一切正常，你可以直接在后台点击【发布】按钮将文章发布到公众号。如果需要修改，可以在后台直接编辑后再发布。

**高级用法**

你也可以提供更详细的指令，自定义文章的风格、配图数量、目标受众等：

@ai-wechat-publisher 帮我搜一下最新的 GPT-5 资讯，写一篇深度分析，目标受众是开发者，生成 5 张配图，发到公众号

Plain Text

```
@ai-wechat-publisher 帮我搜一下最新的GPT-5资讯，写一篇深度分析，目标受众是开发者，生成5张配图，发到公众号
```

这一步是为了让 Skill 按照你的具体要求生成文章，包括搜索关键词、文章风格、配图数量等。

Skill 会解析你的指令，提取关键参数（搜索关键词：GPT-5，文章风格：深度分析，目标受众：开发者，配图数量：5 张），然后按照这些参数生成文章。

1.6 常见问题解答

Q1：生成的文章质量不高怎么办？

如果生成的文章质量不符合预期，可以从以下几个方面进行优化：

• **优化搜索关键词：**在调用 Skill 时提供更精确的搜索关键词，比如不要只说"写一篇 AI 文章"，而是说"写一篇关于 DeepSeek 技术突破的深度分析文章"。关键词越具体，搜索结果越精准，生成的文章质量越高。

• **调整风格指南：**编辑 Skill 的风格指南文件（style-guide.md），明确文章的写作风格、语言风格、内容深度等要求。比如可以添加"避免使用'在当今这个时代'、'随着科技的发展'等套话"、"每个观点都要有数据或案例支撑"等具体要求。

• **增加搜索结果数量：**在配置文件中将 max_results 从 10 增加到 20 或 30，让 Skill 获取更多的搜索结果，有更多的素材可以选择。但要注意，搜索结果越多，成本越高，处理时间也越长。

• **使用更高质量的搜索源：**如果 Exa 和 Tavily 的搜索结果质量不够高，可以考虑添加其他搜索源，比如 Google Scholar（学术搜索）、Hacker News（技术社区）、Reddit（讨论社区）等。

• **人工审核和修改：**即使是 AI 生成的文章，也建议进行人工审核和修改。在发布前检查文章的逻辑、语言、事实准确性等，必要时进行修改和润色。这样可以确保发布的内容质量始终保持在高水平中

**Q2：常见错误和解决方案**

• **提示"IP 地址不在白名单中"：**查看你当前的公网 IP 地址（访问 https://ip.cn），更新 IP 白名单

• **提示"APImart API Key 无效"：**检查 API Key 是否正确复制（没有多余的空格或换行），确认 API Key 是否有效

• **提示"余额不足"：**去后台，看一下账户余额是否够，如果余额不足，进行充值

• **提示"文章生成失败"：**查看日志文件，了解具体的错误原因，尝试重新运行 Skill

• **提示"图片上传失败"：**检查生成的图片是否有效（文件大小、格式等），检查网络连接是否稳定

**Q3：API 调用成本**

**Exa/Tavily API：**

按搜索次数计费，约每次搜索 0.01 到 0.05 美元，如果每天生成 1 篇文章，每篇文章搜索 1 次，月成本约 0.30 到 1.50 美元。

**APImart API**

（gemini-3-pro-image-preview）：每次生成 0.05 美元（生成 3 张图片），如果每天生成 1 篇文章，每篇文章 3 张配图，月成本约 1.50 美元。

**微信公众号 API**

：免费（微信公众号 API 不收费）。

![](img/f524ffc87cf9c5d4201b26d6ab8674fe.png)

2.小红书自动生成与发布 Skills

小红书作为国内最活跃的内容社区之一，是很多创作者和品牌的重要阵地。但每天手动创作小红书内容、配图、发布，工作量非常大。有了 Claude Code 之后，我们可以实现从内容创作到发布的全自动化流程。

完成这个案例的搭建后，你会掌握如何让 Claude Code 自动生成小红书风格的内容、调用 AI 生成配图、通过 Cookie 认证自动发布到小红书平台的完整流程。

这个案例会用到 GitHub 上的开源项目，涉及 MCP 插件安装、Skill 安装、Claude SDK 的使用，以及 Cookie 认证配置，相对来说有一定的技术含量，但按照步骤操作，你也能一步一步搭建出来。

预计完成时间是 40 到 60 分钟。

**注意：本案例难度较大，大家可以在公众号和小红书里只选择一个案例完成即可（新手推荐**公众号案例），不需要全部都完成，21 天里，完成一个 Skills 案例即为收获

2.1 安装小红书 MCP 插件

💡在开始之前，我们需要先安装 xiaohongshu-mcp 这个插件。MCP 是 Claude Code 的插件系统，可以让 Claude Code 具备更多的能力，比如访问小红书平台、发布内容等。

关于 xiaohongshu-mcp

xiaohongshu-mcp 是一个专门为 Claude Code 开发的小红书平台集成插件，它可以让 Claude Code 直接与小红书平台进行交互。通过这个 MCP，Claude Code 可以获取你的小红书账号信息、发布笔记、上传图片、管理草稿等操作。这个插件是开源的，由社区开发者维护，代码托管在 GitHub 上。

使用 xiaohongshu-mcp 的好处是可以实现完全自动化的内容发布，不需要手动登录小红书网页或 APP，支持批量操作和定时发布，可以与其他 MCP 和 Skill 配合使用，打造完整的内容生产流水线。

步骤 1：打开 Claude Code 的对话界面

先启动 Claude Code，确保你的网络连接正常，这一步是为了让 Claude Code 能够访问 GitHub 并下载 MCP 插件。

步骤 2：向 Claude Code 发送安装指令

在对话框中输入以下内容：

[请帮我安装 xiaohongshu-mcp，项目](https://github.com/xpzouying/xiaohongshu-mcp)地址是https://github.com/xpzouying/xiaohongshu-mcp

Plain Text

```
请帮我安装xiaohongshu-mcp,项目地址是https://github.com/xpzouying/xiaohongshu-mcp
```

这一步是为了让 Claude Code 自动从 GitHub 克隆项目代码，解析项目结构，安装必要的依赖，并将 MCP 注册到系统中。

![](img/7bd32ae3adbf0d39c071d880c4e489e8.png)

**步骤 3：等待安装完成**

Claude Code 会自动执行安装过程，这个过程通常需要 2 到 5 分钟，具体时间取决于网络速度和项目大小，这一步是为了让系统完成所有必要的配置和依赖安装。

当你看到安装成功的提示信息时，说明 xiaohongshu-mcp 已经可以使用了。

![](img/77030fc74b5959b82bfbc6a03815f899.png)

2.2 安装智能内容创作 Skill

💡安装完 xiaohongshu-mcp 后，我们还需要安装 smart-content-creator-skill 这个 Skill。这个 Skill 专门用于生成小红书风格的内容，包括标题、正文、话题标签等。

关于 smart-content-creator-skill

smart-content-creator-skill 是一个专门为小红书内容创作优化的 Skill，它内置了小红书平台的内容规范和风格指南。这个 Skill 可以根据你提供的主题或关键词，自动生成符合小红书风格的内容，包括吸引人的标题、结构化的正文、合适的 emoji 表情、热门话题标签等。

使用这个 Skill 的好处是生成的内容更符合小红书用户的阅读习惯，标题更有吸引力，容易获得更多曝光，内容结构清晰，易读性强，自动添加合适的话题标签，提高内容被发现的概率。

步骤 1：向 Claude Code 发送安装指令

把这个 GitHub 开源的项目丢给 cc，让它自动帮我们安装这个 skill

在 Claude Code 的对话框中输入：

请帮我安装 smart-content[-](https://github.com/ginobefun/smart-content-creator-skill)creator-skill，项目地址是https://github.com/ginobefun/smart-content-creator-skill

Plain Text

```
请帮我安装smart-content-creator-skill,项目地址是https://github.com/ginobefun/smart-content-creator-skill
```

这一步是为了让 Claude Code 从 GitHub 下载 Skill 代码，解析 Skill 的配置文件，安装到本地的 Skills 目录中。

![](img/f4bce84d24b345cd60d059459c76836c.png)

**安**装的时候，因为使用 AI 不同，所以可能会出现回答不一样，根据 AI 的回答多尝试几次就行，如果不理解，就多问问 AI。

**步骤 2：等待安装完成**

Claude Code 会自动完成安装，这个过程通常需要 1 到 3 分钟，这一步是为了让系统完成 Skill 的注册和配置。

![](img/a0eec2ad2c77459ecc9c21040bf266a0.png)

步骤 3：验证 Skill 是否安装成功

安装完成后，你可以在 Claude Code 中输入命令查看 Skill 列表：

Plain Text

```
/skills list
```

这一步是为了确认 smart-content-creator-skill 已经成功安装并出现在可用的 Skill 列表中。

如果你是在 VS Code 插件使用 Claude Code，那么这个命令应该是不会有任何显示的结果，可以直接使用提示词。

提示词如下：

列举下现在可以用的skills列表

![](img/586571811e55a3ad8a76028a1f4ef8ca.png)

2.3 使用 Claude SDK 连接功能

💡现在我们已经有了 xiaohongshu-mcp 和 smart-content-creator-skill 这两个组件，但它们还需要通过 Claude SDK 连接起来，才能实现完整的自动化流程。

关于 Claude Agent SDK

Claude Agent SDK 是 Anthropic 官方提供的 Python 开发工具包，它可以让开发者更方便地调用 Claude 的能力，并将多个工具和服务连接起来。通过这个 SDK，我们可以编写自动化脚本，让 Claude Code 按照预定的流程执行任务。

在这个案例中，Claude SDK 的作用是连接 smart-content-creator-skill 和 xiaohongshu-mcp，让内容生成和发布形成一个完整的自动化流水线。具体来说，SDK 会先调用 smart-content-creator-skill 生成小红书内容，然后调用 xiaohongshu-mcp 将内容发布到小红书平台，整个过程无需人工干预。

步骤一：安装 Claude SDK

第一，确认 Python 环境。

先确保你的电脑上已经安装了 Python 3.8 或更高版本，可以在终端中输入以下命令检查：

Bash

```
python --version
```

**这一步是为了确认系统环境满足 Claude SD**K 的运行要求，如果你的电脑没有符合要求的 Python 环境，可以让 Claude code 帮你安装

第二，向 Claude Code 发送安装指令。

把这个 GitHub 的项目丢给 Claude Code，让它自动帮我们安装这个 sdk，在 Claude Code 中输入：

Plain Text

```
请帮我安装Claude Agent SDK,项目地址是https://github.com/anthropics/claude-agent-sdk-python
```

![](img/3348563cd739154b44eb08ac5497d1c6.png)

这一步是为了让 Claude Code 自动安装 SDK 及其依赖包。

**第三，等待安装完成。**

安装过程通常需要 3 到 5 分钟，这一步是为了让系统下载并配置所有必要的 Python 包。

SDK 需要配置 API Key，如果配置我们之前的 skill 配置的时候已经设置过 API key 和 base url 可以和 Claude code 说帮我复用当前的 API key 和 base url就可以了。

也可以重新获取 API Key 和 base url，具体获取方式参考这部分：

获取API key和base URL跳转地址链接

[如果你要配置其他 API key，比如 kimi，](https://login.moonshot.cn/?source=https%3A%2F%2Fplatform.moonshot.cn%2Fredirect%3Fpath%3D%2Fconsole%2Fapi-keys%26&appid=dev-workbench&code_challenge=ytHnOEgm7H-UtAtHnCUSrLlolTRc30Q6Gr87NW7O6dk&code_challenge_method=S256)可以去官网获取（https://platform.moonshot.cn/console/api-keys），然后发给 Claude code

![](img/25afa3f07c0764a8d5860bbbeef16043.png)

**步骤二：配置自动化流程**

第一，让 Claude Code 创建连接脚本。

向 Claude Code 发送以下指令：

Plain Text

```
请帮我创建一个自动化脚本,使用Claude SDK连接smart-content-creator-skill和xiaohongshu-mcp,实现从内容生成到发布的完整流程。
```

![](img/3c67eca68808aab6ab3a86fa54041d2c.png)

这一步是为了让 Claude Code 自动编写连接代码，处理两个组件之间的数据传递和流程控制。

![](img/e54055b65c18daffd88855b92d096fc1.png)

**第二，查看生成的脚本。**

Claude Code 会生成一个 Python 脚本文件，通常保存在当前工作目录下，这一步是为了让你了解自动化流程的具体实现逻辑。

![](img/55b4d0e44881e7305e1cb84d33f0d69d.png)

**第三，若报错用 AI 解决**

可以先进行一次测试运行，确保脚本能够正常工作，这一步是为了在正式使用前发现并解决潜在的问题。

在终端中切换到脚本所在目录 cd /path/to/your/script

Plain Text

```
cd /path/to/your/script
```

[运行测试命令 pyt](http://publish.py)hon3 xiaohongshu_auto_publish.py

Plain Text

```
python3 xiaohongshu_auto_publish.py
```

观察输出结果，如果看到类似这样的输出，说明脚本正常：

✓ 连接 smart-content-creator-skill 成功

✓ 连接 xiaohongshu-mcp 成功

✓ 测试运行完成

![](img/a7904bb93b732e7a4ee496d7e9f39cf4.png)

如果发现报错，直接截图把错误丢给 AI，来回多沟通几遍。

**多次沟通调试的流程：**

第 1 次：运行脚本 → 出现错误 → 截图发给 Claude Code

第 2 次：Claude Code 修复 → 重新运行 → 可能还有错误 → 再次截图发给 Claude Code

第 3 次：Claude Code 再次修复 → 重新运行 → 成功

![](img/6a1eb43d0ca3606c36d31981a277b923.png)

2.4 获取小红书 Cookie

💡要让 Claude Code 能够自动发布内容到小红书，需要提供你的小红书账号认证信息。小红书使用 Cookie 来验证用户身份，所以我们需要从浏览器中获取 Cookie 并配置到 xiaohongshu-mcp 中。

**关于 Cookie 认证**

Cookie 是网站用来识别用户身份的一种技术。当你在浏览器中登录小红书后，小红书会在你的浏览器中存储一个 Cookie，后续的所有操作都会携带这个 Cookie 来证明你的身份。xiaohongshu-mcp 通过使用你的 Cookie，可以模拟浏览器的行为，以你的身份发布内容。

需要注意的是，Cookie 是你的账号凭证，相当于密码，一定要妥善保管，不要泄露给他人。Cookie 通常有有效期，过期后需要重新获取。

步骤一：获取小红书 Cookie

![](img/8244e5453edee1384e2ff2d6e1367636.png)

**首先，打开小红书网页版并登录。**

先打开浏览器（建议使用 Chrome 或 Edge），访问https://www.xiaohongshu.com，点击页面右上角的【登录】按钮，使用扫码或手机号完成登录，这一步是为了让浏览器获取你的登录 Cookie

**然后，打开开发者工具。**

登录成功后，按下键盘上的【F12】键（Mac 用户按【Command + Option + I】），打开浏览器的开发者工具，这一步是为了查看网络请求中的 Cookie 信息。

或者是点击右键，选择【检查】，也可以进入到开发者工具页面

![](img/38620b4cfe8624a2866feb4a1dad32e2.png)

接着，切换到 Network（网络）标签。

在开发者工具的顶部菜单中找到并点击【Network】标签（中文浏览器可能显示为【网络】），这一步是为了查看浏览器发送的所有网络请求。

![](img/1d8f6b5c6a9c3dcd0ccf7baba764c97e.png)

**下一步，刷新页面触发请求。**

按【F5】键或点击浏览器的刷新按钮，让页面重新加载，这一步是为了在 Network 标签中捕获新的网络请求。

然后，在 Network 标签的请求列表中。

点击任意一个发送到[xiaohongshu.com](http://xiaohongshu.com)的请求（通常选择第一个），这一步是为了查看该请求携带的 Cookie 信息。

![](img/49fbaebb86d80f65ae4e5045ea35dcae.png)

最后，查看并复制 Cookie。

在右侧的请求详情中，找到【Headers】（请求头）部分，向下滚动找到【Request Headers】（请求标头），在其中找到【cookie:】这一行，这一步是为了找到完整的 Cookie 字符串。

点击 cookie 后面的值，全选并复制（通常是一长串包含多个键值对的字符串，类似：web_session=xxx； xsecappid=xxx; a1=xxx;...），这一步是为了获取完整的 Cookie 认证信息。

![](img/74206da596c5943c197f2b0154ba0f31.png)

步骤二：配置 Cookie 到 MCP

**我们直接让 Claude **Code 来配置Cookie 到 MCP。

首先，向 Claude Code 发送配置指令。

在 Claude Code 中输入：

Plain Text

```
请帮我配置xiaohongshu-mcp的Cookie。我的Cookie是：[粘贴你刚才复制的完整Cookie字符串]
```

这一步是为了让 Claude Code 自动找到配置文件并写入 Cookie 信息。

然后，等待 Claude Code 完成配置。

Claude Code 会自动执行以下操作：

• 定位 xiaohongshu-mcp 的配置文件（通常在 ～/。config/claude/mcp_config.json

或类似位置）

• 在配置文件中找到 xiaohongshu-mcp 的配置项

• 将 Cookie 信息写入配置

• 保存文件

这个过程通常需要 10 到 30 秒。

**最后，确认配置成功。**

Claude Code 会提示你：

✓ Cookie 配置成功

✓ xiaohongshu-mcp 已更新配置

**安全提醒**

关于 Cookie 安全，不要将 Cookie 分享给任何人，不要将包含 Cookie 的配置文件上传到公开的代码仓库，定期更换 Cookie（建议每个月重新获取一次），如果怀疑 Cookie 泄露，立即在小红书 APP 中退出登录，这会使所有 Cookie 失效。

关于账号安全，建议使用小号进行测试，避免主账号出现问题，不要使用自动化工具进行违规操作，遵守小红书的社区规范，注意发布频率，避免被平台识别为机器人行为。

![](img/4e15c162205cbea35991fb3e692d3729.png)

**2.5 测试与发布**

现在所有的准备工作都完成了，我们可以开始测试整个自动化流程，看看能否成功生成并发布小红书内容。

**步骤一：测试内容生成**

**首先，发送测试指令。**

在 Claude Code 中输入测试指令，比如：

Plain Text

```
@smart-content-creator-skill 帮我生成一篇关于春季护肤的小红书笔记
```

这一步是为了测试 smart-content-creator-skill 是否能够正常生成小红书风格的内容。

**然后，查看生成结果。**

Skill 会生成包含标题、正文、话题标签的完整内容，检查内容是否符合小红书的风格，标题是否吸引人，话题标签是否合适，这一步是为了确认内容生成功能正常工作。

**步骤二：测试自动发布**

**首先，发送发布指令。**

在 Claude Code 中输入：

Plain Text

```
请使用xiaohongshu-mcp将刚才生成的内容发布到小红书
```

这一步是为了测试 xiaohongshu-mcp 是否能够成功调用小红书 API 发布内容。

**然后，观察发布过程。**

Claude Code 会显示发布的进度信息，包括上传图片、创建笔记、发布成功等步骤，这一步是为了了解整个发布流程是否顺利。

**最后，验证发布结果。**

打开小红书 APP 或网页版，进入你的个人主页，查看刚才发布的笔记是否出现，检查内容、图片、话题标签是否正确，这一步是为了确认内容已经成功发布到小红书平台。

**步骤三：使用完整自动化流程**

当单独测试都通过后，就可以使用完整的自动化流程了。

**首先，发送一键生成发布指令。**

在 Claude Code 中输入：

Plain Text

```
请帮我生成一篇关于【你的主题】的小红书笔记并自动发布
```

这一步是为了触发完整的自动化流程，从内容生成到发布一气呵成。

**然后：等待流程完成。**

整个流程通常需要 2 到 5 分钟，具体时间取决于内容长度、图片数量、网络速度，这一步是为了让系统完成所有操作。

**最后，查看最终结果。**

流程完成后，Claude Code 会提示发布成功，并提供笔记链接，你可以直接点击链接查看发布的内容，这一步是为了确认整个自动化流程运行正常。

![](img/9d5c7f576643667ca4202a608e5c8532.png)

💡

**拓展玩法**

有能力的伙伴，可以自行探索一下，让 Claude code 设置好定时发布，从而实现每天定时自动发布**定时自动发布的完整配置步骤：**步骤一：创建定时发布脚本

在 Claude Code 中输入：

请帮我创建一个定时发布脚本，每天上午 10 点自动生成一篇小红书笔记并发布

这一步是为了让 Claude Code 生成一个包含定时任务的脚本。

步[骤二：配置定时任务*](http://publish.py)[*Mac/Linux](http://publish.py) 用户使用 cron：在终端输入：crontab -e

在打开的编辑器中添加一行：0 10 ** cd /path/to/your/project && python3 xiaohongshu_auto_*publish.py保存并退出（按【Esc】，输入 :wq，按【Enter】）**Windows 用户使用任务计划程序：**按【Win + R】，输入 taskschd.msc，按【Enter】打开任务计划程序

点击右侧的【创建基本任务】

输入任务名称（如"小红书自动发布"），点击【下一步】

选择【每天】，点击【下一步】

设置开始时间为上午 10:00，点击【下一步】

选择【启动程序】，点击【下一步】

在"程序或脚本"中输入：python3（或 python）

在"添加参数"中输入：xiaohongshu_auto_publish.py在"起始于"中输入：你的项目文件夹路径（如

C:\Users\YourName\xiaohongshu-project）

点击【完成】

**步骤三：测试定时任务**Mac**/Linux 测试方法：运**行后等第二天看有没有自动发布Windo**ws 测试方法：在任务计划程序中，右键点击刚才创建的任务，选择【运行】，立即测试是否能正常执行注意：电脑必须保持开机：**定时任务只有在电脑开机状态下才会执行

**2.6 常见问题解答**

Q1:为什么要使用 Cookie 认证而不是账号密码？

小红书的 API 不支持直接使用账号密码登录，而是使用 Cookie 来验证用户身份。Cookie 认证更安全，因为 Cookie 有有效期，即使泄露也会自动失效。同时 Cookie 认证不需要在代码中存储明文密码，降低了安全风险。

Q2:Cookie 多久会过期？过期后怎么办？

小红书的 Cookie 通常有效期为 30 到 90 天，具体时间取决于平台设置。当 Cookie 过期后，xiaohongshu-mcp 会提示认证失败，这时需要重新登录小红书网页版，按照前面的步骤重新获取 Cookie 并更新配置文件。建议定期（比如每个月）主动更新一次 Cookie，避免在使用时突然失效。

Q3:自动发布会不会被小红书封号？

如果你遵守小红书的社区规范，发布合规内容，一般不会被封号。但需要注意以下几点：不要发布违规内容（广告、虚假信息等），控制发布频率，避免短时间内大量发布，内容要有原创性，避免重复发布相同内容，不要使用多个账号发布完全相同的内容。建议先用小号测试，确认流程稳定后再用主账号。

Q4:可以同时管理多个小红书账号吗？

可以。你可以为每个账号分别获取 Cookie，在配置文件中添加多个账号的配置，使用时指定要使用哪个账号发布。但需要注意不同账号要使用不同的内容，避免被平台识别为批量操作。同时要注意遵守平台规则，不要进行恶意营销或刷量行为。

Q5:生成的内容可以自定义风格吗？

可以。smart-content-creator-skill 支持自定义内容风格，你可以在调用时指定风格要求，比如"生成一篇专业严谨风格的笔记"或"生成一篇轻松活泼风格的笔记"。也可以修改 Skill 的配置文件，设置默认的风格参数。如果对生成的内容不满意，可以多次生成并选择最好的一篇，或者在生成后手动修改再发布

### 03.进阶：AI 视频创作 Skills

1.小说改编漫剧剧本 Skills

**重点必看：进阶篇只需要完成一个 Skills 案例实操即可，我**们是在案例中掌握 Skills 的用法；

**在进**阶篇中，第一个难度低于第二个，建议新手先把小说改编漫剧剧本的 Skills 做出来，然后就可以进入到 Open claw 的学习了，通过这一个案例，加深对于 Skills 的运用；

**用起来在实操过程中，遇到的任何问题都可以截**图丢给 Claude code，帮你解决

网络小说 IP 改编成短视频漫剧是当下非常火爆的内容形式。传统的改编流程需要专业编剧团队，耗时长、成本高。有了 Claude Code 之后，我们可以实现从小说原文到漫剧剧本的自动化改编，包括剧情拆解、冲突提取、分集标注、剧本创作的全流程。

完成这个案例的搭建后，你会掌握如何让 Claude Code 自动分析小说原文、提取核心冲突点和情绪钩子、按照漫剧节奏进行分集、生成 500 到 800 字的视觉化剧本的完整流程。这个案例涉及复杂的 Skill 配置、多个 Agent 协作、模板和示例文件的使用，是一个比较复杂的一个案例，但相信大家按照步骤操作，配合 AI，也能够把这个案例搭建出来**（版权、二创、人工审核，这部分如果真拿去商用，风险不小）**

推荐先把小说二创后，再去生成，降低风险

![](img/77bb66f3d849702fef8ca9e776d11de2.png)

剧本.mp4【在线播放】

![](img/bacbfe275302ddd991325763e322b01f.png)

**1.1 完整工作流程**

**阶段 1：剧情拆解（当前阶段）**

Plain Text

```
📖 上传小说原文（每5章一批）
↓🔍 输入 /breakdown 开始拆解
↓⚙️ 调用 webnovel-skill 提取剧情点
↓✓  novelsame-agent 自动检查一致
↓💾 保存到 check-down.md
↓📊 标注分集（第X集）+ 状态（未用）
```

输出示例：

Plain Text

```
第1集：
剧情点1：主角被欺辱，激发复仇欲望（冲突强度：8/10）
剧情点2：意外获得神秘玄典（情绪钩子：惊喜+期待）
状态：未用
```

**阶段 2：单集剧本创作**

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

**1.2 下载并准备项目**

💡在开始之前，我们需要先下载一个完整的项目模板。这个项目已经包含了所有必要的配置文件、模板文件和示例文件，我们只需要下载下来，稍作配置就可以使用。

关于这个项目

这**是一个专门为网文改编漫剧设计**的完整工作流项目，它包含了从小说原文到漫剧剧本的全套自动化工具。项目的核心是一个名为webnovel-skill的 Skill，它内置了专业的改编方法论，可以自动识别小说类型、提取冲突点、标注情绪钩子、进行分集规划、生成视觉化剧本。

使用这个项目的好处是不需要从零开始配置，所有的改编规则、输出格式、质量标准都已经预设好，可以直接使用。项目还包含了两个质量检查 Agent，可以自动检查拆解质量和剧本一致性，确保输出的剧本符合漫剧制作标准。

将下方的安装包解压到一个你容易找到的位置，比如桌面或文档文件夹，这一步是为了方便后续在 Claude Code 中打开这个项目。

[

![](img/2b18a427dc9a4a261ffb09639b42d0e4.png)

test.zip](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/CvKHbuPfroLk1OxTd7bcY2NHndc?response-content-disposition=attachment%3B%20filename%3D%22test.zip%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260526%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260526T190327Z&x-oss-expires=86400&x-oss-signature=ee64990e443e57737f498a0c054d085006b9050437682490d5f1b807c812058a&x-oss-signature-version=OSS4-HMAC-SHA256)

解压后你会看到以下文件结构：

这个结构看起来很复杂，但实际使用时你只需要关注 novel 文件夹（放小说）和 scripts 文件夹（查看生成的剧本）就可以了，其他文件都是自动工作的。

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

1.3**准备小说素材**

下载好项目后，我们需要准备要改编的小说原文。这个项目支持任何类型的网络小说，包括玄幻、武侠、都市、言情、悬疑、科幻等。

小说文件需要是 txt 格式的纯文本文件，每一章保存为单独的文件，文件命名建议使用 chapter-001.txt、chapter-002.txt 这样的格式，方便系统按顺序读取。

如果你有自己的小说素材，也可以按照自己的素材来，这里给大家提供了一本小说素材，大家只需要下载即可

[

![](img/58e0482e90fc815bba7b8faff5ebc3e1.png)

novel.zip](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/UNdLb4J4Go01PBxxWqycLTIjn1e?response-content-disposition=attachment%3B%20filename%3D%22novel.zip%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260526%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260526T190327Z&x-oss-expires=86400&x-oss-signature=ced8b1011c6641b313fda4013f61705b5f45ea4c1e3d2898e547d5a21830d1e8&x-oss-signature-version=OSS4-HMAC-SHA256)

![](img/44facc8f2d3a0530b23ac7202058021c.png)

![](img/2a4969d10843d5dcd4dc70ab896ba4f0.png)

**1.4 进行剧情拆解**

准备好小说文件后，我们就可以开始进行剧情拆解了。剧情拆解是整个改编流程的第一步，也是最关键的一步，它决定了后续剧本的质量。

关于剧情拆解：剧情拆解的核心工作是从小说原文中提取核心冲突点和情绪钩子。核心冲突点是推动剧情发展的关键事件，比如主角被欺辱、获得金手指、与敌人对决等。情绪钩子是能够引发观众强烈情绪反应的时刻，比如打脸爽点、虐心痛点、真相揭露等。

这个项目使用的改编方法论会自动识别小说类型（玄幻、都市、言情等），然后根据类型特点提取相应的冲突和钩子。比如玄幻类小说会重点提取境界突破、越级碾压的情节，言情类小说会重点提取误会产生、虐心痛苦的情节。

拆解完成后，系统还会自动进行分集标注，将提取的剧情点按照漫剧节奏分配到各集，确保每集都有足够的冲突密度和情绪强度。

步骤 1：启动 Claude Code 项目

首先，先打开终端或命令行工具

![](img/1fd9992a76f3091a12756a4d561111f9.png)

启动claude code.mp4【在线播放】

![](img/1881da5c6772bc97833de6aa4ee35797.png)

直接在目录下 cmd 启动 Claude Code

Claude Code 会自动识别。claude 文件夹中的配置，你会看到项目相关的提示信息，这一步是为了确认项目配置已经正确加载。

**如果这里出现了报错，可以把报错截图直接发给 Claude **code，让 AI 帮你分析哪里出问题了

![](img/e95261dd93c795e7555ae98a40bbcfbf.png)

![](img/52aa630c2e72b62035706a1e18b1bc9a.png)

![](img/3d10ebd085acf8cc43282a02116f5a75.png)

步骤 2：告诉 Claude Code 小说名称和类型

现在 Claude Code 已经启动并加载了项目配置，我们需要告诉它要改编的小说信息。

**这里不要忘**记了把前面的压缩包的小说解压后放到novel的目录下面

![](img/f9fa2208d1a01c0b976a5cd3a3a33b8b.png)

在 Claude Code 的对话界面中输入小说的基本信息，比如：我要改编一部小说，名字是《天逆玄典》，类型是玄幻，这一步是为了让 Claude Code 了解你要改编的小说，并根据类型选择相应的改编策略。

Plain Text

```

我要改编一部小说，名字是《天逆玄典》，类型是玄幻
```

Claude Code 会确认小说信息，并询问你是否准备好开始拆解，这一步是为了确保所有准备工作都已完成。

**P**S：注意，你的截图和下方不一样很正常，只要出现想要的内容即可往下走，如果遇到问题直接截图问 Claude code 即可

![](img/db9d4d6f811ac1631563cdd18d6462f5.png)

![](img/b3c27b49c48c215bdc229c864ad410b4.png)

![](img/7194544a70959f6131dc3df1d81ded70.png)

步骤 3：让 Claude Code 执行拆解命令

在 Claude Code 中输入命令：/breakdown，这一步是为了触发剧情拆解流程，让 webnovel-skill 开始工作。也可以输入汉字：“拆解剧情”

Plain Text

```
breakdown
```

注意，这里直接输入的就是一个 breakdown 的提示词，就可以触发。

前面加了斜杠，可能会和 Claude Code 的自定义命令功能冲突，会提示你找不到命令的错误提示。

然后，Claude Code 会询问你是手动指定章节还是自动扫描 novel 文件夹，因为我们的章节文件命名规范（chapter-001.txt 这样的格式），所以直接输入scan 让系统自动扫描，这一步是为了让系统知道要处理哪些章节。

Plain Text

```
scan
```

注意，这里直接输入的就是一个 breakdown 的提示词，就可以触发。

前面加了斜杠，可能会和 Claude Code 的自定义命令功能冲突，会提示你找不到命令的错误提示。

![](img/2fe4fbd5c8a36ce1b626daa072022c45.png)

系统会开始读取小说原文，提取冲突点和情绪钩子，标注分集信息，这个过程通常需要 3 到 5 分钟，具体时间取决于章节数量和内容长度，这一步是为了让 AI 完成复杂的分析和提取工作。

**步骤 4:查看拆解结果**

当你看到"完成！我已经完成了第 1 到 6 章的剧情拆解和分集标注"这样的提示时，说明拆解已经完成，这一步是为了确认第一批次的拆解工作已经结束。

![](img/d9ac0669cad3079d15b6467f1d4aee6f.png)

打开项目目录中的[breakdown.md](http://breakdown.md)文件，你会看到类似这样的内容：这一步是为了确认拆解结果是否符合预期，每个剧情点是否清晰，分集是否合理。

系统会自动调用 novelquality-agent 进行质量检查，检查冲突提取是否准确、情绪钩子密度是否达标、分集标注是否合理，如果检查通过，会显示 PASS 状态，如果有问题，会显示具体的修改建议，这一步是为了确保拆解质量符合专业标准。

**步骤 5:继续拆解更多章节**

如果你的小说有更多章节，可以继续输入/breakdown 命令，系统会自动处理下一批次的章节，这一步是为了完成整部小说的剧情拆解。

![](img/8e3d54be0be3f5aa0ceb6e31cb4d8781.png)

1.5**创作单集剧本**

完成剧情拆解后，我们就可以开始创作单集剧本了。单集剧本是可以直接用于漫剧制作的脚本，包含场景描述、角色动作、对话、特效标注等内容。

关于剧本创作：剧本创作的核心是将拆解出的剧情点转化为视觉化[的脚本。这个过程会自动完](http://breakdown.md)成以下工作：读取breakdown.md中标记为"未用"的剧情点，根据剧情点生成 500 到 800 字的剧本，使用视觉化语言描述场景和动作，添加特效标注和卡黑结尾，保存到 scripts 文件夹中，更新剧情点状态为"已用"。

生成的剧本会严格遵循漫剧的节奏要求，确保每集都有足够的冲突密度和爽点，适合短视频平台的观看习惯。

**步骤 1：执行创作命令**

首先，在 Claude Code 中输入命令：create，这一步是为了触发剧本创作流程，让 webnovel-skill 开始生成剧本。

Plain Text

```
create
```

注意，这里直接输入的就是一个 breakdown 的提示词，就可以触发。

前面加了斜杠，可能会和 Claude Code 的自定义命令功能冲突，会提示你找不到命令的错误提示。

然后，Claude Code 会询问你要创作哪几集的剧本，你可以选择创作第 1 集，或者批量创作第 1 到 6 集，这一步是为了让系统知道要生成多少集剧本。

系统会依次读取每一集的剧情点，生成对应的剧本，这个过程通常需要每集 2 到 3 分钟，这一步是为了让 AI 完成剧本的创作工作。

![](img/45813630649808abaadd2ef23cd975dc.png)

**步骤 2:查看剧本输出**

当你看到"第 1 集剧本已完成"这样的提示时，说明该集剧本已经生成，这一步是为了确认剧本创作已经结束。

[进入项目目录中的 scr](http://Episode-1.md)i[pts 文件夹，你会看到](http://Episode-2.md)生成的剧本文件，比如Episode-1.md、Episode-2.md等，这一步是为了查看生成的剧本内容。

![](img/38dd62d348182f4b5b47cb9dd448b110.png)

打开任意一个剧本文件，你会看到 AI 生成的内容，这一步是为了确认剧本格式是否符合漫剧制作要求，场景、动作、特效标注是否清晰。

同时，系统会自动调用 novelsame-a[gent 进行一致性检查](http://breakdown.md)，确保剧本内容与breakdown.md中的剧情点一致，没有偏离原定方向，这一步是为了确保剧本质量符合标准。

1.6**理解背后的配置逻辑**

到这里，你已经完成了从小说到剧本的完整改编流程。但你可能会好奇：为什么输入 /breakdown 就能自动拆解？为什么 Agent 会自动检查质量？这些都是怎么实现的？

**配置文件的作用**

在。claude/文件夹中，有几个核心配置文件，它们共同定义了整个改编流程：

[CLAUDE.md](http://CLAUDE.md)**的作用：**[CLAUDE.md](http://CLAUDE.md)是整个项目的总调度中心，它定义了主 Agent 的角色和工作流程，也就是**"什么时候做什么"**

这个文件告诉 Claude Code：

+   当收到/breakdown 命令时 → 执行剧情拆解流程

+   当收到/create 命令时 → 执行剧本创作流程

+   拆解完成后 → 自动调用 novelquality-agent 检查质量

+   剧本完成后 → 自动调用 novelsame-agent 检查一致性

通过这个文件，Claude Code 知道自己在这个项目中扮演的是编剧角色，负责调用 webnovel-skill 执行专业改编，调用双校验 Agent 做质检，整个生产流程都固化在这个文件中。

[skill.md](http://skill.md)**的作用：**[skill.md](http://skill.md)是 webnovel-skill 的本体文件，它定义了这个 Skill 到底会干什么。

这个文件规定了 Skill 的能力范围，包括类型识别（识别小说是玄幻、都市还是言情），剧情拆解（提取冲突点和情绪钩子），分集标注（按照漫剧节奏分配剧情点），单集剧本创作（生成 500 到 800 字的视觉化剧本），内容修订（根据反馈优化剧本）。

同时还规定了每个阶段要读哪些文件，用什么模板，参考哪些示例，确保 Skill 的工作流程清晰可控

[adapt-method.md](http://adapt-method.md)**的作用：**[adapt-method.md](http://adapt-method.md)是改编方法论文件，它只管一件事：改编这件事本身应该怎么做。

这个文件定义了整套改编科学，包括冲突识别（如何判断核心冲突、次级冲突、过渡冲突），钩子提取（如何识别打脸蓄力、碾压爽点、金手指觉醒等情绪钩子），密度压缩（如何将小说内容压缩到漫剧节奏），分集策略（如何合理分配剧情点到各集），节奏公式（如何确保每集都有足够的冲突和爽点）。

[output-style.md](http://output-style.md)**的作用：**[output-style.md](http://output-style.md)专门规定 AI 输出内容"长什么样"，它不管剧情对不对，只管写出来有没有画面感、节奏够不够快、爽点够不够密、能不能直接拍成漫剧。

这个文件规定了场景标识（使用※符号），动作标识（使用△符号），特效标识（使用【特效】标记），卡黑结尾（每集结尾必须有悬念），对话格式（简短有力，不超过 20 字），确保生成的剧本可以直接用于漫剧制作。

**示例和模板文件**

examples 文件夹中包含两个示例文件：

• plot-breakdown-example.md 展示了如何写剧情点，如何标注集数，如何标注情绪钩子，如何管理状态，AI 会直接模仿这个结构输出。

• script-example.md 展示了场景如何写、动作如何标注、特效怎么加、如何卡黑，这是 AI 学习视觉语言的模板。

templates 文件夹中包含两个模板文件：

• plot-breakdown-template.md 规定了剧情拆解的固定格式，确保拆解结构统一。

• script-template.md 规定了剧本的固定结构，保证每集都是可制作脚本。

**为什么要这样设计？**

因为这样可以让你轻松定制。比如：

• 如果你想修改改编方法，只需要改 adapt-method.md

• 如果你想修改剧本格式，只需要改 output-style.md

• 如果你想增加新命令，只需要改 CLAUDE.md

所有配置都是独立的，互不影响，易于维护和复用。

1.7**常见问题解答**

Q1：为什么要把小说拆分成多个章节文件？

因为 Claude Code 处理单个文件有长度限制，如果整部小说放在一个文件中，可能会超出处理能力。拆分成章节文件后，系统可以逐批处理，既保证了处理质量，又避免了长度限制。同时拆分后的文件更容易管理，可以灵活选择要改编的章节范围。

Q2：拆解出的剧情点数量不够怎么办？

如果系统提示冲突密度不足，可能是因为这几章的小说原文确实缺少核心冲突[，也可能是系统识别不够准](http://breakdown.md)确。你可以手动检查小说[原文，看是否有遗漏的冲突点，然](http://adapt-method.md)后在breakdown.md中手动添加。也可以调整adapt-method.md中的冲突识别标准，降低核心冲突的判定门槛。

Q3：生成的剧本风格不符合我的要求怎么办？

你可以修改[output-style.md](http://output-style.md)文件，调整输出风格的要求。比如如果你希望对话更多，可以在文件中增加"对话占比不低于 30%"的要求。如果你希望动作描写更详细，可以增加"每个动作至少用两句话描述"的要求。修改后重新运行/create 命令，系统会按照新的风格要求生成剧本。

**Q4：可以同时改编多部小说吗？**

[可以，但建议为每部小说创](http://breakdown.md)建独立的项目文件夹。因为breakdown.md和 scripts 文件夹是共用的，如果在同一个项目中处理多部小说，会导致内容混乱。你可以复制整个项目文件夹，为每部小说创建一个副本，分别进行改编。

**Q5：这个改编流程可以商用吗？**

可以，但需要注意以下几点：确保你有小说的改编授权，不要侵犯原作者的版权。生成的剧本需要人工审核和润色，不能直接用于商业制作。如果用于商业项目，建议在 AI 生成的基础上进行二次创作，增加原创性。同时要注意遵守各平台的内容规范，避免违规内容。

![](img/a2667674dbf28620f1ad930fa2a6a086.png)

1.  剧本分镜创作 Skills

2.1 完整工作流

**注意：本案例难度较大，大家可以在小说改编漫剧和剧本分镜创作里只选择一个案例完成即可（新手推荐完成实战篇**的一个案例后直接进入到 Open claw 的学习），不需要全部都完成，21 天里，完成一个 Skills 案例即为收获

💡

**本**节**要带你完成什么**

想象一下这样的场景：你手里有一个精彩的剧本，想要把它变成视觉分镜。传统方式下，你需要找到一位分镜师，沟通需求、反复修改，耗时数周。而如果用 AI 直接生成，又会遇到各种头疼的问题——第一张图主角是黑发，第二张变成了金发；这一格主角朝左走，下一格突然朝右；有的画面像新海诚，有的像皮克斯，风格完全不统一……

**AI 分镜师**

这个项目，就是为了解决这些问题而诞生的。

在 3.1 节中，我们学会了怎么样把一个网络小说改编成一个漫剧剧本，现在你手里有了一份完整的剧本，每一集都有清晰的剧情点、冲突设计和情绪钩子。

现在你就可以利用**AI 分镜师**这**个 skill**s，通过三个专业 AI 助手的协作，将你的剧本自动转化为可用于 AI 出图和图生视频的提示词。更重要的是，它采用独特的"渐进式视觉展开"方法论，确保了人物一致性、镜头连贯性和风格统一性，它是一个完整的智能工作流系统

**完成这个案例后，你会得到什么？**

• 一套完整的 AI 分镜生成 skills，可以把剧本片段转化为分镜脚本

• 9 格关键画面提示词（叙事锚点图）- 一眼看清整个故事的发展脉络

• 45 个动态指令（图生视频用）- 可以直接用于 Seaweed Dance 等 AI 视频工具

**预计完成时间：**

90-120 分钟（首次搭建）

在开始实操之前，我们先看一下整个系统的工作流程，这样你就知道我们要搭建的是什么。

**阶段 1：叙事节点分析**

Plain Text

```
📖 输入小说文本
↓🤖 视觉叙事师分析剧情
↓📊 识别14个叙事节点
↓🎯 选出9个关键锚点
↓✓ 质量把控审核
↓💾 保存到 narrative-nodes.md
```

**这一步是为了：**

从小说中提取关键的故事转折点，就像看电影时记住的那些重要场景。系统会自动识别哪些情节是关键的，哪些可以省略。

**阶段 2：叙事锚点图（9 格）**

Plain Text

```
📋 读取叙事节点分析
↓🎨 视觉叙事师生成9格提示词
↓🖼️ 每格包含：构图+光影+色彩+人物描述
↓✓ 质量把控审核（检查人物一致性、风格统一性）
↓💾 保存到 anchor-prompt.md
```

**这一步是为了：**

生成 9 个关键画面的详细描述，这 9 格就像是整个故事的"骨架"，定义了人物长什么样、场景是什么风格、整体色调如何。后续所有画面都会以这 9 格为基准。

阶段 3：动势展开图（36 格）

Plain Text

```
📋 读取叙事锚点图
↓🎬 视觉叙事师展开每个锚点
↓📐 每个锚点展开成4格（起承转合）
↓🧬 继承锚点的&quot;视觉DNA&quot;（人物、风格、色调）
↓✓ 质量把控审核（检查连贯性）
↓💾 保存到 unfold-prompt.md
```

**这一步是为了：**

在 9 个关键画面之间填充过渡画面，让故事更流畅。就像动画中的"中间帧"，确保从一个动作到下一个动作的过渡自然。

**阶段 4：动态指令（45 个）**

Plain Text

```
📋 读取锚点图+展开图
↓🎥 动态设计师生成运动指令
↓📝 每格定义：镜头怎么动、人物怎么动、节奏快慢
↓🌍 输出英文指令（AI视频工具支持更好）
↓✓ 质量把控审核
↓💾 保存到 kinetic-prompt.md
```

**这一步是为了：**

把静态画面变成动态视频。每个画面都有对应的运动指令，告诉 AI 视频工具"镜头要推进"、"人物要转身"、"云要飘动"等等。

**为什么不直接让 AI 一次性生成 36 格分镜，而要分成"9 格→3**6 格"两个阶段？因为 AI 分镜存在人物不一致、镜头不连贯、风格不统一三大痛点

而这个工作流程里面采用了渐进式视觉展开，

先定锚点，再展开细节。

就像画一幅巨大的壁画，传统方法是直接从左画到右，很容易出问题。渐进式方法是：

1.**先画素描草图**（叙事节点分析）- 确定主要元素的位置

2.**再画 9 个彩色小样**（叙事锚点图）- 定义视觉风格、人物外貌、色调

3.**最后画完整细节**（动势展开图）- 拿着 9 个小样作为参考，画每个区域的细节

**关键机制：视觉 DNA 传递**

当生成第 3 组展开图时（比如"主角进入游戏"这组），系统会把第 3 格锚点图作为"参考图片"输入给 AI，AI 看到参考图后，会继承图中的人物外貌、服装、发型、光影风格。

这就好比：你让画师画一个角色，第一次你详细描述；第二次你不用重新描述，直接给他看第一次画的图，说"照着这个画"。

![](img/0bc415546563611591d28b3a78c4381e.png)

2.2 手把手带你走完完整流程

让我们先抛开所有技术细节，跟着一个实际案例，走一遍完整的操作流程。

**场景设定**

假设你是一位短剧创作者，手里有一个网文改编的剧本。你想把它做成 9:16 竖屏短剧，风格想要"日漫·新海诚"的感觉。

第一步：准备工作（2 分钟）

**1️⃣ 确认项目结构**

打开项目文件夹，你应该看到这样的结构：

Plain Text

```
AI 分镜师/
├── script/          ← 这是放剧本的地方
├── outputs/         ← 这是生成结果会保存的地方
└── .claude/         ← 这是系统配置（你不用动）
```

**2️⃣ 放入剧本**

把你的剧本保存为.md或.txt文件，放进script/文件夹。

比如，创建一个第一章.md，内容是你的剧本（这里我给大家准备了一个）：

[

![](img/4c3940faceb5c3919e4365f934ae447f.png)

ch01-第一章.md](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/KPUMbz3baoPqrzxYtOjcxpjgnOc?response-content-disposition=attachment%3B%20filename%3D%22ch01-%E7%AC%AC%E4%B8%80%E7%AB%A0.md%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260526%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260526T190327Z&x-oss-expires=86400&x-oss-signature=2b26ed4a313416bc6093107cbc57b0fe8f29fa3f3512351eaa1c00c1bdec97c4&x-oss-signature-version=OSS4-HMAC-SHA256)

**注意**

：虽然系统支持任意文件名，但建议带上集数标识，比如ep01-创世.md或ch01-开局.md，这样处理多集时更方便。

第二步：启动系统（3 分钟）

1️⃣ 打开 Claude Code

在终端中进入项目文件夹，启动 Claude Code。

**2️⃣ 系统初始化**

系统启动后，会自动检测项目状态。你会看到类似这样的欢迎语：

Plain Text

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

如果项目里面缺少需要的项目文件夹，它也会补充项目文件夹

**3️⃣ 配置项目信息**

系统会询问你三个关键问题：

**问题 1：视觉风格**

系统会列出可选风格：

• 写实类：真人写实、电影胶片、纪录片

• 3D 动画：皮克斯、迪士尼、梦工厂、3D CG

• 2D 动画：日漫、日漫·新海诚、日漫·吉卜力、国漫、国漫·水墨

• 艺术类：概念艺术、油画、水彩

• 特殊类：赛博朋克、蒸汽朋克、黑色电影

你回答：**日漫·新海诚**

**问题 2：目标媒介**

可选：电影、短剧、漫剧、MV、广告

你回答：**短剧**

**问题 3：画幅比例**

可选：16:9（横屏）、9:16（竖屏）、21:9（超宽）、1:1（方形）

你回答：**9:16**

这三个答案会被系统记录下来，成为后续所有生成工作的基准。

第三步：输入"继续"，让系统自动工作

从现在开始，你的操作变得极其简单——只需要输入"继续"。

![](img/88c3e77898a1b665021c38c1c5ef9720.png)

**1️⃣ 第一阶段：叙事节点分析**

系统开始工作：

Plain Text

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

Plain Text

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

Plain Text

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

Plain Text

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

第四步：查看你的成果

现在打开outputs/文件夹，你会看到四个文件：

Plain Text

```
outputs/
├── narrative-nodes-ch01.md      # 叙事节点分析
├── anchor-prompt-ch01.md        # 9格叙事锚点图
├── unfold-prompt-ch01.md        # 36格动势展开图
└── kinetic-prompt-ch01.md       # 45个动态指令
```

这些文件的内容是什么呢？

narrative-nodes-ch01.md是系统对剧本的结构化分析。它识别出了 14 个叙事节点，并从中选出了 9 个最关键的作为"锚点"。

anchor-prompt-ch01.md是 9 格提示词。每一格对应一个关键叙事节点，包含完整的画面描述、构图、光影、色彩等信息。这 9 格连起来，能一眼看清整个故事的发展脉络。

unfold-prompt-ch01.md是 36 格提示词。它将 9 个锚点中的每一个都展开成 4 格（起-承-转-合），展示更细致的动作和情绪变化。

kinetic-prompt-ch01.md是 45 个动态指令。它为每个画面定义了如何运动——镜头怎么推、人物怎么动、节奏是快是慢。这些指令可以直接用于图生视频工具。

第五步：使用这些提示词

**1️⃣ 用于 AI 出图**

打开anchor-prompt-ch01.md，找到第一格的提示词：

Markdown

```
**⚠️ IMPORTANT - CHARACTER REFERENCE IMAGE ⚠️**
If you have character reference images for An Lushan, Li Longji, Yang Guozhong, or Chen Xuanli, UPLOAD them and set reference strength to HIGH. The character&#x27;s face, hairstyle, and body type must MATCH THE REFERENCE IMAGE EXACTLY.

A 3x3 storyboard grid showing 9 sequential narrative panels of the An Lushan Rebellion&#x27;s outbreak and the fateful court decision that sealed the Tang Dynasty&#x27;s fate.

**Character Consistency (CRITICAL - Use Reference Image if Provided):**

Li Longji (Tang Emperor Xuanzong): A 70-year-old Chinese man, emperor of the Tang Dynasty. Wears luxurious golden imperial robes with dragon embroidery, a flat-topped imperial headdress with hanging jade beads. His face shows both the dignity of a once-great ruler and the weariness of age—deep wrinkles around the eyes, slightly sagging skin, but still commanding presence. Gray beard and thinning gray hair. When smiling, appears benign but somewhat detached; when angry, brow furrows deeply.
```

复制这段文字，粘贴到 Nano banana 中，就能生成对应的分镜图。由于对于 AI 来说，9:16 不是一个常见的训练图的尺寸，所以有可能会出现问题。但出现问题了之后，你再去跟他多一轮沟通，也会得到好的效果。

沟通过程：

![](img/6f5076a423f40479ed3589bc877188d3.png)

最后成品结果：

![](img/0ada6cbdd3921270ded0385bc8cc73e8.png)

拆分分镜

由于九宫格肯定不能完整地把我们一集视频全部都搞出来，所以某些中间特定的关键帧就需要把镜头进行拆分。这时候我们需要做的就是点开unfold-prompt-ch01.md文件，找到对应的镜头，比如说展开组 1 就是第一个镜头

![](img/3c9ef0e4faad78c255f17d73a164b230.png)

然后通过跟 AI 去沟通描述，把对应的分镜给拆解下来：

![](img/17449b8e5002f3df0f4c9c28daa58110.png)

再把对应的分镜和对应的提示词放到对话框中，就可以形成新的分镜拆解

![](img/edb85ece02b53328ac7b134669149ea6.png)

最后的效果：

![](img/9d5766f4ff1fc3aac93175f20882ba53.png)

**2️⃣ 用于图生视频**

打开kinetic-prompt-ch01.md，找到对应的动态指令：

![](img/4f470c0ec6113a78f0ddc806f62071c6.png)

先用 AI 出图工具生成第一格的静态图，然后把这张图和这段动态指令一起输入到 AI 视频提示词 中，就能生成对应的视频片段。

效果如下（模型：Wan2.6）：

![](img/3414d58e70b085af205cc66b66f4ae7a.png)

d36bba6bb43b6c99496c0ab6649b6a9231370f0dd163691d606dff1a5883801a.mp4【在线播放】

![](img/c9b599e2df1f3453c4879028ebfae611.png)

![](img/fd926fcdbeadb3e7cea71782dfc1f4db.png)

2.3自己动手搭建skills

跟着走完前面的流程后，你应该很期待这样的一个 skills 怎么搭建出来吧。现在，让我们动手从零搭建一个简化版。

第一步：新建一个项目目录

新建一个项目目录，比方说我现在用的项目目录叫 AI 分镜师，在项目里边新建一个文件夹，命名为。cluade，这个是我们后续 skill 要存放的文件夹。把下面的这个解压缩文件包下载到本地，然后解压缩，等待下一步。

[

![](img/c10a0a08e06e9ee8ebfd34503f674c0a.png)

AI 分镜师.zip](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/R5pqba9WXof0DQx1XmWc6Az7nyc?response-content-disposition=attachment%3B%20filename%3D%22AI%20%E5%88%86%E9%95%9C%E5%B8%88.zip%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260526%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260526T190327Z&x-oss-expires=86400&x-oss-signature=f24eec4eca45edff1095a2a3b0b5fc640475df47ceed94d0b46b92bdfa6ef51a&x-oss-signature-version=OSS4-HMAC-SHA256)

![](img/05b25296be42c1a118a17445117b70ff.png)

第二步：创建主控制器

创建.claude/[CLAUDE.md](http://CLAUDE.md)，它[相当于是所有 Ag](http://CLAUDE.md)ent 和工具的基石，是整个项目的主 Agent，也是我们这个整个分镜师项目的总负责人，他会给各个 Agent 和 Skill 去安排工作。去我们文件夹里面找到CLAUDE.md的这个文件，可以点开我们现在的这个文件去熟悉一下，或者直接复制到项目目录里。

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

第三步：创建 Agents

创建.claude/agents/文件夹，这是我们放三个 Agent 的角色的地方，Agent 的角色就如下面的这个代码块所示，两个“---”之间的部分是这个 Agent 简短的介绍，分别说明了这个 Agent 叫什么、它具体的用处是什么，然后它用到的 Skill 是什么，每一次当 AI 被调取的时候，会首先看这一部分来决定是否启用这个 Agent。同样的，你们可以把文件夹中的 agents 部分的内容粘进来，或者自己做出适当的修改

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

第四步：创建 Skills

创建.claude/skills文件夹，这块主要是我们放我们几个 skills。Skills 的话可以被看作是 Agent 的工具。我们每一次在启动项目的时候，AI 也都会读一下两个“---”，中间部分的内容。Skill 是工具，是处理工作的这些细节的流程，而 Agent 主要是这个人格，是更好的帮助这个流程进行判断。

每一个都会有一个[SKILL.md](http://SKILL.md)的文[件作为这个 Sk](http://SKILL.md)ill 的主控单元，他去分配、去指导整个 skill 的工作流的工作，其余的还会有比方说模板文件夹，或者说一些可执行文件。比方说下图的这个 skill，除了SKILL.md文件之外，就是一个指导图片提示词生成的 MD 文件以及相对应的模板文件。模板文件为了方便管理，我们这里也单独放了一个文件夹，其他的 skill 也是以此类推。

![](img/bd521b40ccddddcf2a1765630a34cd74.png)

第五步：创建 Methodology

创建.claude/methodology/文件夹，这个文件夹里面主要是放的我们修改内容的一个方法论。注意，这个文件夹不是系统中必须要用到的一个文件夹，系统中一个 Agent 和 Skill 组成的工作流，只有 Agent 和 Skill 这两个文件夹是必须要存在的。像方法论这个文件夹主要是单独放置我们的方法论部分内容，方便管理和读取。方法论的这个文件夹里边包含有动态和静态提示词怎么写，以及故事节拍的这个模板，保证能够每一次输出都稳定的运行。

![](img/93c1ce9e4cee0df79cace83b87093140.png)

第六步：测试

1.  启动 Claude Code

1.  输入"继续"看系统是否正常工作（由于我们项目里边没有创建剧本以及输出的文件夹，初次运行的时候，整个系统会帮我们直接创建文件夹）

1.  在 Script 把我们的小说放进去，跟 Cloud 说继续，他就可以继续帮我们进行小说的拆解了

![](img/11f9379a1ba13823b8134303a8345768.png)

2.4 理解 skills 里面每个文件是什么意思

现在，我们要打开系统的"黑箱"，看看里面到底有哪些文件，每个文件是干什么用的，为什么要这样设计。

视频教程：

通过网盘分享的文件：RS200pro 2026-04-01 01-13-56.mp4

链接:[h](https://pan.baidu.com/share/init?surl=7KADNE8C4MPQ4Jt0QWY66Q&pwd=pqdn)ttps://pan.baidu.com/s/17KADNE8C4MPQ4Jt0QWY66Q?pwd=pqdn提取码: pqdn

--来自百度网盘超级会员v7的分享

**项目文件夹全景图**

让我们先看看整个项目的文件结构：

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

这个结构遵循一个清晰的原则：输入-处理-输出分离，配置与逻辑分离。

• script/和outputs/是用户可见的输入输出区

• .claude/是系统核心，用户不需要修改，但理解它有助于掌握系统

整体的结构讲完了，接下来咱们拆解一下配置各个文件的思路是什么：

**核心控制器：**[CLAUDE.md](http://CLAUDE.md)

**这是什么？**

[CLAUDE.md](http://CLAUDE.md)是整个系统的"大脑"和"中央控制器"。当你启动 Claude Code 时，它会首先读取这个文件，了解：

• 我是谁？（项目统筹）

• 我要做什么？（协调三个助手完成分镜）

• 怎么调用其他助手？（通过 Task 工具）

• 工作流程是什么？（四阶段流程）

• 出错了怎么办？（重试机制）

**为什么要单独写一个**[CLAUDE.md](http://CLAUDE.md)**？**

[在 Claude ](http://CLAUDE.md)Code 的架构中，CLAUDE.md是入口文件。它定义了这个项目的"系统提示词"（System Prompt），决定了 AI 的行为模式。

如果不写这个文件，Claude Code 就像一个没有受过训练的通用助手，不知道这个项目要做什么。

**关键内容解析**

让我们逐段分析[CLAUDE.md](http://CLAUDE.md)的内容：

**【角色】部分**

Markdown

```
[角色]
你是一名项目统筹，负责协调 storyboard-artist（视觉叙事师）、
director（质量把控）和 animator（动态设计师）完成影视分镜工作。
```

这段定义了"我"的身份。注意这里用**了项目统筹**而不是分镜师——因为它的职责是协调和管理，而不是直接生成内容。

**【任务】部分**

Markdown

```
[任务]
完成影视分镜提示词的生成工作，包括：
1. 叙事节点分析
2. 叙事锚点图提示词
3. 动势展开图提示词
4. 动态指令
```

这段定义了目标产出。明确列出四个阶段，确保不会遗漏。

**【总体规则】部分**

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

这段是核心工作流定义。它明确了：

1.  **阶段顺序不能跳**：必须先有节点分析，才能有锚点图

1.  **谁干活谁审核**：生成和审核必须是不同的 agent

1.  **循环改进机制**：不通过就修改，直到通过

【Subagent 调用机制】部分

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

这段解释了技术实现。关键点：

• 每个助手（subagent）有独立的上下文

• 通过agentId和resume机制保持对话连续性

• 这样助手能记住之前的讨论，不会"失忆"

**【错误处理与重试机制】部分**

Markdown

```
[错误处理与重试机制]
审核重试限制：
- 同一阶段最多重试 3 次
- 超过 3 次后，暂停并请求用户介入：
  &quot;⚠️ 审核未通过（已重试 3 次）
...&quot;
```

这段定义了兜底机制。如果质量把控连续 3 次都不满意，可能是遇到了复杂问题，需要人类介入。

AI 助手配置：agents/ 目录

agents/ 目录下有三个文件，分别配置三个 AI 助手。

**为什么要用配置文件定义助手？**

Claude Code 支持通过 Markdown 文件定义自定义助手（Custom Agents）。这样可以把助手的角色、技能、输出规范都固化下来，每次调用时都保持一致的行为。

**storybo**ard-artist.md（视觉叙事师）

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

**逐段解析：**

• Frontmatter（--- 之间）：定义助手的元数据

◦name：标识符，用于调用

◦description：一句话说明用途

◦skills：关联的技能包

◦model：使用的 AI 模型（opus/sonnet/haiku）

◦color：UI 显示颜色

• **[角色]**：定义身份定位，强调"视觉叙事"能力

• **[任务]**：明确职责范围，四个任务

• **[输出规范]**：这是对输出格式的硬性要求

◦"中文叙事描述式"：不是关键词堆叠，而是完整段落

◦"不要逐条解释"：避免啰嗦，直接给结果

• **[协作模式]**：定义与其他助手的关系

[director.md](http://director.md)**（质量把控）**

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

**关键设计：**

• **输出必须是 PASS/FAIL**：不能模棱两可

• **FAIL 时必须给具体意见**：不能只说"不好"，要说"哪里不好、怎么改"

• **关联 skills**：审核时会读取 review-checklist.md 作为标准

[animator.md](http://animator.md)**（动态设计师）**

Markdown

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

**关键设计：**

• **使用 sonnet 模型**：动态指令相对简单，不需要 opus 的复杂推理，sonnet 更快更经济

• **输出必须是英文**：图生视频工具对英文支持更好

• **职责单一**：只负责动态指令，不碰静态分镜

**技能包：skills/ 目录**

如果说 agents/ 定义了"谁"，那么 skills/ 就定义了"怎么做"。

每个技能包相当于一本"执行手册"，详细说明：

• 这个任务的目标是什么？

• 分几个步骤执行？

• 每一步要读取什么文件？

• 输出要遵循什么格式？

为什么要分离 agents 和 skills？

这是**角色与能力分离**的设计。

• Agent 定义"我是谁"（身份）

• Skill 定义"我怎么做"（方法）

好处是：

1.  **可复用**：同一个 skill 可以被多个 agent 使用

1.  **可维护**：修改 skill 不需要改 agent 配置

1.  **清晰**：结构和逻辑分离

[film-sto](http://SKILL.md)**ryboard-**skill/SKILL.md（分镜师技能包）

Markdown

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

**关键设计解析：**

1.  **【文件结构】部分**：明确列出了依赖的文件，方便维护者理解关系

1.  **【功能】部分****：每个功能**都分为"第一步、第二步"，这是标准化流程

◦每一步明确要读取什么

◦每一步明确要输出什么

◦这样 agent 执行时不会遗漏步骤

1.  **【分镜原则】部分**：定义了不可违反的硬性规则

◦方法论遵循原则 → 确保质量

◦视觉 DNA 传递原则 → 确保一致性

◦模板遵循原则 → 确保格式统一

[storyboa](http://SKILL.md)**rd-revi**ew-skill/SKILL.md（导演技能包）

Markdown

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

**关键设计解析：**

1.  **【审核流程】标准化**：每个审核都遵循"五步流程"

◦建立整体理解（读剧本）→ 知道要干什么

◦读取基准（读方法论+清单）→ 知道标准是什么

◦读取待审核内容 → 看实际产出

◦逐项检查 → 对比标准和实际

◦输出结果 → PASS 或 FAIL

1.  **【输出格式】严格定义**：

◦PASS 时简要说明通过原因（让用户知道为什么过了）

◦FAIL 时必须给"位置+规则+修改方向"（让用户知道怎么改）

**animator-skill/**[SKILL.md](http://SKILL.md)**（动画师技能包）**

Markdown

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

**关键设计解析：**

1.  **【依赖关系】明确声明**：

◦动态指令必须基于静态分镜

◦如果前置文件不存在，技能包会报错

1.  **【读取顺序】有讲究**：

◦先读 narrative-nodes.md → 理解"这个场景要表达什么情绪"

◦再读锚点图和展开图 → 理解"画面长什么样"

◦最后读方法论 → 理解"怎么写动态指令"

方法论：methodology/ 目录

如果说 skills/ 是"怎么做"，methodology/ 就是"做到什么标准"。

**storybo**ard-methodology-playbook.md（分镜方法论）

这是一个 700+ 行的庞大文档，定义了分镜的所有规则。它是整个系统的"法律"，所有产出必须符合这里的规定。

文档结构：

Markdown

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

**为什么要写这么详细？**

因为 AI 助手需要具体的规则才能做出正确判断。比如：

• 不只是说"要连贯"，而是要说"屏幕方向要保持一致，越轴必须有过渡手段"

• 不只是说"要简洁"，而是要说"一镜一意，能用一个画面讲清就不要重复"

**motion-pr**ompt-methodology.md（动态指令方法论）

定义了如何将静态分镜转化为动态指令的规则。

核心原则：

Markdown

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

为什么动态指令和静态分镜的方法论不同？

因为两者的输入输出完全不同：

| 维度 | 静态分镜 | 动态指令 |
| --- | --- | --- |
| 输入 | 剧本文字 | 已有图片 |
| 输出 | 画面描述 | 运动描述 |
| 长度 | 详细（几百字） | 简洁（50-200 字符） |
| 语言 | 中文 | 英文 |

模板：templates/ 目录

模板定义了输出文件的格式。它们位于各自 skill 包的 templates/ 目录下。

**为什么要模板？**

1.  **格式统一**：每次生成的文件结构一致

1.  **字段完整**：不会遗漏必要的信息

1.  **易于解析**：后续程序可以预期文件结构

narrative-nodes-template.md

Markdown

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

anchor-board-template.md

Markdown

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

unfold-board-template.md

Markdown

```
# 动势展开图提示词

## 视觉DNA传递规范
## 格1展开：【锚点名称】
1-1（起）：
1-2（承）：
1-3（转）：
1-4（合）：
```

kinetic-prompt-template.md

Markdown

```
# 动态指令

## 格1：【锚点名称】
### 关键帧
1-0: [Kinetic Directive]

### 展开格
1-1: [Kinetic Directive]
...
```

## 三、OpenClaw 的入门和实战

### 01.入门：全面认识 OpenClaw

0.本章概要

💡**本章会带你正式进入 OpenClaw 的入门与实战阶段**，重点不是停留在“知道 OpenClaw 是什么”，而是让你真正学会：怎么部署、怎么接入聊天渠道、怎么安装 Skills、怎么把它变成一个能替你干活的 AI 员工。

首先，你会建立一个关键认知：**O**penClaw 不是一个只会给建议的聊天工具，而是一个可以接收指令、调用工具、执行任务的自主式 AI Agent。

它的核心价值，不是“陪你聊天”，而是“替你做事”——比如读取文件、操作浏览器、整理资料、定时执行任务、接入飞书/微信/QQ 等渠道，真正进入日常工作流。

接着，你会学习 OpenClaw 的实际部署与安装方法，以及安装和使用 Skills 的基本方式。学完这一部分，你就能把 OpenClaw 真正跑起来，并让它在飞书、微信、QQ、钉钉、企业微信等场景里和你正常协作。

在此基础上，本章还会带你进入两个实战方向。**第一个是 OpenClaw 的基础使用场景，**包括定时发送新闻总结、发票归档、论文搜索等“小试牛刀”案例，帮助你快速建立对 OpenClaw 工作方式的直觉；**第二个是 OpenClaw 的典型实战应用，**比如搭建个人知识库、跑通公众号自动化，或者进一步延伸到企业知识库、AI 数字员工、AI 客服等业务自动化场景。

学完这一章，你真正收获的，不只是装好一个 Op**enClaw，而是掌握一种新的**工作方式：让 OpenClaw 帮你干活

**注意：实战篇有 2 个实操案例，进阶篇有 2 个实操案例，这 4 个案例不需要你全部掌握，**只需要学会一个即可，新手推荐第一个个人知识库搭建，先把 OpenClaw 用起来

💡

**本章航线图**

完成本章节的学习和实操，即可完成航线图的第一阶段。

第三阶段：OpenClaw 的入门和实战（约 7 天）

完成 OpenClaw 安装部署（约 1 天）

完成 OpenClaw 的**一个**实战案例（约 3 天）

完成 OpenClaw 的**一个**进阶案例（约 3 天）

1.  OpenClaw 是什么

26 年初，一个叫做 OpenClaw 的 AI 产品在 Github 上迅速爆火，直接导致了 Macmini 卖断货，各模型厂商的 API 调用量激增，间接推高了 AI 大模型公司的股价，比如 Mninimax 和智普。据说 M2.5 调用量在 OpenRouter 排名前十，而且现在国内大模型和云计算厂商迅速跟进，也都搞出了自己的小龙虾版本，掀起了百虾大战。

![](img/5f76e2490c02ff2b43333f3c7f11e963.png)

OpenClaw 到底有什么魔力，让世界为之疯狂，纷纷加入养虾大军，它不是又一个 Chatbox，而是一个可以通过简单的对话方式给你干活的 AI 员工。

不是给方案，而是直接执行

我们可能已经习惯了这样的应用场景，当我们需要 AI 解决问题时：

Plain Text

```
你：帮我清理一下服务器上的磁盘空间
ChatGPT：我可以给你一些磁盘清理的建议...
```

OpenClaw 不一样：

Plain Text

```
你：帮我清理一下服务器磁盘空间
OpenClaw：[正在SSH连接服务器...]
[正在读取磁盘分区...]
[已分析磁盘空间占用情况...]
请问是否要删除 xx。
```

一个给建议，一个做事情。 这就是本质区别。

OpenClaw（龙虾）能读写文件、执行命令、控制浏览器、收发消息、定时巡检——所有数据都在你自己的设备上。你可以让它每天早上推送新闻简报，自动回复邮件，甚至写代码、提 PR、跑测试。

**1.1**OpenClaw 的本质：自主式 AI Agent**

O[penClaw 是](https://en.wikipedia.org/wiki/OpenClaw)一个开源的自主式 AI Agent 执行引擎，由开发者 Peter Steinberger 创建。根据Wikipedia的介绍，它是一个免费开源的自主人工智能代理项目，以消息平台（WhatsApp、Telegram、Discord、Slack 等）作为主要用户界面。

这主要依赖它的核心功能：

• **本地运行**。**数据完全由你掌控，不送到别人的服务器

• **多渠道 Gateway 网关**。**通过单个 Gateway 网关进程连接 WhatsApp、Telegram、Discord 和 iMessage。

• **插件渠道**。**通过扩展包添加 Mattermost 等更多渠道。

• **多智能体路由**。**按智能体、工作区或发送者隔离会话。

• **媒体支持**。**发送和接收图片、音频和文档。

• **Web 控制界面**。**浏览器仪表板，用于聊天、配置、会话和节点管理。

• **移动节点**。**配对 iOS 和 Android 节点，支持 Canvas。

**1.2 OpenClaw 的**工作原理

![](img/17767fb096e54cd1bc5caf0c263c1e7e.png)

OpenClaw 通过 Gateway 网关将聊天应用连接到 AI 智能体。Gateway 是会话、路由和渠道连接的唯一事实来源。

核心组件：

1.  Gateway 网关

◦连接各个聊天平台（飞书、企微、QQ、Telegram 等）

◦管理会话和消息路由

◦默认地址：http://127.0.0.1:18789/

◦配置文件：~/.openclaw/openclaw.json

1.  AI 智能体

◦支持 Claude、GPT、Gemini、DeepSeek、Kimi 等多种模型

◦可以本地运行或远程调用

1.  Skills 技能系统

◦文件管理、知识管理、自动化等

◦可自定义开发

1.  ClawHub

◦技能市场，可以下载和分享 Skills

💡 Gateway 网关是什么？Gateway 是 OpenClaw 的核心服务，它像一个"中央调度站"，负责：

• 接收来自不同平台的消息（飞书、企微、QQ、Telegram 等）

• 将消息转发给 AI 智能体处理

• 把 AI 的回复发送回对应平台

• 管理所有的会话和上下文

这就是为什么你可以在任何平台上使用 OpenClaw，因为 Gateway 统一管理了所有的连接。

![](img/179bdc989d4fee62429c247c0ba8b734.png)

1.3OpenClaw 的架构分为四层

1.  消息渠道（Channels）：Telegram、Discord、Slack、飞书、CLI 等多种接入方式

1.  智能决策核心（Brain）：LLM 推理、任务分解与规划、工具选择与调用

1.  技能插件系统（Skills）：文件操作、Shell 命令、浏览器控制、API 集成等

1.  记忆与身份系统（Memory & Identity）：一组 Markdown 文件——IDENTITY.md（身份）、SOUL.md（性格）、USER.md（你的信息）、MEMORY.md（长期记忆）等

这种分层设计让 OpenClaw 既灵活又可控。

![](img/101e0a43fd9b6a58e74d1bb0a70e0c23.png)

**深入了解：价值与成本**

优势：

• 并行探索：多个 Sub-agent 同时搜索、分析、汇总，比串行快得多

• 上下文隔离：子任务在干净的上下文中执行，避免"上下文退化"

• 推理算力扩展：突破单个 Agent 的上下文窗口限制

成本：

• Token 成本从 1x 跃升到 15x

• Agent 间传递会丢失上下文细节（"电话游戏"效应）

• 多 Agent 并行时可能产生隐式决策冲突

Anthropic 的经验："有些团队投入数月构建复杂的多智能体架构，结果发现改进单智能体的提示词就能达到同等效果。"

判断标准：低耦合任务（搜索、信息收集）适合拆分；高耦合任务（架构设计、核心编码）保持单一。

![](img/a7dbb3fe53619d9793c0e830a718eb04.png)

**深入了解：应用场景**

个人效率：每天早上自动推送天气 + 日历 + 邮件简报；自动分类邮件并标记优先级。

开发者工作流：PR 提交后自动代码审查；函数签名变更时自动更新 API 文档。

企业级应用：多渠道客户支持自动化；每周自动生成数据分析报告。

![](img/a4423843dfbcdca073072f91cb708c1f.png)

1.  OpenClaw 的部署和安装

2.1 云服务器一键部署安装

对于大多数人来说，云部署是最省心的选择。你不需要在自己电脑上装任何东西，只需要在浏览器里操作。

目前，国内主流云厂商都支持 OpenClaw 一键部署。但经过实际体验，各家的方案差异不小。我们先给一个总览，再重点讲最推荐的方案。表 3-1 给出了国内云厂商方案总览。

**表 3-1 国内云厂商方案总览**

| 平台 | 最低配置 | 价格 | 内置模型 | 绑定生态 | 适合谁 |
| --- | --- | --- | --- | --- | --- |
| 腾讯云 | 2 核 2GB | 99 元/年 | 否 | 不绑定，自由配 Key | 综合首选 |
| 阿里云 | 2 核 2GB | 秒杀 9.9 元/月 | 是（qwen3.5-plus） | 百炼 Coding Plan | 抢到了很划算 |
| 火山引擎 | 2 核 4GB | 9.9 元/月起 | 是（方舟模型） | 方舟 Coding Plan | 飞书重度用户 |
| 百度云 | 2 核 4GB | 0.01 元首月 | 是（千帆模型） | 千帆平台 | 纯体验尝鲜 |
| 扣子编程 | 不需要服务器 | 免费起步 | 是（豆包 2.0） | 字节生态 | 零门槛体验 |

看完这张表，你可能觉得阿里云 9.9 元/月、火山引擎 9.9 元/月看着更便宜，但实际用下来，事情没那么简单。

**阿里云**

的 9.9 元/月是限时秒杀价，需要抢，而且限购。抢不到的话常规价并不便宜，续费价格比新购还高不少。另外，它内置的模型走的是百炼平台的 Coding Plan，基本绑定在阿里自家的模型生态里。

**火山引擎**

的问题更明显。虽然标着活动价 9.9 元/月，但它的方舟 Coding Plan 价格不低——一台 2 核 2GB 的服务器加上模型套餐，每月实际开销轻松超过 100 元。同样绑定在字节的模型生态里。

相比之下，**腾讯云**最实在。99 元/年的 2 核 2GB 轻量应用服务器，折算下来每个月不到 **9 块钱。这个价格稳定，不**用抢，支持续费同价，不会遇到“续费刺客”。最关键的是：腾讯云的方案不绑定模型生态。你买完服务器之后，可以自由配置任何模型厂商的 API Key——DeepSeek、Kimi、Claude、GPT。这在实际使用中非常重要，因为你很可能会在不同模型之间切换和尝试。

所以，我们推荐腾讯云作为云部署的首选方案。下面以腾讯云为例，手把手走一遍。

**（一）**购买轻量应用服务器**

[在腾讯云上打开部署 OpenClaw 页面：](https://cloud.tencent.com/act/pro/openclaw)https://cloud.tencent.com/act/pro/openclaw，如图所示，直接点击“立即部署我的 AI 助理”按钮。

![](img/2674792f36878bbae429c10b6172e681.png)

此时会打开如图所示的服务器选择页面，初次上手可以选择 2 核 2G 的，年费是 99 元，还是比较划算的。接着，直接点击“立即购买”按钮**（新手第一次可以先买一个月 20 的体验一下）**

![](img/739d55c099a27e40bebff0f931137bca.png)

或者可以选择 99 包年的套餐

![](img/7282d0aec2a3ef720b9c3b7051503bb0.png)

技术小贴士：什么是“2 核 2G”？

“2 核”是指服务器有 2 个 CPU 核心，决定它能同时处理多少任务；“2G”是指 2GB 内存，决定它能同时在“脑子”里装多少东西。对于 OpenClaw 来说，2 核 2G 完全够用——真正吃算力的推理工作是交给外部 AI 模型来做的，服务器只负责调度和转发，非常轻量。

**（二）选择 OpenClaw 应用模板

点击“立即购买”按钮后，就跳转到了如图 3-3 所示的配置页面。在这个页面中，你需要确认以下两项。

• 地域：建议选择离自己比较近的城市，这里我选择“广州”，以获得更快的响应速度。

• 镜像：确认为 OpenClaw 官方镜像（一般默认就是），如果不是，可以在下拉列表中手动选择。

核对无误后，再次点击底部的“立即购买”按钮进入支付环节。

提示：这里的“搭配购买”项并非必选，大家可以看自己情况购买。若无特殊业务需求，直接跳过即可，不影响 OpenClaw 的正常运行。

![](img/c50f230b1fa4fdd6f982199a705caeb4.png)

下一步就跳转到支付页面，如图所示，选择自己的付款方式就可以了。

![](img/a7ec2fea4c42a78b8c582f85ec94b666.png)

买完之后，在腾讯云的控制台中找到“轻量应用服务器”的“服务器”项，就可以看到刚刚买到的 OpenClaw 服务，如图所示。

![](img/dbb63b8deddb1b785d69a3fe4f27e8b7.png)

这里还需要再次确认服务器的“防火墙”里是否有 18789 放行端口。如图所示，在防火墙列表中，请检查是否已添加了 18789 端口。通常，镜像会默认添加该规则。如未看到，点击“添加规则”按钮即可。

![](img/686af7e7399d7ad6c3519a3682391373.png)

然后按照图所示，选择“全部 IPv4 地址”和 18789 端口，点击“确定”按钮即可。

![](img/4db35c923160fc8784c9ac964444a124.png)

![](img/e01d1afa2c9b3e205214ee863e1ff3ab.png)

**（三）**打开 Dashboard**

现在有了新的方式可以直接打开 Dashboard 对话框

如下图，打开腾讯云轻量云服务器的 OpenClaw 的配置

切换到「应用管理」的菜单，然后会在右侧页面看见一个「安全开启 OpenClaw 面板」

![](img/43c62ddbafccf17bd8b57918fd95ed01.png)

单击后，就会如下图，等待生成最后的 url 就可以。

![](img/ba423c874f5d74b2b6136c330049292b.png)

然后就会出现下面的图片，点击立即访问就可以

![](img/aed0fecb9d504c0fdd0e453c5d67a21c.png)

如果还是不能访问，那么就再次点击下面的这个按钮

![](img/13baa2bfbc731456e6aeee560454306f.png)

他就会说放行端口

![](img/72bd1880595a809b40df6d54e8936ef5.png)

然后就会有如下图的链接显示

![](img/9a43b18d5b53bd24609ec091c02580fa.png)

现在点击立即访问，就可以了

![](img/2495e7a667da3fc8f57d66d8c757f21b.png)

（四）接入飞书

**渠道（Channel）**

就是为了解决这个问题的。把飞书接上之后，你在飞书里给智能体发一条消息，它就在飞书里回你。不需要打开任何额外的网页或 App。

飞书是国内企业用户最主流的聊天工具之一，而且 OpenClaw 从 2026 年 2 月起就内置了飞书支持，配置起来比较顺畅。下面我们以飞书为例，完整演示渠道接入的流程。

在腾讯云服务的 OpenClaw 模板上，安装极其简单。如图所示，腾讯云提供 OpenClaw 服务快捷配置飞书通道，点击“前往授权”按钮。

![](img/5fc009e6a9f9382704ffda86358317dc.png)

下一步就是如图所示，使用飞书扫码配置飞书机器人。

![](img/8f5eb3c26093e1ebd552e9574ad5065f.png)

接着会打开如图所示的页面，此时会自动配置各种权限，我们只需要等待就行。

![](img/17ac6a2b7bccf95e5eb281286bfa435e.png)

上面的每一个步骤完成后，就可以看到如图 所示的界面，飞书就会收到消息，我们点击“打开应用”按钮就可以看到对话机器人了。

![](img/0150d3b0f53313333345b3350681c096.png)

打开应用后，就可以看到输入消息框，我们输入“你好，你是谁？”，就可以看到 OpenClaw 的回复，就代表飞书通道已经配置成功，如图所示。

![](img/cadc5d1a45c6a1bf57951147b9b2fc63.png)

（五）配置模型

上面已经配置好了飞书的通道，那我们现在就需要配置小龙虾的大脑，也就是模型。

我们上面刚好买了 Minimax 的 Token Plan 套餐，在这里刚好腾讯云的这个 OpenClaw 也支持，我们正好一键配置。

下面的链接就是访问轻量云服务器的地址，如果你不知道怎么进入，就直接点击下面的地址进去。（）

[h](https://cloud.tencent.com/login?s_url=https%3A%2F%2Fconsole.cloud.tencent.com%2Flighthouse%2Finstance%2Findex)ttps://console.cloud.tencent.com/lighthouse/instance/index

![](img/3ba3ed4a92e658a57be3947552af3fca.png)

点击配置，进来后就会看到类似如下的页面，我们找到页面上的「模型」的那个模块。

首先配置，选择模型， Coding Plan 如下，那就会出现各个厂商的，我们上面购买的是 Minimax 的 Token Plan，那我们就选择 Minimax 的 Token Plan。

如果你选择了其他的 Calling Plan，那么就选择对应的套餐就可以。如果你没有 Calling Plan，想用 API 其他的 API，那么就选择模型 API。

![](img/ab73d2f9ff80e59065abf53745b4004e.png)

下面就是选择模型版本，这个可以保持默认。

![](img/b508041ae3e9b2f5938cf7e70bbbcce3.png)

下面就是要粘贴你的 API Key 了。

我们在前面购买的 Mini Max 的地方，进入到 Token Play。如果你忘记链接了，可以点击下面的直接进入。

[https://platform.minimaxi.com/use](https://account.minimaxi.com/unified-login?login_redirect=%2Foauth2%2Fauthorize%3Fclient_id%3Dplatform-minimax%26redirect_uri%3Dhttps%253A%252F%252Fwww.minimaxi.com%252Fauth%252Fcallback%26response_type%3Dcode%26state%3DeyJyZWRpcmVjdF91cmkiOiJodHRwczovL3BsYXRmb3JtLm1pbmltYXhpLmNvbS91c2VyLWNlbnRlci9iYXNpYy1pbmZvcm1hdGlvbi9pbnRlcmZhY2Uta2V5IiwiY3NyZiI6IjIzMmQ2N2VlLWUzMmMtNGQwYi05NGI1LWM3OWQ4NzM0ZjQ1NiJ9)r-center/basic-information/interface-key

![](img/536920a71535448fc92061148dfc3f39.png)

复制好上面的 Token，Plan Key 以后。回到腾讯云的轻量服务器的 OpenClaw 界面。是前面刚刚的那个界面。

![](img/bc068bcf687550ec467518e799d00518.png)

![](img/822c00064b1bc096e8edabfde954a8f3.png)

2.2其他手机端的接入方式

💡这里演示的是手机端其他的应用程序，比如 QQ、钉钉、企业微信等的接入。

其实官方的说法叫 channels 的接入。

（一）手机个人微信接入

相信大家看到这个还是比较开心的，微信是大家现在都离不开高频率使用的应用，所以微信的接入小龙虾，方式有两种，下面分开来说一下

💡两种方式用的都是同一个微信 ClawBot 机器人

• 如果你是腾讯云，无脑选择第二种安装

• 如果你是其他云，或者可以进入终端输入命令的选择第一种

**第一种：手机端微信插件安装**

这个首先保证你的微信版本在 8.0.70 版本以上。

然后进入到微信“我的-设置”页面，如图，找到“插件”菜单，点击进去。

![](img/8d5ce65a402da9d5db992348b97c1494.png)

点击进来后可以看见如图所示，看到又要给“微信 ClawBot”的插件，我们点击“详情”。

![](img/73e69ef543ec34935d77ba2552db0227.png)

进来插件的详情页后，如图所示，就可以看到如何安装，以及快捷的扫一扫。

![](img/92220d3091015046d7944225df5c3c83.png)

然后打开对应的终端，如果是本地电脑，苹果电脑打开的就是终端软件，Windows 打开的就是 PowerShell，云服务器的可以在对应的后台链接终端。

如图所示，打开终端后是一个黑色的窗口，直接复制上面截图的命令，然后粘贴到终端执行。

![](img/271fd8626058eb1589076e7bb2acaef9.png)

如图所示，安装插件完成后，就会启动微信扫码登录，下面会有一个二维码，我们在刚刚手机微信页面，点击“开始扫一扫”。

![](img/2f4c0acf67b2003279f64f8004aebdf1.png)

如图所示，手机微信扫码后，就会提示微信连接成功。

![](img/e477b59fd269ad1e36f6ef2352ce018e.png)

我们在手机微信推出前面的页面，回到微信聊天框，如图 5-xx 所示，就会出现一个红色的头像，显示名称“微信 ClawBot”的一个联系人。

![](img/86429b69a5d7a12700604ad2bd9cbafc.png)

下面就可以点进去，跟这个微信机器人聊天，如图 5-xx 所示，可以发文字，还可以发语音。

![](img/5d9dbe43e89d921dac041cda84ccd10c.png)

到这里微信 ClawBot 的机器人就安装完成了，下面就可以愉快的在微信里面进行养虾。

**第二种：腾讯云一键安装**

如果你是腾讯云安装的 OpenClaw 用户，那么在腾讯云服务器的 OpenClaw 的“应用管理”下的通道就可以看到微信的接入。

[如](https://cloud.tencent.com/login?s_url=https%3A%2F%2Fconsole.cloud.tencent.com%2Flighthouse%2Finstance%2Findex)图所示，首先我们需要进入到腾讯云轻量服务器的控制台（链接https://console.cloud.tencent.com/lighthouse/instance/index），直接点击“配置”按钮。

Plain Text

```
https://console.cloud.tencent.com/lighthouse/instance/index
```

![](img/ace637de7775cd2deebe78287104d61b.png)

下面就是如图 5-xx 所示，可以看到通道的配置栏里会有“微信”的显示，我们点击“前往授权”。

![](img/cbec079b9dfd9511b9c9f425aa4a1b38.png)

如图 5-xx 所示，点击“前往授权”后就可以看到弹框页面，等待二维码的升成。

![](img/87be07c3b784be9169f4f83f891764ce.png)

等二维码生成后，直接使用个人微信的“扫一扫”就可以，如图 5-xx 所示，可以看到有“连接”的按钮

![](img/de1e6ec008814dc390e40406a74ab127.png)

图 5-xx 微信 ClawBot 扫码连接

我们点击“连接”按钮后，就直接进入了和微信 ClawBot 的对话框，如图 5-xx 所示，下面就可以发送消息，比如我先发个“你好”，可以看到微信 ClawBot 已经回复消息。

![](img/a2fec687dd3a66d807db7957df7cbee2.png)

图 5-xx 微信 ClawBot 回复消息

![](img/29305f12b7111c99038ee81be0b5657b.png)

**（二）QQ接入龙虾**

（1）打开 QQ 的开放页面[https://q.qq.com/qqbot](https://q.qq.com/qqbot/openclaw/login.html)/openclaw/login.html

然后使用手机 QQ 扫描右侧的二维码，就会跳转到配置机器人的页面，如图所示。

![](img/05170805242d510663214cd13cee1221.png)

（2）点击“QQ 开放平台”页面上的“创建机器人”按钮，如图所示，会显示 AppID 和 AppSecret 信息。

提示：AppID 和 AppSecret 信息一定要保存到本地，因为第二次就不会显示，重置会更改值，可能导致机器人失效。

![](img/6dc4fb797cb5abcbf0c318712eed550d.png)

下面截图的就是 AppID 和 AppSecret 的信息，一定要记得保存好。

![](img/fab9ef5138d82cc245f35c533f20f251.png)

图 4-11 创建机器人显示 AppId 和 AppSecret 页面

（3）下面就是去填写的小龙虾绑定，这里介绍的是腾讯云的配置方式。

![](img/5f095faa067dccd6b0bb1fdba1a3e569.png)

此时就可以看见 QQ 里面有机器人的消息，打开机器人消息聊天框，可以发送消息“你好，你是谁”，可以看到有回复，就代表配置成功了，如图所示。

![](img/dd242005ea84092145ca553dc7b40d53.png)

![](img/8a59bca20fa191d15169dec9c6f69ceb.png)

**（三）钉钉接入龙虾**

（1）打开钉钉开放者平台后（访问链接：https://open.dingtalk.com），点击页面右上角的“开发者后台”

![](img/b99f1ed79cfdfe7e33cfdf9f527a4498.png)

如图所示，先点击顶部的“应用开发”，然后点击左侧菜单的“钉钉应用”，就会看见页面上出现“立即创建”按钮即可。

![](img/3c66af118e700f23f9ddb009e80f915a.png)

（2）此时会打开“创建 OpenClaw 机器人”页面，机器人名称和机器人简介可以采用默认值，当然你也可以修改，如图所示

![](img/a04d1cb0089d7584ec336b5b600962d5.png)

（3）点击“确定”按钮，此时会出现如图 4-16 所示的页面，这里记得保存好 Client ID 和 Client Secret 信息。

![](img/ccca53799b2c79d8b3049b75692cccb6.png)

（4）在腾讯云的 OpenClaw 中配置绑定。

![](img/d824267d65b2e2f0802fffc6ee0adfb5.png)

此时在钉钉里面搜索刚刚创建的机器人“OpenClaw 小钉”，打开后，就可以发送消息了。

我们还是发送：“你好，你是谁”，可以看到已经回复消息了，就表示配置成功了，如图所示。

![](img/d8546c61168a5a6fbb39d257c56fcf65.png)

![](img/6fb53ce2d446e501083b9909d4653172.png)

**（四）企业微信接入龙虾**

（1）打开微信管理后台页面：https://work.weixin.qq.com/，扫码登录，如果没有企业，需要先创建一个企业。

（2）打开“管理工具”页面，找到“智能机器人”并点击，如图所示。

![](img/bd3a003767daa06168cd72bc1dd0ec2d.png)

（3）创建机器人。在打开的“智能机器人”页面点击“创建机器人”按钮，如图所示。

![](img/316655717aa61f597da0fdc70aa84d73.png)

（4）此时会打开如图所示的页面，这里选择“手动创建”。

![](img/f3f540227dda238d3a22a28440b1ec7d.png)

（5）划到底部，点击链接“API 方式创建”，如图所示。

![](img/522b6f126b9442c1e705c6c24d5bfd94.png)

（6）在打开的页面中选择“使用长连接”，如图所示，这里的 Bot ID 和 Secret 记得保存起来。

![](img/f6a70064d57a24dd37a243312033c0cd.png)

（7）下一步如图所示，填写机器人名称和机器人简介信息，就可以点击“确定”按钮了。

![](img/e8b22d2f4b13f7068e6fbbc7f63fc482.png)

（8）在腾讯云的 OpenClaw 中配置绑定。如图所示，在腾讯云服务器上粘贴 Bot ID 和 Secret，然后点击“添加并应用”按钮。

![](img/7b9975acbb17d63bea28919cfd9f6d4d.png)

（9）如图所示，点击右上角的三个点，获取二维码，使用手机企微扫一扫，就可以打开机器人聊天窗口了。

![](img/cba8b55034581becfdab2fde12fb6fc2.png)

（10）打开 OpenClaw 机器人对话后，发送消息：“你好，你是谁”，如果可以看到机器人回复消息，就表示已经配置成功了，如图所示

![](img/41c57b230cdf12b69006b26ac624ebe3.png)

2.3其他部署 OpenClaw 方式

💡上面的方式可能对于大家来说步骤还是比较多

建议还是大家用云服务器的方式，灵活安装，如果你已经完成了云服务器部署，可以直接进入到实操板块，下面内容仅做了解**

如果就只是想体验下，还想用本地的环境，还不想配置那么麻烦，那么就可以用这里的方式：

• WorkBuddy：一键安装，算是小龙虾变体，不算是对 OpenClaw 的套壳，本地部署

• QClaw：腾讯手机助手出品，也是唯二支持微信的，本地部署

• 飞书 OpenClaw 一键部署：零配置，一个按钮搞定，一键打通飞书体系的权限，开箱即用，云端部署

怎么选择：

1.  飞书体系，就选飞书 OpenClaw

1.  本地，优选 QClaw，接入微信，一键使用

（一）WorkBuddy（本地可选）

💡也是腾讯出品，是 WorkBuddy 团队收购

注意，这个不是 OpenClaw 的包装，而是 CodeBuddy 产品的包装。

前面讲过，有很多大模型和云计算厂商提供了一键部署小龙虾的产品，这里他们直接把小龙虾产品化了，你部署的只是一个实例，而不需要独立的服务器，这种部署方式最简单也性价比最高，但是可玩性就差一点，比较时候新手用户。

比如智普的 AutoClaw， 腾讯的 WorkBuddy， 火山的 ArkClaw 等，这些产品都是把小龙虾封装进了他们的产品，提供了多个大模型选择

我们这里用 WorkBuddy 的一个主要原因就是它支持接入微信，这样我们在手机上就不用再另外安装其他应用了，微信使用起来也比较方便，当然功能弱一点。

新用户限时赠送 500 积分，零成本上手。

为什么推荐 WorkBuddy？

WorkBuddy 是腾讯推出的全场景职场 AI 智能体桌面工作台。您只需用一句话描述需求，WorkBuddy 便能像同事一样自主规划和执行复杂任务，并交付可验收的结果。

与传统的 AI 对话不同，WorkBuddy 不仅能"听懂人话"，还能"带脑子思考"并"实际操作本地文件"，真正帮您干活。

一键安装：像装普通软件一样，下载 → 双击 → 完成，无需安装 Node.js、无需配置 API Key，支持 macOS 和 Windows

**核心优势**

• 一句话下达任务：用自然语言描述需求，无需复杂操作

• 自主规划执行：自动拆解任务、规划步骤、完成交付

• 多任务并行：支持同时发起和管理多个任务，适合并行处理

• 本地文件操作：可读取授权的电脑文件夹，进行批量处理

• 结果可验收：生成的文档、表格、PPT 等可直接使用

**适用场景**

工作模式 -- 面向职场通用工作场景（默认模式）：

• 文档生成：生成工作报告、技术文档、README 等

• 数据分析：上传数据文件，自动分析和可视化

• PPT/报告生成：从需求描述生成演示文稿和报告

• 深度研究：对复杂问题进行深度调研并输出报告

• 邮件编辑、周报生成等办公场景

• 批量文件处理：自动整理、重命名、转换文件格式

编程模式 -- 面向代码开发场景：

• 日常编码辅助：代码生成、代码审查、Bug 修复、重构优化

• 项目理解：快速了解陌生代码库的架构和逻辑

• 网站/应用开发：从需求到代码的全流程辅助

一键接入企业微信、微信、QQ、飞书、钉钉：

模型随意切换：默认 Pony-Alpha-2，也支持 GLM-5、DeepSeek、Kimi、MiniMax 等任意模型 API

![](img/b86cbfaa8590337bc908dbdf3bbb5a06.png)

![](img/47cd775268d5f61da0e927df5d55a0e9.png)

**一、下载登录**

打开 WorkBuddy 官网https://www.codebuddy.cn/work/， 点击下载 WorkBuddy 就可以看到底部的下载了

![](img/9b57088bd9916c7e6ed9ead08464fd4f.png)

根据你的系统版选择下载

![](img/cc506538e380007a11eb6f5d967d4070.png)

安装之后微信登录

![](img/c99a89bf32352dee0fc5dece2c5edc2b.png)

![](img/78eb7f57def00cfde427677363007ebd.png)

![](img/a9b0a48d48b79925c6e331591e785f6d.png)

**二、开始对话**

![](img/a3dc9531b1f45b2a9714ea49d2610a81.png)

WorkBuddy 是以任务驱动设计的，首先我们需要创建一个任务，右侧选择任务类型

代码开发：面向开发场景

日常办公：日常办公操作场景

然后左侧的 Claw 就是小龙虾本身了，我们可以跟小龙虾对话让他直接干活，我们可以看到 WorkBuddy 直接集成了一个 IDE， 可以进行代码管理和网页预览

![](img/fa4611335a256ed050e5344aae84525a.png)

技能 Sklls，就是给小龙虾调用的技能，已经内置了几十个 Skills，但是好像没有接入 SkillHub（腾讯的 ClawHub 镜像），不过可以支持导入，我们可以从官方市场下载之后导入

![](img/4c599c795ebff1517497ed7bfcde9b84.png)

然后插件，官方已经集成了很多插件，比如浏览器操作 playwiright-cli， pdf ，ppt 操作等

![](img/34c5b48246ee86cf2de528c0fcdb7496.png)

自动化就类似龙虾的定时任务，根据设置的时间定时执行

![](img/61e204c9e9ac6b6cf68b4a093fa95823.png)

点击右上角头像我可以打开个人菜单，看到积分余额

![](img/27a37720a964753fffdc76d8136fd13b.png)

Claw 设置就可以打开设置面板，我们可以在这里配置接入的渠道，微信客服号集成就是我们可以用微信通过 WorkBuddy 的微信客服号跟我们的小龙虾对话

![](img/dac762c3f6d7230a4488e9e799139ddd.png)

然后我们来体验一下编程模式，右侧可以直接预览结果，效果还不错

![](img/8cc49b212a0c68cfe344feefe547c943.png)

![](img/c5e6437b4159d440c51580ce8cc23113.png)

（二）QClaw

💡本地安装的方式

腾讯电脑管家出品。

支持 Windows 和苹果电脑。

集成一些灵感广场，以及很多的 skills，开箱即用。

并且赠送 4 千万 TOKEN，当前是还不需要花费的。

注意：是不能配置自定义模型的 API Key 或者 Coding Plan 的。

浦大喜奔，现在不需要邀请码了

下载地址：https://qclaw.qq.com/

![](img/faf1644b88f35d80bb7474b7b4893f3f.png)

下载后直接点击安装，这里以

![](img/3390f9b0238bc96af808821331da272f.png)

如下图，有安全提示，我们选择"是"。

![](img/2bfa7c7d7e897143abdff465e182e5d8.png)

下一步选择安装位置。等待完成安装就可以。

![](img/dcb4c80c147e84eac25cb18da69281b7.png)

![](img/0133fbdc4276562c59e4758efd92086c.png)

最后点击完成就可以。 完成以后我们看到桌面会有一个 QClaw 的图标。

![](img/0e5d8d37c9bbb00bc595c073987788e9.png)

![](img/6e8b4b34cb2999a8cb6d9e626a4ea7c1.png)

默认是会自动打开 QClaw 的

![](img/bfc0d5dab3342bd9569c413e4e678ea4.png)

进来后如下图，点击左下角的「未登录」按钮， 开始扫码登录你的微信

![](img/a3c526894e176e4672709ab9e863ce7a.png)

开始登录你的微信就行，然后就会出现二维码，使用你的微信扫码登录就可以。

![](img/3cf7efbeb9b811af417760e480a27e85.png)

登录进来后左下角会弹出提醒，让你连接微信。我们点击「关联微信」的按钮就可以。

![](img/34d28b1c5e10037dc84a3b38170f8fc1.png)

微信扫一下中间的二维码就可以。

![](img/23df5971adf36e94222817b6653e0dd6.png)

然后手机上就可以看到有一个 QClaw 客服的微信号。 电脑上的 QClaw 到也可以看见微信连接的提醒，我们点击确定就可以。

![](img/1be2f64657ca18dc281c419d2452680e.png)

![](img/111f8575ddb9cfa73a321fdbf29e66fa.png)

如果是出现如下截图类似的一些错误，我们先可以不用管。我们先去对话客服机器人那里发一下消息。

![](img/be877f5b1526f5a74e7d71f5f7df694b.png)

我们发送一个"你是谁"测试一下。 我我们可以看到手机上也回复了消息，电脑端的 Qclaw 也同步进行了消息的展示。

![](img/d3ae62be26fe757fe6113c7726f2d57d.png)

![](img/637ec89a99198242fa95ec33d3b8472c.png)

好了，基本的 QClaw 的安装就到这里结束。

下面是一些功能的探索，比如左下角的灵感广场。如果你不知道干什么，可以看看灵感广场里面的一些案例，我们直接可以点击具体对应的案例里面就可以用。

![](img/60c0b5d4831372a201958ab418d32f4e.png)

比如我点一个热点资讯自动汇总的，我们点击下面的"立即使用"按钮就可以。

![](img/808feb763493868fa045d83d8280ce59.png)

下面 QClaw 它就会问你一些话，抓取什么内容、什么时间。

![](img/6720d2bd53596ca242c7ab1d50469bb9.png)

我们发送如下类似的消息。 重点就是说下面两个点：

1.  定的时间

1.  需要哪一类相关的新闻。

Markdown

```
每日早上8点抓取全网的AI相关新闻，发送给我
```

![](img/e1baa3be070d570821ee286dc178da48.png)

另外一个功能就是定时任务，比如我们上面让 QClaw 给我们发送 AI 相关新闻的一个定时任务，就是用的这个功能。

![](img/1872be55b9bc7141150517e8db05a526.png)

由于接入微信的渠道目前只有 QClaw 和上面所说的 WorkBody，大家可以探索还有一些什么功能可以使用。

💡就目前来说微信的生态比较封闭，并且添加的机器人是一个客服号，是属于微信的一个二级目录。我们是没有办法去拿进去以及把我们群里的消息转发给这个客服机器人的。这是目前的限制。

![](img/6be2200d80905ffb96f6934c3d57cef8.png)

（三）飞书一键部署 OpenClaw

💡这个方式的要点就是：只点一下，所有环境就都配置好了，包括飞书机器人的权限配置。剩下的操作都不用做。

等待安装完之后通知后就可以直接使用 OpenClaw。

但是需要注意，这个有额度问题，可能问了几个问题后，额度就没有了

飞书官方推出了“妙搭”平台，支持一键部署 OpenClaw。不用买服务器、不用装环境、不用在开放平台配权限——点几下按钮，就能直接在飞书里跟你的智能体对话。

**1.怎么操作**

打开飞书妙搭的 OpenClaw 部署页面：https://openclaw.feishu.cn/home，如图 3-2 所示，点击“创建”按钮就进入创建的步骤。

![](img/636db52752c2c046e35f69dcd17ccd6b.png)

图 3-2 飞书妙搭创建 OpenClaw 助手

提醒：如果没有登录，下一步记得扫码登录飞书。

如图 3-3 所示，创建 OpenClaw 助手，先在“名称”文本框填写助手名称，然后给助手选一个自己喜欢的头像，最后点击“创建”按钮进入下一步。

![](img/45142840133c92d6d365265a4f2fe436.png)

图 3-3 创建 OpenClaw 智能助手

如图 3-4 所示，这就进入 OpenClaw 智能助手创建的步骤，等待就行。

![](img/95ef87725e384c94882f4989cb838691.png)

图 3-4 创建 OpenClaw 智能助手流程

当出现如图 3-5 所示的界面，就表示添加成功了。

![](img/6b5ea81dc76ec9b0c483fd8dec475fff.png)

图 3-5 创建 OpenClaw 助手完成

接着在飞书就会收到 OpenClaw 助手添加成功的消息，如果 3-6 所示。

![](img/63a322e634328d74e5fa0841a369eceb.png)

图 3-6 添加 OpenClaw 助手成功

部署完成后，你会在飞书里看到一个新的机器人联系人。给它发一条消息试试——如果收到了回复，恭喜你，你已经养好了第一只“虾”，如图 3-7 所示。

![](img/eae1aec9890149310fdf0b18659c3b50.png)

图 3-7 你的第一只“虾”

这里最让人省心的是权限配置。以前手动接飞书需要在开放平台创建应用，配置一大堆权限，发布审批——现在这些全部跳过了，妙搭会在聊天框里直接引导你授权，方便得多。

提示：手机上的操作和电脑上差不多，直接在飞书的“工作台”页面搜索“妙搭”应用，进去后点击“一键部署 OpenClaw”，即可开始部署，剩下的操作和电脑端差不多。

**2.免费额度**

飞书妙搭提供自己的内置模型，每天免费 100 万 token（注册首日发放 400 万 token 免费额度）。对于日常体验和轻度使用来说完全够用。云主机配置是单核 CPU、4GB 内存、1TB 硬盘，跑一只“虾”绑绑有余。

目前这个服务是限时免费的，具体截止日期以飞书官方公告为准。

**3.它的限制**

飞书妙搭确实是最快的上手方式，但你需要了解它的边界。

• **模型不能自由选择。**它用的是飞书妙搭自带的模型，你没办法换成 DeepSeek、Claude 或 GPT。如果你对模型有特定偏好，或者需要在不同模型之间切换，这个方案就不太够用了。

• **绑定飞书生态。**你只能在飞书里跟智能体对话。想同时接钉钉、企业微信、QQ？做不到。想通过 Dashboard 直接管理？也不方便。

• **扩展性有限。**自定义 workspace 文件、安装 Skill、配置多智能体等高级玩法，在妙搭平台上的灵活度不如自建方案。

• **数据在飞书平台上。**你的对话记录和配置不在你自己的硬盘里，而是托管在飞书的服务上。

所以，飞书妙搭适合回答一个问题：OpenClaw 到底值不值得我花时间认真搭？

如果你体验了几天，觉得“就这样吧，够用了”——那继续用飞书妙搭也完全没问题。

但如果你发现自己想换一个更聪明的模型，想在钉钉里也能用，想有更大的自定义空间——那就是时候正式搭建一套属于自己的了。

![](img/3a559c2e0a5f82fa72d7c30b5c7fa4d4.png)

2.4 如何养龙虾🦞

（一）领养龙虾的几种方式

![](img/14f67ff1eed41b2e38f3521e6b8876c6.png)

| 安装方式 | 适用场景 | 说明 | 快速链接 |
| --- | --- | --- | --- |
| 一键安装： 各云厂商的养虾套餐 比如智普的 AutoClaw | 零基础用户 | 下载 → 双击 → 注册即用，内置模型和免费额度 | https://autoglm.zhipuai.cn/autoclaw/ |
| 手动安装 | 想完全掌控的用户 | 终端几行命令，自由选择模型和配置 |  |
| 安全优先 / 多智能体 | 隐私敏感 / 团队协作 | IronClaw （WASM 沙盒）/ HiClaw （多龙虾协作） |  |
| 云端托管 / Docker | 服务器部署 | 各大云厂商托管方案 | 火山引擎 9.9 起 腾讯一键部署 |

（二）养虾四步法：雇佣一个 AI 员工的流程

| 流程 | 比方 | 干啥 |
| --- | --- | --- |
| 租房子 | 给员工一个工位 | 安装 OpenClaw（本地电脑或云服务器） |
| 买粮食 | 给员工发工资 | 配置模型 API Key（Token 就是龙虾的&quot;口粮&quot;） |
| 给联系方式 | 让客户能找到员工 | 接入聊天平台（QQ / 飞书 / Telegram） |
| 培训上岗 | 教员工怎么干活 | 配置智能体、工具、定时任务 |

（三）注意事项

**安全：**

安[全风险不容](http://X.com)忽视，一方面是来自小龙虾自身的，因为它的操作权限非常大，比如可以操作你本地的文件，比如会有删除你硬盘文件的风险，之前有小龙虾删除X.com高管邮件的案例，另一方面来自外部，很多人安装好小龙虾没有对服务器做基本的防护，容易被黑客入侵，而下龙虾里又配置了各种 API Key，之前就有公司 Key 被盗刷了几万美元的案例。

所以我们一般推荐小龙虾运行环境与你的工作环境隔离，比如服务器部署或者虚拟机部署，这个我们后面会讲。

**成本：**

给你的 API 调用设置权限和消耗上限，优先使用缓存和本地模型，监控 Token 消耗。

推荐优先使用编程套餐接入，性价比高。

![](img/a3849a84152c54d423aa6bb7ecc117ea.png)

1.  OpenClaw 基础使用场景（小试牛刀）

3.1定时发送新闻总结

💡演示环境：腾讯云轻量云服务器的 OpenClaw 模板

我们需要先安装 skills

Markdown

```
安装这个 https://clawhub.ai/joargp/news-summary  skills，并介绍下当前这个 skills 功能
```

![](img/04f32348e0714ce7c49120c071a457ff.png)

然后比如说如下提示词

Markdown

```
设置每日「8:00」的自动定时任务，
自动抓取全网的今日「AI科技」相关热点、重要资讯与要闻简报，
整理成简洁清晰的内容发送给我。
```

![](img/74ff051d96462fb469aa3b543df6a4e1.png)

![](img/101ddf5c3e52c3f610515addec22eed8.png)

3.2发票归档/单据统计

💡演示环境：腾讯云轻量云服务器的 OpenClaw 模板

这里需要用到的是两个 skills

直接就将下面的提示词发送给小龙虾：

Markdown

```
帮我安装如下两个 skills

https://gitee.com/iamzhihuix/claude-official-skills-mirror/tree/main/skills/pdf
https://gitee.com/iamzhihuix/claude-official-skills-mirror/tree/main/skills/xlsx
```

注意：这里的 skills 是 Claude 官方的 skills，只不过是做了镜像，方便网络不通的同学使用。

![](img/8298bbc4cacfa885a333fbb34bbbde1a.png)

等待它完成以后，它会说明有哪些功能。

我们发送一个发票信息过去，让它整理成报销的格式，如下图：

Markdown

```

这个是我的发票信息，帮我整理成报销的格式
```

![](img/7468a87887f3b5ed2b8e6800e7a510c1.png)

它已经整理成报销的格式，并发给我一个 Excel，我们打开这个 Excel 看看：

可以看到，单子里面的收款方、开户行、账号以及总金额的信息，都是跟原 PDF 里面的发票信息保持一致的。

![](img/45f5aad3148d25f375ac0ec110a213af.png)

附上 excel 原件：

[

![](img/1f45bad69a177710c3f117be8d81ff52.png)

expense_report.xlsx](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/AcszbhHC4o7TqExQgDIcCGjBnUd?response-content-disposition=attachment%3B%20filename%3D%22expense_report.xlsx%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260526%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260526T153247Z&x-oss-expires=86400&x-oss-signature=e8dde14c9c1abeecf1dde524a8b17573c0faeeb43c880fc49fec9338fd0f8d7d&x-oss-signature-version=OSS4-HMAC-SHA256)

注意如果你是本地的 OpenClaw，直接告诉路径就可以

Markdown

```
/Users/happypeet/Downloads/invoice-农耕记.pdf 这个目录下的这个文件
```

![](img/e4fd0731b01c7dcad7561deda85e3f8e.png)

![](img/15a50b8e4734bd05e183de1638cd78c9.png)

3.3论文总结/搜索

💡演示环境：腾讯云轻量云服务器的 OpenClaw 模板

还是老样子，需要先安装 Skills。

让 OpenClaw 小龙虾自己安装。

直接把这些提示词发给小龙虾

Markdown

```
帮我安装下面的两个 skills：
https://gitee.com/iamzhihuix/zhihui-awesome-skills-open/tree/main/skills/arxiv-reader
https://gitee.com/iamzhihuix/zhihui-awesome-skills-open/tree/main/skills/arxiv-watcher
```

等待安装完成

![](img/e4afd2bed78d393c29ff21f11d06f9eb.png)

让小龙虾给我们介绍一下这两个 skills 如何使用。

![](img/a13dafddd430b3f6b3a978da5a254ead.png)

比如让他帮我们搜索一下关于 LLM Agent 的一些情况怎么样？

Markdown

```
最近一周有哪些关于LLM Agent的新论文？
```

![](img/f49d78e109e520224003241284609bf9.png)

可以看到，给我们近期的 LLM Agent 的笔记列表。

并且他给了我们提示，我们可以直接发送他的 ID 让他获取详细的内容。

![](img/9f95a20d51a3e41ea96e3e750ea85192.png)

到这里我们就完成了论文搜索，以及针对某一篇论文的详细阅读理解。

如果下面有一些新的想法，可以根据他的提示来继续操作，就可以继续跟 OpenClaw 小龙虾对话了。

### 02.实战：OpenClaw 典型场景实战应用

1.用 OpenClaw 打造你的个人专属知识库

你有没有想过，如果把梁宁、刘润和华杉同时请到你的办公室，让他们针对你当下的难题辩论半小时，是种什么样的感觉？

以前这叫白日做梦。现在，这个通过专属知识库就能实现。

在 OpenClaw 的运行逻辑里，每一本你读过的书、每一篇你收藏的干货，都不是死文字，而是一个活的数字分身。

当你问出一个关于品牌的问题：

• 华杉会跳出来跟你讲**超级符号**；

• 刘润会从底层逻辑**拆解成本**；

• 梁宁则会提醒你注意用户的**确定性依赖**。

你不是在翻笔记，你是在主持一场顶级智囊团的圆桌会议。

这一章，教你用 30 分钟，把那些躺在收藏夹里的作者激活，让他们 24 小时待命，随时为你 Battle。

搭建时间：**30 分钟**。一次搭好，终身使用。

**你需要准备什么？**

开始之前，确认以下三件事：

• 一台腾讯云轻量应用服务器（已安装 OpenClaw）

• OpenClaw 已配置好模型，能和 AI 正常对话（我们这里展示用的是飞书来和小龙虾交流，你用其他 IM 也行）

• 一个微信公众号（个人订阅号就行，用于登录文章导出工具）

不需要编程基础。下面的每一步都有完整操作说明，照着做就行。

第一部分：配置 OpenClaw 模型

如果你的 OpenClaw 还没配置模型，先完成这一步。已经配好的可以跳过。

1.1 购买 MiniMax Coding Plan

OpenClaw 需要一个 AI 模型来驱动对话。我们用 MiniMax，国产模型里的性价比产品。

1.  打开浏览器，访问 MiniMax 开放平台，注册并登录

1.  **进入「套餐管理 → Co**ding Plan」，购买Starter 月度套餐（29 元/月）

◦每 5 小时 40 次对话，日常知识库问答完全够用

1.  购买后，在同一页面找到**API Key**（以sk-cp-开头），点击「复制」

![](img/67a71e7e8ebd45cfbcedb4ffacbdc3a6.png)

1.2 在 OpenClaw 中配置模型

1.  打开腾讯云轻量应用服务器的 OpenClaw 管理页面

1.  在「模型 （Models）」区域：

◦第一个下拉框选择：MiniMax（国内-Coding Plan）

**◦**第二个下拉框选择：**MiniMax M2.5（最新旗舰模型，质量最好）

1.  填入你刚才复制的 API Key

1.  点击添加

1.3 配置飞书通道

1.  在「通道 （Channels）」区域，选择飞书

1.  按照提示完成飞书机器人的创建和绑定

1.4 验证

在飞书里找到你刚创建的机器人，发一句"你好"。如果它回复了，说明配置成功。

![](img/3b1298fd584c20d3fc68435e2f64ba9a.png)

![](img/c68385ebe6e0af2ccc084962ff72845c.png)

第二部分：准备你的内容素材

知识库的质量，取决于你往里面喂了什么。垃圾进，垃圾出。精华进，智慧出。

本教程用 4 位商业大 V 的公众号文章做演示。你完全可以换成自己的弹药：读书笔记、行业研报、竞品分析，任何你觉得以后肯定用得上的内容。

2.1 导出公众号文章

我们用一个免费的在线工具来批量导出公众号文章，打开网页就能用，不需要安装任何东西。

**前提条件**

：你需要一个微信公众号（个人订阅号就行，免费注册）。没有的话，去微信公众平台注册一个，5 分钟搞定，或者用朋友的扫个码也行。

**第一步：打开工具，扫码登录**

1.  在浏览器中打开https://down.mptext.top

1.  点击左下角「登录公众号」

1.  用微信扫描二维码，选择你自己的公众号完成登录

![](img/8ff55e72cec8c519dd2488b21f0920d6.png)

**注意：扫码**登录只是为了获取接口权限。登录后可以搜索和导出任何公众号的文章，不限于你自己的。

**第二步：添加你想导出的公众号**

1.  点击顶部的「添加」按钮

1.  在搜索框中输入公众号名称，比如"刘润"

1.  在搜索结果中点击对应的公众号

![](img/20262b000ec6e1ad8c38824f9284baa8.png)

系统会自动开始同步该公众号的文章列表。

![](img/49f296a4731798a172cd1eb8f387da6e.png)

你可以按这个方法添加多个公众号。本教程的演示知识库包含以下公众号：

![](img/8ea6cc1d285b7bfd0e36e42ea6475e81.png)

**第三步：抓取文章内容**

1.  点击左侧「文章下载」菜单

1.  在顶部下拉框中选择一个公众号

1.  勾选你想导出的文章（点击表头的全选框可以全选）

1.  点击右上角「抓取」→ 选择「文章内容」

![](img/25cf55ece76c00f998bf7759e65fc07e.png)

系统会开始逐篇抓取文章正文，你可以看到进度。

第四步：导出为 Markdown

抓取完成后：

1.  再次全选文章

1.  点击「导出」→ 选择**Markdown**格式

![](img/a06752341611fb7e325de5a963b54c8b.png)

1.  浏览器会提示你选择一个文件夹保存，选好后点确认。导出完成后，你会得到一个文件夹，里面是每篇文章的.md文件。

![](img/ce894809222e811355ec7c9a358906d6.png)

![](img/c7b8cbcd893be61fb199aa3e7ce76d8b.png)

第三部分：搭建知识库

这一部分是核心。但别紧张，你不需要懂任何技术，全部交给 AI 来做。你只需要复制粘贴几段话。

为什么不能直接让 AI 读文章回答问题？

想象你有一书柜的书。你不可能每次问问题，都让 AI 从第一页翻到最后一页。所以我们先给这些文章建一套"索引"，就像图书馆的编目系统。

AI 会把文章切成小段，给每段做一个"语义指纹"，存进数据库。以后你提问时，AI 拿你的问题去比对指纹，几秒钟就能找到最相关的那几段。不是关键词匹配，是理解意思的匹配。

效果就是你问"小公司怎么跟巨头竞争"，它能找到讲"破坏性创新"的那段，虽然原文里压根没出现"小公司"三个字。

3.1 压缩文章，发给 AI

不需要手动整理目录，也不需要自己上传服务器。我们把文章打包发给飞书里的 AI，让它全自动处理。

注意：飞书不支持直接发送文件夹，需要先压缩成 。zip 文件。

1.  找到你刚才导出的文章文件夹

1.  右键 → 压缩（Mac）

或 发送到 → 压缩文件夹（Windows）

1.  打开飞书，找到你的 OpenClaw 机器人

1.  把压缩好的 。zip 文件拖进对话框发送

![](img/865465843770e036b0d26e0fb56c7187.png)

3.2 发送搭建指令

发完 zip 文件后，把下面这段话复制粘贴发给 AI：

Plain Text

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

AI 会开始逐步执行。你会看到它自动完成以下工作：

• 解压文件，列出所有文章（按作者分类）

• 安装 Python 依赖

• 把文章保存到工作目录

• 写好切片脚本并运行，生成数千个文本片段

• 写好向量化和查询脚本，等你提供 API Key

![](img/ad528bd59e04880724a9079710a2096e.png)

**这一步需要耐心等待。**

AI 需要处理所有文件、写代码、运行脚本，整个过程大约 10-15 分钟。如果你的知识库内容更多（比如几十本书），可能需要 20-30 分钟。不用担心 AI 没有反应，它在后台默默干活。去喝杯咖啡，回来就好了。

3.3 注册硅基流动，获取 API Key

AI 执行到第 5 步时会停下来，问你要硅基流动的 API Key。这个 Key 是用来做向量化的，把文字翻译成 AI 能理解的数字。

我们用硅基流动（SiliconFlow），原因很简单：国内直连、注册只需手机号。

1.  打开浏览器，访问 cloud.siliconflow.cn

1.  用手机号注册并登录

1.  **完成身份认证**（重要！）：进入「账号管理」→「实名认证」，完成实名认证。未认证的账号有严格的请求频率限制，向量化过程会报错RPM limit exceeded

1.  登录后，点击左侧「API 密钥」→「创建新的 API 密钥」

1.  名称随便填（比如"知识库"），点创建

1.  复制生成的 Key（以sk-开头的一串字符）

![](img/a67b87b70e578001fd83ed5ef86c9cd2.png)

这个 Key 非常重要，丢了就得重新创建。建议先存到备忘录里。

3.4 提供 Key，完成向量化

把 API Key 发给飞书里的 AI：

Plain Text

```
硅基流动 API Key：（sk-你的真实Key粘贴在这里）
请继续运行向量化脚本。
```

![](img/e99cfb4143d2b5743133fa88e6508dcb.png)

AI 会用这个 Key 运行向量化脚本，把所有文本片段转成语义向量存入数据库。这一步根据内容量不同，需要 2-15 分钟。

完成后，AI 会告诉你知识库搭建成功，并显示总共处理了多少个片段。

![](img/b8d735623859b2f4891aef167c209bed.png)

3.5 让 AI 创建知识库 Skill

向量化完成后，还需要让 AI "记住"这个知识库，以后你每次提问它都会自动去检索。在飞书里发这段话：

Plain Text

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

AI 会自动创建 Skill 文件并确认。

![](img/9425716f5e987f07e9e338ad24ebc650.png)

3.6 实测

知识库搭好了，试一下效果。在飞书里问：

Plain Text

```
小公司怎么跟大公司竞争
```

![](img/64ecfeade7b056704f2073ae3e853f0e.png)

注意看 AI 的回答。它从 3 位不同作者的文章里分别找到了相关观点：

• **刘润**讲差异化战略，引用了他关于"蓝海战略"的原文

• **华与华**讲聚焦根据地，引用了"无论规模大小，都要有一块别人拿不走的根据地"

• **黄有璨**讲小而美，引用了他关于"一人公司"的思考

最后还整合出了一个结论：不要正面硬刚，找细分领域建立根据地。

这就是知识库真正厉害的地方。这些作者从来没有坐在一起讨论过"小公司怎么竞争"这个话题。但 AI 从他们各自的文章里，提炼出了各自的思维框架，拼出了一个谁都没单独给过你的答案。

而且每个观点都标了出处，不是瞎编的，你可以回去翻原文验证。

**没有知识库的 AI**

，像一个什么都知道一点但什么都不深的泛泛之交。

**有了知识库的 AI**

，像四个你读过的作者同时坐在你对面，各抒己见。

![](img/01131f802bc948300f3f12644ba59c51.png)

第四部分：进阶玩法

4.1 新增内容

你的知识库，并不是“死的”，而是可以不断更新迭代的。以后想往知识库里加新文章，重复第二部分的导出流程就行：

1.  用https://down.mptext.top导出新文章为 Markdown

1.  压缩成 。zip 发给飞书里的 AI

1.  告诉它：

Plain Text

```
我新增了几篇文章，请添加到知识库里，重新切片和向量化。
```

AI 会自动处理。已有的内容不会重复处理。

注意：不能直接发公众号链接给 AI，微信文章有访问限制，AI 读不了。必须先用导出工具把文章下载下来。

4.2 跨来源关联查询

这是知识库最有价值的能力。展示一些值得一试的问法：

Plain Text

```
知识库里所有作者对&quot;用户增长&quot;这件事，有没有互相矛盾的观点？
```

![](img/7e2ae4f118756ce8204d21e42e718ea9.png)

这种提问方式是单个 AI 做不到的。它需要从你的知识库里真正检索、对比、整合多个来源的原文。

4.3 调整沟通风格，固化到工作流

你可能会发现刚刚 AI 的回答的那个问题，读起来像论文，一板一眼、引经据典，不太好消化。

这时候你可以直接告诉它你想要的风格：

Plain Text

```
我发现目前你给我的答案，读起来像是论文，非常费力。能不能调整一下？我希望能像朋友吃着小龙虾喝着啤酒在给我唠嗑的感觉。
```

![](img/260db7047795cf8e5923d62fb491401a.png)

**AI 会立刻切换风**格。但接下来，你需要做的更重要的事情是——把这个调整固化下来，否则下次对话又会恢复原样。

告诉 AI：

Plain Text

```
请帮我把这个调整，记录在对应的工作流程里
```

![](img/f08079d019c93347d4d5400a7516d0b9.png)

AI 会把你的偏好写入[AGENTS.md](http://AGENTS.md)（工作流程规范）和[SOUL.md](http://SOUL.md)（AI 人设），以后每次对话都会自动用这个风格。

这个"调教"能力非常有用。你可以随时调整 AI 的回答风格、详细程度、语气，然后让它记住。比如"回答控制在 200 字以内"、"多用类比少用术语"、"每次回答先给结论再展开"。说一次，永久生效。

4.4 你还能放什么进去

教程用公众号文章做示例，但知识库能装任何文本内容：

![](img/f0de32832b558e44b66fee909a17f569.png)

关键不在于放什么，而在于：当你积累够多的时候，知识库会开始给你"意料之外的关联"，那种你自己翻笔记翻一年也想不到的关联。

附录 A：NotebookLM 路线（需要能访问 Google 服务）

如果你能访问 Google 服务，NotebookLM 是一个更好的方案。不需要跑任何代码，不需要服务器，在浏览器里上传文件就能用。

**跟本地 RAG 方案的对比：**

![](img/2e931df30d2956498d936ef4e24117c5.png)

**两个方案不冲突**

，你可以同时用。比如日常在 NotebookLM 里快速查询，遇到需要大规模检索的场景（上百篇文章）再用本地 RAG。

**A.1 快速上手**

1.  打开浏览器，访问 notebooklm.google.com

1.  用 Google 账号登录

1.  点击「新建笔记本」

1.  点击「添加来源」，上传你的文件（支持 PDF、TXT、Markdown、Google Docs、网页链接）

![](img/6ef6f3977f2ded9d1a0244b90d69e1a7.png)

1.  上传完成后，直接在下方的输入框里提问

试一下这个问题：

Plain Text

```
刘润最近的文章里，有没有观点跟他以前的说法矛盾的地方？
```

![](img/d3edb2f6107ee1e99a73e8c326dff8d7.png)

注意看回答的深度。NotebookLM 找到了刘润在不同时期对同一件事的不同态度：

• **关于 OKR**：早期说"忘记复杂数字，管理要简单"，最近却说"管理必须量化，OKR 要设得繁复严密"

• **关于人才培养**：一边说"成年人只能筛选，不能教育"，一边又引用"We hire for attitude， and train for skill"

NotebookLM 不只是找到了矛盾，还给出了深层解读：这些"矛盾"其实是刘润针对不同管理痛点的演进，从宏观的心智建设下沉到了微观的防范人性漏洞。

这种"同一个作者的观点自我对比"能力，是 NotebookLM 理解力的最佳体现。它真的读懂了内容，不是在做关键词匹配。

A.2接入 OpenClaw（可选）

如果你想在飞书里直接查询 NotebookLM 的内容（而不是每次都打开浏览器），可以把它接入 OpenClaw。

在飞书里给 AI 发这段话：

Plain Text

```
请帮我安装 notebooklm CLI 工具，然后接入我的 NotebookLM 笔记本。
我会提供 Notebook ID，你帮我配置好，让我以后可以在飞书里直接查询。
```

![](img/b30b073192ea4cd1569bd01c8405ba53.png)

AI 会引导你完成安装和配置。你需要提供的是 NotebookLM 笔记本的 ID（在浏览器地址栏里可以找到）。

配置完成后，你就可以在飞书里这样提问（我这里就不具体展开啦，大家感兴趣去试试～）

Plain Text

```
从 NotebookLM 里查一下：刘润怎么看&quot;底层逻辑&quot;
```

附录 B：常见问题

Q：向量化报错 RPM limit exceeded

硅基流动对未实名认证的用户有请求频率限制。解决方法：去cloud.siliconflow.cn→「账号管理」→「实名认证」，完成认证后重新运行。

Q：飞书里发文件夹给 AI，提示读取不了

飞书不支持直接发送文件夹（发的其实是云空间引用）。解决方法：先把文件夹压缩成 。zip 文件再发。

**Q：AI 处理文件时一直没反应**

正常现象。解压、切片、写脚本需要时间，内容多的话可能要 10-30 分钟。耐心等待，不要重复发消息打断它。

**Q：查询结果不准确**

几种可能：

• **内容太少**：知识库里就几篇文章，效果不如内容丰富时好。建议至少放 10 篇以上。

• **问法太泛**：把问题问得更具体。"商业策略"太宽泛，"初创公司在资金有限的情况下如何做品牌定位"更好。

**Q：知识库数据会不会上传到云端**

不会。你的文本内容和向量数据全部存在服务器上。唯一的网络请求是调用 Embedding API 把文本转成向量，发送的是 500 字的片段，不是你的完整文件。

**写在最后**

搭这套系统之前，你读过的书、收过的文章，像沙子一样散落在各个角落。你知道自己好像在哪儿看过一个类似的观点，但就是想不起来在哪

搭好之后，这些沙子变成了一张网。每一篇文章都是一个节点，每一次提问都可能触发一次你从未预想过的连接。

有一天你随口问了一个问题，AI 从你三个月前存进去的一篇文章里翻出一段话，刚好和你今天思考的问题形成了呼应。

那个时刻你会明白：AI 时代的学习方式，已经彻底改变了。

![](img/29a5f8702673f247cdf1035fc6c5a14d.png)

2.用 OpenClaw 跑通个人 IP 公众号自动化

**注意：本案例难度较大，大家可以在打造专属知识库和个人 IP 公众号自动化里只选择一个案例完成即可（新手推荐**完成第一个案例后即可），其他的作为拓展学习内容，不需要全部都完成，21 天里，完成一个 Open Claw 案例即为收获

AI 写文章最大的问题不是写得差。恰恰相反，它写得太好了。

好到每一句都通顺。好到结构永远清晰。好到从不犯语法错误。好到你读完会觉得——这是一篇标准答案。

但是，如果你要做一个 IP

你发公众号，就不是在交作业。你的读者关注你，是因为你说话的方式跟别人不一样。他们想看的是你的偏见、你的口头禅、你的坏脾气——不是一篇无功无过的机器文本。

这篇教程教你一件事：怎么让 AI 写出来的东西，带上你自己的味道。

**前提**

：你已经有一个在跑的 OpenClaw 实例（还没有的话先看部署教程）。

💡两条路径：选适合你的节奏

这篇教程内容不少，但你不需要一口气全做完。根据你的时间，选一条路径：

快速路径（30 分钟，先跑通核心）

：Step 1 中的 1.1-1.3 快速建一份风格配置 → 用它写一篇短文验证效果 → 发到草稿箱。30 分钟内你就能看到一篇带你风格的 AI 文章出现在公众号草稿箱里。体验到了再决定要不要往深了搞。

完整路径（3 小时，全链路搭通）

：Step 1 到 Step 6，包括素材采集、配图、定时任务——所有环节走一遍，搭成一条真正能日常运转的流水线。

建议先走快速路径。尝到甜头再回来补全。

**开始前准备**

动手之前，先确认这几件事都就绪了。别跑到 Step 2 才发现网络不通，那很扫兴。

![](img/28b9b3b6150a2e137f0ad28b021b311e.png)

**工作原理**

一条线串起来：

Plain Text

```
素材采集（Tavily + MediaCrawler）→ 风格化写作（三层架构）→ 配图（封面+内文）→ 排版（HTML）→ 发布（草稿箱）
```

核心差异在中间那一步。用一个比喻讲清楚：

把 AI 想象成一个文笔极好但没有个性的代笔人。你需要给他三样东西：

• **第一层 · 风格指南**：告诉他你是谁——你的说话习惯、用词偏好、段落节奏

• **第二层 · 范文样本**：给他看你写过的好文章——不是描述风格，而是直接展示

• **第三层 · 禁忌清单**：告诉他你绝不会这样说——比如你不会用"综上所述"，不会用"让我们深入探讨"

三层叠加之后，10 篇文章发出去，你朋友分不出哪篇是 AI 写的。

具体的架构图和 Skill 清单放在文末附录了，现在不用看。先动手。

**搭建步骤总览**

![](img/6440f6a87e5a5fb36b5736e1310c0a5d.png)

总计：首次搭建约 3 小时，之后每篇文章 10-15 分钟

Step 1：建立你的风格档案

【声明】

本教程以咪蒙的公开作品为例演示流程，选择她是因为写作风格辨识度极高，便于展示三层配置的效果差异。**这不代表推荐她的写作策略。**教程演示的是如何让 AI 学会一种风格的方法，至于学什么风格、用什么价值观写作，由你自己决定。请勿将任何人的风格配置用于冒充他人身份发布内容。搭建你自己的风格档案时，请使用你自己的素材。

后面五个步骤加起来 1 小时。这一步你可能要花 2 小时。

但如果你跳过这 2 小时，后面那 1 小时只会帮你更高效地生产 AI 垃圾。

[

![](img/598d568199b01bc40ea3ff6ff959bbf0.png)

咪蒙文章.txt](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/VOhxbkXq1olNODxZjRTc4fT1nRg?response-content-disposition=attachment%3B%20filename%3D%22%E5%92%AA%E8%92%99%E6%96%87%E7%AB%A0.txt%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260527%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260527T011932Z&x-oss-expires=86400&x-oss-signature=26fba0d85ed179ff3a083434de74977458f99ab33c23d246b32e4573009c8a57&x-oss-signature-version=OSS4-HMAC-SHA256)

[

![](img/e29a45250032ccdfaad1d9727c10264c.png)

咪蒙精选30篇.md](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/MaAbbYnCpoKkhCxEqQ7cSDqvnkh?response-content-disposition=attachment%3B%20filename%3D%22%E5%92%AA%E8%92%99%E7%B2%BE%E9%80%8930%E7%AF%87.md%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260527%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260527T011932Z&x-oss-expires=86400&x-oss-signature=2b4961774ff8ab3412feff5272e2e8c9ac9c7cd426279276b7929515639d2d46&x-oss-signature-version=OSS4-HMAC-SHA256)

[

![](img/bf667c5a3777b5121790431a3f74336c.png)

咪蒙风格DNA分析报告.md](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/SOGmbp0WHoJ8NFx05fZc4NKxnUg?response-content-disposition=attachment%3B%20filename%3D%22%E5%92%AA%E8%92%99%E9%A3%8E%E6%A0%BCDNA%E5%88%86%E6%9E%90%E6%8A%A5%E5%91%8A.md%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260527%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260527T011932Z&x-oss-expires=86400&x-oss-signature=1a3100a3dbe81a4de096fd654b846a7bc12d0a2893c418d0d7434eb5fa28f4ca&x-oss-signature-version=OSS4-HMAC-SHA256)

1.1 收集个人语料

你在微信群里认真打字的时候——不是回复"好的""收到"，而是突然来了兴致，噼里啪啦敲了三百字那种——那个就是你的风格。

大部分人跳过这一步。他们直接在 prompt 里写"用轻松幽默的口吻"，然后抱怨 AI 写出来不像自己。你连自己是什么样都没告诉它，它怎么像你？

**你需要收集的素材**

（越多越好，最少 10 篇）：

• **历史文章**：你以前写过的公众号文章、博客、朋友圈长文

• **聊天记录**：你在微信群里的长段输出（那种你认真打字的时候）

• **语音转文字**：你的语音日记、会议发言、播客录音

• **演讲稿/分享 PPT 的备注**：你在公开场合说过的话

把这些素材统一放到一个文件夹：

Plain Text

```
# 在 OpenClaw 中说：
帮我创建一个文件夹 ~/Documents/我的风格语料库，用来存放我的写作素材
```

然后把你的历史文章、聊天记录截图转文字等放进去，每篇一个 。md 或 。txt 文件。

验证：

Plain Text

```
# 在 OpenClaw 中说：
帮我看看 ~/Documents/我的风格语料库 目录下有多少个文件
# 输出应该 &gt;= 10，少于 10 篇效果会打折扣
```

**没有历史文章怎么办？**

随便找 5 个你关心的话题，坐下来手写 5 篇 500 字以上的短文。不用排版，不用润色，想到什么写什么——这才是你的声音。

案例演示：如何收集和清洗公开人物的语料（以咪蒙为例）

如果你想先用一个风格鲜明的公开人物做练习，素材收集流程是这样的：

**第一步：找到素材源**

公开人物的文章通常有网友整理过合集（PDF、TXT、网盘分享）。我们拿到的咪蒙合集是一个 13.8 万行的 txt 文件，包含 900+ 篇文章。

其他常见素材源：

• 微博长文（手动复制或用 MediaCrawler 抓取）

• 演讲视频（下载后用 mlx-whisper 转文字稿）

• 书籍（微信读书、Kindle 等电子版）

• 知乎/博客历史文章

**第二步：筛选代表作**

合集里什么都有——广告软文、团队成员写的、带货文、水文。你需要筛选出最能代表本人风格的纯观点文。

我们的筛选标准：

• 只保留本人署名的文章（过滤掉团队其他成员的）

• 只保留观点文/情感文/社会评论（过滤掉超过 50% 篇幅在推荐商品的软文）

• 覆盖不同主题（感情、职场、社会现象、自我成长等）

• 最终选出 30 篇

在 OpenClaw 中，你可以直接让 AI 帮你筛选：

Plain Text

```
请读取 ~/Documents/咪蒙合集.txt，从中筛选出 30 篇最能代表咪蒙写作风格的纯观点文章。
筛选标准：必须是咪蒙本人署名，不是带货软文，覆盖不同主题。
保存到 ~/Documents/我的风格语料库/咪蒙精选30篇.md
```

**第三步：清洗噪音**

网友整理的合集里通常夹带私货——整理者的公众号二维码、微信号、小广告。这些必须清理掉：

• 删除整理者署名和水印（如"WCplus"、"数据部落"等）

• 删除淘口令（￥...￥）

• 删除图片占位符（《《 向左滑动查看图片 》》）

• 如果文章末尾几段突然变成产品推荐，截断到观点部分结束

清洗完的 30 篇文章，约 9 万字，就是你的分析语料库。

1.2 分析风格 DNA

素材有了，接下来让 AI 帮你把风格翻译成它能理解的语言。

直接说：

Plain Text

```
请读取我接下来发你的所有文章，按照以下维度分析我的写作风格 DNA：
```

然后接上下面这套分析框架。这套框架不只看句子怎么写，还看思维怎么转——调性、洞察偏好、表达招数、句式节奏一起拆：

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

AI 输出的报告里应该有具体的原文引用，不是泛泛而谈。如果全是"您的文风轻松幽默"之类的废话，说明语料太少或者太同质，补充更多素材重新跑。

1.3 生成三层风格配置

分析完之后，把结果整理成三个文件。

**文件一：**风格指南.md（第一层 · System Prompt）

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

**文件二：**范文样本.md（第二层 · Few-Shot）

从你的语料中精选 3-5 篇最能代表你风格的文章，完整放入。

选范文的标准：

• 你自己看了觉得这篇就是我

• 涵盖不同类型（观点文、故事文、干货文各挑一篇）

• 每篇至少 800 字（太短 AI 学不到节奏感）

**文件三：**负面约束.md（第三层 · Anti-Slop）

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

关于第三层，推荐一个省力的做法：Ruben Hassid 的方法。去 Wikipedia 搜 "Signs of AI writing"，把整篇文章复制下来，直接作为负面约束的底稿。他的原话是："模型不需要知道你听起来像什么——它需要知道你永远不会听起来像什么。"你自己的禁止清单再叠加上去，效果更好。

**别指望一次就到位。**

风格配置是迭代出来的，不是一次性生成的。正确的节奏是这样的：

1.  用三层配置让 AI 写一篇

1.  读完之后，标出这句不像我的地方

1.  回去更新风格指南或负面约束

1.  再写一篇，再对比

循环几轮之后你会发现，到第 5 次左右 AI 的输出开始稳定了，到第 10 次以后一致性甚至超过你自己手写——因为你手写有情绪波动，它没有。

如果你嫌手动迭代麻烦，可以试试开源工具cw-style-skill-creator（haowjy/creative-writing-skills），它能从你的语料自动提取风格指南并生成 Claude Skill，省掉不少来回调的时间。

验证：三个文件都创建好了没？

Plain Text

```
# 在 OpenClaw 中说：
帮我确认 ~/Documents/我的风格语料库/ 目录下是否有这三个文件：风格指南.md、范文样本.md、负面约束.md
```

1.4 案例演示：咪蒙风格三层配置

为了让你直观感受三层架构的效果，我们用咪蒙的 30 篇代表作做一个完整的演示。她的风格辨识度极高，Before/After 差异一目了然。你搭建自己的风格档案时，把咪蒙换成你自己就行。

**咪蒙风格指南（第一层）**

：Markdown

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

**咪蒙范文样本（第二层）**

—— 从 30 篇中精选 3 篇代表作（社会评论类《你支持的不是蒋劲夫，是家暴！》、情感类《我把你当老公，你把我当子宫》、自嘲幽默类《我，一个矮子的史诗》），完整正文放入配置文件。

**咪蒙负面约束（第三层）**

：Markdown

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

1.5 Before / After 对比

光说三层配置有用太抽象。同一个主题——为什么 AI 写的公众号文章都很难看——我们看看不加配置和加了三层配置之后的差异。

不加任何风格配置，直接让 AI 写：

在当今 AI 时代，越来越多的创作者开始使用 AI 辅助写作。然而，许多人发现 AI 生成的公众号文章往往缺乏个性和温度。这主要有以下几个原因：首先，AI 缺乏个人经历和情感体验；其次，大多数用户未能提供足够的风格引导；最后，AI 模型本身倾向于生成安全、中庸的内容。值得注意的是，这并不意味着 AI 不能写出好文章，关键在于如何正确地引导它。

典型的 AI 八股文。"在当今""首先其次最后""值得注意的是"——每一句都是 AI 的安全牌，每一句都让人想划走。

加了咪蒙三层配置后，同一个 AI 写：

前两天有个做公众号的朋友，花了 3000 块买了个"AI 自动写文章"的工具。

我问他效果怎么样。

他说，生成倒是挺快的，十分钟一篇。

然后呢？

然后他把那十篇文章发给我看了。

特么的，十篇读起来像同一篇。都是"在当今 AI 时代"开头，都是"首先其次最后"三段论，都用"值得注意的是"转折，最后都来一句"希望对你有所帮助"。

我说，这不叫写文章，这叫 AI 在做完形填空。

（他还反驳我：你看，它连排版都帮我做好了！我：……排版做得再好，内容像机器人写的有什么用？你把屎摆成米其林摆盘，它还是屎啊。)

说真的，AI 写文章最大的问题，不是写得不好。是写得太好了。好得没有一丝人味儿。没有偏见，没有情绪，没有那种这话只有你会这么说的辨识度。

你的读者关注你，是因为你会说"卧槽这也太离谱了"，而不是"这一现象值得我们深入思考"。

感受到差距了吧？同一个模型，同一个主题。前者是 AI 在写作文，后者是一个有脾气的人在跟你吐槽。短句、口语、自嘲、括号内心独白、比喻接地气——这就是三层风格配置的效果。

1.6 小试牛刀

在进入 Step 2 之前，先拿你刚建好的三层配置练一把手。

在 OpenClaw 中说：

Plain Text

```
请读取 ~/Documents/我的风格语料库/ 下的风格指南.md、范文样本.md 和负面约束.md，然后用这个风格写一段 200 字的短文，主题是&quot;为什么大部分人学不会 AI&quot;
```

主题随你换——你最近关心什么就写什么。

读完之后，问自己一个问题：如果这段话混在你的朋友圈里，你的朋友能认出这不是你写的吗？

如果答案是能认出来，回到 1.2 调整风格指南，重复测试。这个调试过程通常需要 2-3 轮，别急。

如果答案是差不多了——好，风格这关算过了。

我自己的体感是：只有风格指南，输出大概六成像我；加上范文，能到八成；再加负面约束，基本九成以上——剩下的一成靠发布前人工微调。三层缺一层，效果都会明显掉档。

![](img/8b0bd0db016b6bd7afc102a3d0fdfb88.png)

Step 2：给你的 AI 装上眼睛

写文章最怕的不是写不好，是不知道写什么。

你不是在洗稿，你是在逛菜市场——挑食材，回家做自己的菜。这一步就是帮你搭一个自动逛菜市场的系统：你什么都不用做，每天早上醒来，一份新鲜选题已经躺在桌上了。

2.1 入门版：3 分钟装好，够用了（推荐新手）

只需要一个工具：**Tavily Search**。它是一个专门给 AI 用的搜索引擎，一个 API Key 就能搜全网，OpenClaw 社区公认的必装工具。

**第一步**

：打开[tavily.com](https://www.tavily.com/)**，注册账号，复制你的 A**PI Key。完全免费，不需要绑信用卡，注册就送每月 1000 次搜索额度（公众号日更每天搜 3-5 次，一个月才 100 多次，绰绰有余）。

装不了 Tavily？没关系

如果你因为网络原因无法访问[tavily.com](http://tavily.com)**或拿不到 AP**I Key，可以跳过这一步，不影响后续流程。Step 2.2 的 MediaCrawler 不依赖任何 API Key，直接就能采集国内各平台的内容。Tavily 是锦上添花，MediaCrawler 才是核心。

**第二步**

：在 OpenClaw 对话中说：

Plain Text

```
帮我安装 Tavily 搜索工具，API Key 是 xxxxxxxxxxxxx(填写你的key)
```

![](img/89b28dc564f63b8dab03be47cba9728f.png)

![](img/a04da62044f9f689241e1cfdfb54f296.png)

**第三步**

：试一下

Plain Text

```
# 在 OpenClaw 中说：
帮我搜索一下最近一周&quot;公众号自动化&quot;相关的热门讨论，重点看用户的痛点和吐槽
```

几秒钟后你会看到搜索结果——全网的公开讨论、帖子、文章，已经整理成结构化摘要了。这些就是你的写作素材。

![](img/d9ab905860df64e496484483b3a696a5.png)

![](img/0e1d59d073128f866dd0a7a02f4f8916.png)

Tavily 的本质是 Web 搜索，能搜到被搜索引擎索引的公开内容。它不能像专用爬虫那样直接抓小红书评论区或 B 站弹幕，但对于找选题、找素材来说，完全够用。先跑通流程比覆盖所有平台重要。

![](img/fdc4f94af2ee3d991ee6956bce7b35cc.png)

2.2 进阶版：MediaCrawler 国内平台深度采集（推荐）

Tavily 能搜到公开内容，但小红书评论区、B 站弹幕、微博热评这些——搜索引擎压根索引不到。你需要一个能钻进这些平台捞评论的工具。

**MediaCrawler**

是目前最热门的开源社交平台采集工具（GitHub 4.3 万+ Star），一套工具覆盖 7 个国内主流平台：

![](img/a1d7f9559da94b3b3a6a58aed06ffe4b.png)

**不需要全部登录。**

你有哪些平台的账号就登哪些。小红书 + B 站 + 微博三个平台的素材已经非常够用了，其他的是加分项。

为什么选 MediaCrawler？

• **一套工具搞定所有国内平台**——不需要给每个平台装一个插件

• **评论抓取是核心功能**——评论区才是真正的金矿，这正是 Tavily 搜不到的

• **专为服务器设计**——基于 Playwright，天然支持在 VPS 上无界面运行

• **自带 WebUI**——首次登录扫码可以通过网页界面完成，不需要远程桌面

• **月成本 $0**——开源免费，不需要任何 API Key

**搭建步骤**

：

第一步：安装 MediaCrawler

在 OpenClaw 中说：

Plain Text

```
帮我安装 MediaCrawler（GitHub: NanmiCoder/MediaCrawler），用 Python 环境装好，并安装 Playwright 浏览器
```

![](img/6eb9eacefea5636d3a7fd0308dfc8840.png)

**第二步：启动 WebUI**

在 OpenClaw 中说：

Plain Text

```
帮我启动 MediaCrawler 的 WebUI 界面
```

启动后，用你的手机或电脑浏览器打开http://你的VPS的IP:8080，你会看到 MediaCrawler 的操作界面。

![](img/27a78d5ba68912091c03bb44d34c5724.png)

**第三步：登录平台（只需一次）**

在 WebUI 界面上选择你要登录的平台（比如小红书），它会弹出一个二维码。用对应平台的 App 扫码登录就行。

![](img/3b1c457afb1eb1715f42a8a19363dcb9.png)

![](img/b12eef58f65c40335cba3c1798e23404.png)

![](img/ce00bac5f0211b2b84531b959cffb603.png)

登录成功后，Cookie 会自动缓存在服务器上。以后每次采集都会复用这个登录状态，不用反复登录。通常几周到几个月才需要重新扫一次码。

**第四步：测试采集**

在 OpenClaw 中试一次：

Plain Text

```
# 在 OpenClaw 中说：
帮我用 MediaCrawler 搜索小红书上&quot;公众号自动化&quot;相关的笔记，抓取前 10 条笔记和评论
```

![](img/7ca46e5595a0c1cb91ccb1dfd44a4954.png)

![](img/247a5d7378b4b8b08b32707c9af95749.png)

![](img/e635aabcf0f374294838a90b8d467638.png)

**和 Tavily 怎么配合**

：Tavily 管广度——搜全网，帮你发现哪些话题正在被讨论。MediaCrawler 管深度——钻进具体平台，把评论区原话全捞出来。

举个例子：Tavily 搜到最近很多人在吐槽公众号 AI 文章没有人味这个趋势，你用 MediaCrawler 去小红书和 B 站搜这个话题，把评论区的真实吐槽全抓下来——"全是 4 点""没有人味儿""内容屠宰场缺我这把刀吗"——这些评论就是你文章里最有说服力的素材。

只用 Tavily 不用 MediaCrawler 也行——Tavily 搜到的内容足够找选题。但如果你想让文章里的论据来自真实用户原话（而不是 AI 编造的"据某用户反映"），MediaCrawler 就是你的弹药库。

**注意事项**

：

![](img/38ab46abb9f05c7f12fbeea0421f1c9e.png)

**海外平台怎么办？**

MediaCrawler 覆盖的是国内平台。如果你还想采集 X（Twitter）、Reddit、YouTube 等海外平台的内容，Tavily 的搜索结果通常就够用了。大部分公众号作者的读者和素材来源都在国内，先把国内平台的采集搞定再说。

入门版（Tavily）+ 进阶版（MediaCrawler）加起来：1 个 API Key + 1 个开源工具，月成本 $0，能搜全网 + 能深度抓取 7 个国内主流平台的评论区，覆盖 95% 的选题场景。

2.3 从信号到选题到文章

不管你用入门版还是专业版，采集到的素材都不能直接变成文章。中间有一个转化过程：

Plain Text

```
搜索结果（信号）→ 你的观点（选题）→ 文章骨架（大纲）→ 完整文章
```

举个例子：

1.  **信号**：MediaCrawler 在小红书上搜到一条笔记，评论区有人说："用了三个自动化工具，生成的文章全是 AI 味，改了一下午还不如自己写"，这条评论 328 个赞

1.  **选题**：公众号自动化工具都在解决错误的问题——它们帮你更快地发文章，但没人帮你发出来像你自己写的

1.  **大纲**：用你在 Step 1 中定好的风格指南，把选题展开成文章骨架

1.  **文章**：在 Step 3 中用风格化写作流水线生成

注意第 1 步到第 2 步——信号是别人的经历，选题是你的观点。你不是在转述别人的评论，你是从中提炼出你自己认同的论点，然后用你自己的方式论证它。

搞完之后检验一下，分别验证两个工具：

**验证 Tavily**

：Plain Text

```
# 在 OpenClaw 中说：
帮我搜索一下最近关于&quot;AI写作 个人IP&quot;的讨论，找出用户最大的痛点是什么
```

![](img/e71c4eb272845b069b5247000501d4d8.png)

**验证 MediaCrawler**

：Plain Text

```
# 在 OpenClaw 中说：
帮我用 MediaCrawler 搜索 B 站上&quot;AI写作&quot;相关的视频，抓取前 5 条视频标题和播放量
```

![](img/df2b87c6e3871bd1f0e3ee0e62dc474e.png)

你应该看到：

• Tavily 搜索结果正常返回（有标题、摘要、来源链接）

• MediaCrawler 能搜索平台并返回内容和评论

• 你能从结果里提炼出至少一个选题

能做到这三点，素材采集就搭好了。以后每次写文章前，Tavily 找方向，MediaCrawler 捞评论。

![](img/aee486072f5fb1f191d40602c535c8de.png)

Step 3：风格化写作流水线

**核心理念**

去 AI 味的本质不是写完再修，而是从第一个字就像你。

小红书上最火的去 AI 味教程，本质都是事后补救——写完一篇 AI 文章，然后改措辞、加口语、打乱结构。这就像做了一盘难吃的菜，然后疯狂加调料。调料加再多，底味还是不对。正确的做法是：从选食材开始就按你的口味来。

3.1 将三层配置注入写作流程

你手里现在有三个文件了：

• 风格指南.md（第一层）

• 范文样本.md（第二层）

• 负面约束.md（第三层）

下一步：把它们装进写作流程，让 AI 每次写作时自动读到。

在 OpenClaw 中，你可以把这三个文件做成一个 Skill，或者直接放在项目目录下作为写作时的参考文件。两种都行，但我推荐前者——因为做成 Skill 之后，你不用每次手动粘贴，AI 自己就会去读。

**推荐方式：做成 Skill**

在 OpenClaw 中说：

Plain Text

```
帮我创建一个写作风格 Skill，目录是 ~/.claude/skills/my-writing-style，
把 ~/Documents/我的风格语料库/ 下的风格指南.md、范文样本.md、负面约束.md 合并成一个 SKILL.md 放进去
```

验证：

Plain Text

```
# 在 OpenClaw 中说：
帮我确认 ~/.claude/skills/my-writing-style/SKILL.md 文件是否存在
```

3.2 文章生成流程

一篇文章从选题到成稿，完整走一遍大概是这样的：

**第一步：给定选题和素材**

Plain Text

```
# 在 OpenClaw 中说：
写一篇关于&quot;为什么大部分公众号自动化工具都在解决错误的问题&quot;的文章。

参考素材：
- [粘贴从 Tavily/MediaCrawler 采集到的相关信号和用户原话]
```

![](img/12b4f6d7db937a46f0c74375de38d2a7.png)

**第二步：像挑刺的甲方一样审大纲**

AI 会根据你的风格指南先生成一个大纲。别急着说"行，往下写"——这是你最该较真的环节。大纲一旦定歪了，后面写得再好也是精装修的毛坯房。

审大纲的时候重点看三件事：

**结构对不对味**

——你平时写文章是先讲故事再抛观点，还是反过来？大纲得跟你的习惯一致。如果你是那种喜欢上来就怼的人，大纲却安排了三段铺垫才进正题，直接打回去。

**开头是不是烂大街**

——如果第一行是"在 AI 时代..."或者"随着 XX 的快速发展..."，直接打回去。不用客气。你自己写文章的时候会这样开头吗？不会的话，AI 也不许这样写。

**论据是真的还是编的**

——每个论据都应该追溯到真实素材。你在 Step 2 用 Tavily 和 MediaCrawler 采集到的用户原话、评论区内容、数据，这些是你的弹药。AI 自己编造的"据某调查显示""有研究表明"，一律删掉。宁可论据少一个，也不要假论据。

**第三步：逐段生成**

不要让 AI 一口气写完全文——那样风格最容易跑偏。让它按大纲逐段写，每段写完检查一次风格是否一致。

**第四步：风格一致性校验**

文章写完后，做一次整体校验：

Plain Text

```
请对比这篇文章和我的风格指南，检查以下维度：
1. 是否有负面约束清单中的禁止句式出现？
2. 句式节奏是否符合风格指南描述？
3. 口语化程度是否匹配？
4. 观点表达方式是否一致？

如果发现不一致，请标注具体位置并修改。
```

![](img/42132430358bb048a0b6610e9e4eb4f3.png)

3.3 跨文章人格一致性

风格一致性不只是单篇文章内部的事。连续发 10 篇文章，读者应该觉得都是同一个人写的。这比单篇写得好更难，也更重要——因为人格一致性才是个人 IP 的根基。

**三个关键策略**

：

**策略一：固定开头范式**

每篇文章的开头用同一种模式。不是说每次写一样的话，而是用同一种进场方式。就像你每次进一个房间，有人习惯先敲门，有人习惯踹门进去。你的文章开头就是你的进场方式。

几种常见的固定范式，对号入座：

• **罗永浩式**：先讲一个反常识的事实或者直接怼一个流行观点。"我最近试了 XX，结果相当令人沮丧。"——上来就有冲突感。

• **半佛仙人式**：用一个荒诞的比喻或者黑色幽默切入。"如果 XX 是一道菜，那它大概是把所有调料倒进一个碗里然后告诉你这叫'融合菜'。"——上来就笑了，然后开始想。

• **和菜头式**：从一个私人的、微小的日常切入，然后突然拉到一个大话题。"今天下午在楼下咖啡馆坐着，听到旁边两个人聊 XX..."——上来就有画面感和亲近感。

**策略二：固定收尾范式**

每篇文章的结尾也要有一致的退场方式：

• **罗永浩式**：回到理想主义，或者一句简短有力的断言。

• **半佛仙人式**：把开头的荒诞比喻收回来，但翻转一下意思。

• **和菜头式**：回到那个私人的、安静的场景，但你看完文章之后感受不一样了。

**策略三：固定口头禅**

有意识地在每篇文章中复用几个标志性表达。罗永浩的"认真""理想主义""彪悍"，半佛仙人的"朋友们""硬核""离谱"，和菜头的"世事如此""且如此这般"——读者看到这些词就知道是谁在写。

**反面案例**

：如果你的第一篇文章用"我"开头、口语化、讲个人经历；第二篇文章变成"近年来..."开头、书面语、纯说理——读者会觉得不是同一个人写的。这种割裂感会快速消耗信任。

3.4 给表达提提味：五个招数

文章写完之后，还有一个可选但强烈推荐的环节：用表达五招再过一遍，把平淡的段落变得更有穿透力。

你可以自己对照检查，也可以让 AI 帮你过一遍：

Plain Text

```
# 在 OpenClaw 中说：
帮我用&quot;五个招数&quot;优化这篇文章的表达：把大变小、把远变近、把抽象变具体、把复杂变简单、把平淡变精彩。
```

五个招数分别是：

• **把大变小**：宏观观点缩到具体问题。"AI 正在改变世界"不如"AI 让你每天省出 2 小时"

• **把远变近**：从抽象技术拉到读者自己的场景。"分布式架构"不如"你的服务器扛不住了怎么办"

• **把抽象变具体**：用数字、案例、场景替代概念。"性能提升很多"不如"从 8 秒变成 0.5 秒"

• **把复杂变简单**：删掉修饰词和行话。能用大白话说的，不用术语

• **把平淡变精彩**：加对比、反差、意外视角。"这个方法不错"不如"这个方法让我删掉了之前写的 300 行代码"

验证：让朋友当裁判

用你的风格配置写一篇完整的测试文章（1500-2000 字），然后做几件事：

1.  把文章发给一个朋友，什么都不说，就问他一句："你觉得这像不像 AI 写的？"他的第一反应比任何检测工具都准。

1.  把这篇文章和你以前手写的文章放在一起看——风格统不统一？如果你自己都觉得这不像我，那就回 Step 1 调风格指南，别凑合。

1.  全文搜一遍负面约束清单里的禁止词。"综上所述""让我们深入探讨""在当今时代"——一个都不该出现。

1.  有条件的话，跑一次朱雀 AI 检测，目标 < 30%。

**微练习**

：现在就试一次。随便挑一个你最近感兴趣的选题，用你的风格配置让 AI 写一个开头段落（200-300 字）。写完之后，自己动手改一遍——哪些地方不像你，就改成你会说的话。改完对比一下原稿和你的修改稿，差异越大说明风格指南越需要补充。这个练习 10 分钟就能做完，但它会让你对自己的风格有更清晰的体感。

![](img/097a1d9840086b4695126095d028b300.png)

Step 4：配图自动化

关于 baoyu 系列 Skills

Step 4 和 Step 5 用到的 baoyu-cover-image、baoyu-article-illustrator、baoyu-image-gen、baoyu-markdown-to-html、baoyu-post-to-wechat 等 Skills，需要提前安装。在 OpenClaw 中说"帮我安装 baoyu 系列 Skills"即可。如果你的 OpenClaw 是完整版部署，这些 Skills 通常已经预装好了。

你自己刷公众号的时候，有没有碰到过那种全是字的长文？大概滑了三四屏之后，你的拇指就开始加速了——不是因为内容不好，而是眼睛累了。一张图就能把拇指刹住。

配图在公众号里有两个完全不同的角色，很多人只知道第一个，忽略了第二个：

**第一个角色：正文里的喘息点。**

一篇 3000 字的文章，每 800-1000 字需要一张图。不是为了好看，是为了让读者的眼睛休息一下。没有这个节奏，读者在第三屏左右就会划走。

第二个角色：封面图是你在信息流里的视觉签名。

这个更重要但更容易被忽略。读者刷朋友圈的速度是每秒 2-3 条，你有 0.3 秒让他认出这是你的文章。不是靠标题——标题太多了，来不及读。靠的是封面图的色调、构图、质感形成的视觉印记。所以封面风格一旦定下来，就别换。

4.1 封面图：先选套餐，跑通再说

封面图生成用baoyu-cover-imageSkill。它有 5 个维度可以调，但你第一次用的时候不需要全部搞懂。先从下面三个套餐里选一个，直接开跑：

选好了？直接用：

Plain Text

```
# 在 OpenClaw 中说：
给这篇文章生成封面图，用 cool 配色 + digital 渲染 + minimal 构图
```

一句话搞定。Skill 会自动读取你的文章内容，提取核心主题，生成匹配的封面图。

![](img/bc997df76fa68c4118338c18ede60dff.png)

选哪个套餐？看你的内容类型。科技/效率/AI 类选科技极简，文化/生活类选文艺手绘，商业/职场类选商务专业。拿不准就选科技极简——干净利落，不容易出错。

**想自定义？**

完整的 5 维参数表放在文末附录了，跑通了套餐之后再去看也不迟。

**输出**

：•封面图保存在cover-image/{topic-slug}/cover.png

• 同时生成 prompt 文件，方便你回看这张图是怎么生成的，下次微调

打开生成的cover.png，过四道关：

1.  图片尺寸对不对？公众号封面推荐 2.35：1（即 900x383 或同比例）

1.  风格和你指定的套餐一致吗？

1.  图上文字（如果有）清晰可读吗？

1.  把图片缩小到手机信息流的大小，主体还能认出来吗？这一步很关键——你的读者看到的是缩略图，不是大图。

4.2 内文配图

封面搞定了，接下来是正文里的配图。手动选图太累，让 AI 帮你决定在哪插图和插什么图。

**使用 baoyu-article-il**lustrator Skill，两个维度

：

**工作流程（全自动，你只管等）**

：

1.  Skill 分析文章结构，识别核心观点和段落分界

1.  按段落长度自动选择配图位置（约每 800-1000 字一张）

1.  为每个位置生成对应的图片 prompt（提示词）

1.  调用 baoyu-image-gen 生成图片

1.  自动插入文章中对应位置

**实际操作**

：Plain Text

```
# 在 OpenClaw 中说：
给这篇文章配内文插图，用 notion 风格
```

搞完之后检查一下：

1.  配图数量合理吗？3000 字大约 3-4 张

1.  两张图之间有没有挨太近？至少隔 600 字

1.  图片内容和上下文相关吗？不是随机装饰吧？

1.  所有图片风格是统一的吗？

![](img/3843774cae56b38bed5ce44a410d40be.png)

4.3 图像生成后端

**上面两个 Skill 底层都调**用baoyu-image-gen来生成图片。你可以把它理解成一个统一收银台——不管你从哪个供应商那里拿图，都走它这一个入口。

目前支持的供应商：

**配置默认供应商**

：在 OpenClaw 中说"帮我把默认的图像生成供应商设为火山引擎的 Seedream"，设好之后每次生成图片就不用再指定了。

验证：

Plain Text

```
# 快速测试图像生成是否正常，在 OpenClaw 中说：
用 baoyu-image-gen 生成一张测试图：一只猫坐在电脑前写代码
```

如果 30 秒内返回一张图片，说明后端配置正确。

![](img/54b6c3b8b009f2846901817d3f842647.png)

Step 5：排版 + 发布

公众号排版的本质不是好看，而是别让排版成为读者离开的理由。

这话不是我故作深沉。大多数人排版踩坑，不是因为不懂设计——是因为微信的渲染引擎有一堆反直觉的限制。你在电脑上精心调好的排版，发到手机上一看，列表缩进全乱了、代码块挤成一坨、字号小得要命。不是你的问题，是微信的问题。但读者不会去怪微信，他们只会划走。

好消息是，这些坑 Skill 全帮你踩过了。你只管写 Markdown，它来处理微信的那些反人类规则。

5.1 Markdown 转公众号 HTML

公众号编辑器不认 Markdown。你需要把 Markdown 转成带内联 CSS（就是把样式直接写在每个标签上，而不是单独放一个样式文件）的 HTML，才能在公众号里正常显示。

这一步用baoyu-markdown-to-htmlSkill，一句话搞定。

**4 种预设主题**

：

**实际操作**

：Plain Text

```
# 在 OpenClaw 中说：
把这篇 Markdown 文章转成公众号 HTML，用 modern 主题
```

**输出**

：•同目录生成一个.html文件

• OpenClaw 会返回图片占位符列表（后续发布时会自动替换为图床 URL）

![](img/942d21ea1a80c28071f69c702341f440.png)

![](img/dbfd0c2640bf20158b5d0a91b12ec685.png)

![](img/2f3d9844bae628c5121bb623a5ebc0c4.png)

关键细节（微信的那些反人类坑，Skill 都帮你处理了）

：

![](img/c656cfd852641cbbd8072beac871ae34.png)

这些坑 Skill 都帮你处理了，但如果你后续手动调整 HTML，记得别踩回去。

拿到 HTML 了，快速过一遍：

1.  打开生成的 。html 文件，在浏览器中预览

1.  字号看着舒服吗？

1.  列表显示正常吗？

1.  代码块换行正常吗？

1.  图片位置有占位符（发布时会替换）

5.2 发布到草稿箱

HTML 准备好了，最后一步——送进公众号草稿箱。

用baoyu-post-to-wechatSkill，推荐用 API 方式（比浏览器自动化方式快 10 倍，也更稳定）。

Plain Text

```
# 在 OpenClaw 中说：
把这篇文章发布到公众号草稿箱
```

密钥获取：

登录：

https://developers.weixin.qq.com/

在开发密钥点击重置，弹出的弹窗里复制 AppID,AppSecret

![](img/0821349083575306c9cd4a9abb5b9160.png)

![](img/24370d1c2872bbad30db1b7d2dd0a41e.png)

如果密钥配置后，重新发布会提示IP不在微信公众号的 IP 白名单中的错误，配置白名单

登录：https://mp.weixin.qq.com/

设置与开发——安全中心——IP白名单——去设置

然后把提示的IP添加添加白名单就可以了

![](img/cb08c004110e577fec3befe6a5ef03d7.png)

![](img/3981a493b5335d130cd977d54794968d.png)

背后发生的事情你不需要操心：Skill 先把图片传上去，再把文章传上去，最后在草稿箱里组装好。整个过程 10-30 秒。

**重要限制（必须知道）**

：

![](img/92d2b3b6f1ce621fd5852d8c0f151d8e.png)

换句话说，AI 帮你做到了 95%，最后的"发布"按钮需要你自己去按。这其实也是好事——发布前多看一眼，避免翻车。

5.3 发布前检查——别急，最后看一眼

文章进了草稿箱之后，先别急着点"发布"。花两分钟过一遍，这两分钟能帮你避开不少尴尬：

• 拉到文章底部，确认结尾在不在。长文容易被截断，草稿箱里看着前面好好的，结果最后三段没了。

• 图片都正常显示吗？偶尔图床上传会失败，出现裂图。碰到了重新发一次就行，别带着裂图发出去。

• **重点来了：点"预览"，发到自己手机上看一遍。**电脑上看着没问题的排版，手机上可能字太小、图太大、行距太挤。

• 封面图没被裁切吧？（2.35：1 比例是安全的）

• 标题没被截断吧？（公众号标题限 64 字符，超了会被砍掉）

• 检查一下标点：英文冒号要换成中文冒号，弯引号要换成直引号。这些小东西不影响阅读，但影响专业感。

经验之谈：手机端预览是最重要的一步。**一定要发到手机上看一遍再发布。**我自己踩过好几次坑——电脑上看得心满意足，发出去打开手机一看，代码块挤成一行，引用块的左边框消失了。改倒是能改，但已经推送出去的文章改不了。

验证

完整跑一遍发布流程，确认链路畅通：

1.  准备一篇测试 Markdown 文章（随便写几百字就行）

1.  转成 HTML：把这篇 Markdown 文章转成公众号 HTML，用 modern 主题

1.  发布到草稿箱：把这篇文章发布到公众号草稿箱

1.  打开mp.weixin.qq.com，进入"内容管理"，找到"草稿箱"，确认文章出现

Plain Text

```
mp.weixin.qq.com
```

最后确认四件事：

1.  文章出现在草稿箱了

1.  排版正常，没有乱码

1.  配图完整显示

1.  封面图正确

如果四项全部通过——你的 AI 写作 -> 配图 -> 排版 -> 发布全链路已经跑通了。从现在开始，每篇文章从选题到进草稿箱，10-15 分钟。

![](img/3450ca37710f644fbfcbd1636aab08a5.png)

Step 6：日常运营 SOP

3 小时搭的系统，死活就在每天那 5 分钟上。

你见过太多这样的人：花一个周末搭了一套自动化，兴奋了三天，然后再也没打开过。系统不是坏了，是没人喂它。接下来这几个 SOP，就是把你得记得去跑变成它自己跑完等你看。

6.1 Heartbeat 定时任务

先把最机械的那一步自动化掉——每天自动采集素材。你早上醒来打开电脑，一份今日选题推荐已经静静地躺在那里了。

在 OpenClaw 中说：

Plain Text

```
帮我设置一个每天早上 6 点自动执行的定时任务：
用 Tavily 搜索&quot;公众号自动化&quot;&quot;AI写作&quot;&quot;个人IP&quot;这几个关键词的最新讨论，
整理成今日选题推荐，保存到 ~/Documents/每日选题/ 目录下
```

配好之后，建议连续跑三天确认一次——有些网络问题只有在凌晨 6 点、网络配置环境自动断开的时候才会暴露出来。

6.2 IM 指令：随时触发

定时任务解决了每天采集，但有时候你临时冒出一个选题，想立刻写。这时候不用打开终端、不用记命令——直接给 OpenClaw 发一句话就行。

通过飞书/Telegram 给 OpenClaw 发：

Plain Text

```
写一篇关于XXX的文章，发到公众号草稿箱
```

OpenClaw 会自动跑完全流程：

1.  用 Tavily + MediaCrawler 采集相关素材

1.  用你的风格指南写文章

1.  生成封面图和内文配图

1.  转成公众号 HTML

1.  发布到草稿箱

你只需要做一件事：去草稿箱检查一遍，然后点"发布"。

从冒出想法到草稿箱里躺着一篇文章，中间大概 12 分钟。你甚至可以在地铁上触发，下车的时候文章就好了。

6.3 风格漂移检测

这是最容易被忽略、但最致命的一步。

什么叫风格漂移？举个具体的例子：第一周你写"这玩意儿不靠谱"，第三周 AI 悄悄变成了"该工具的可靠性有待商榷"——这就是漂移。AI 会在不知不觉中回归它的默认腔调，温水煮青蛙式地把你的风格磨平。

每周花 5 分钟做一次风格体检，把本周的文章和风格指南对比。重点盯这三个症状：

• **口语化程度逐渐降低**：第一篇还在说"扯淡"，第三篇就变成"不切实际"了

• **开头/结尾范式开始变化**：你本来是"直接甩观点"的风格，AI 悄悄改成"在这个 XXX 的时代..."

• **禁止词开始偷偷出现**：负面约束清单里写了"赋能"不能用，结果它在第四篇里给你塞了一个"数字化赋能"

**解决方法**

：发现漂移就立刻更新风格指南和负面约束清单，把新发现的问题补进去。风格配置是活的，要跟着你的实际产出不断迭代。

验证：

Plain Text

```
# 在 OpenClaw 中说：
对比这三篇文章和我的风格指南，检测风格一致性：
1. [粘贴本周第一篇]
2. [粘贴本周第二篇]
3. [粘贴本周第三篇]

重点检查：开头范式、收尾范式、口头禅使用、禁止词出现次数。
```

6.4 成本控制

跑这套系统每个月要花多少钱？说实话，比你想象的少。关键是把钱花在刀刃上——采集环节不需要聪明的模型，写作环节不能省。

![](img/37cc623594957a354a0893b2734adf93.png)

**月成本估算**

（每周 3 篇文章）：

• 采集：约 $2-5/月

• 写作：约 $10-20/月

• 配图：约 $5-10/月

• **总计：约 $17-35/月**

换个角度算：一篇文章的全链路成本不到 3 块钱。你在星巴克买杯咖啡的钱，够发一周的公众号了。

特殊处理

**朱雀 AI 检测**

微信公众号用朱雀系统检测 AI 内容。AI 率超过 30% 会限流。

好消息是，本教程的三层风格架构已经从根源上降低了 AI 味——不是写完再去 AI 味，是从第一个字就不像 AI。但如果你仍然不放心，有几个额外措施：

1.  **在关键段落加入个人真实经历**——AI 无法编造你的经历，这是最强的人味儿信号

1.  **引用真实用户原话**——来自 MediaCrawler 采集的评论素材，带着错别字和情绪的那种，反而更真实

1.  **保持合理的不完美**——偶尔的口语化、非标准表达反而更像人写的。完美无瑕的文章才可疑

1.  核心观点自己写，AI 负责展开和润色——把你最有态度的那几句话自己敲出来，其他的交给 AI

如果你有朱雀检测渠道，把文章贴进去跑一次，目标是 AI 率低于 30%。如果超标，重点检查哪些段落被标记为 AI 生成，针对性地加入个人经历或真实用户原话。

**登录态维护**

baoyu-post-to-wechat 的 API 方式需要 AppID 和 AppSecret，这些不会过期，配一次管终身。

但如果你用浏览器方式发布，登录态可能过期。解决：在 OpenClaw 中说"帮我检查公众号的登录状态是否正常"，如果过期了，它会引导你重新登录。

常见问题

Q：我没有历史文章，怎么建风格档案？

A：这是最常见的冷启动问题。别慌，你不需要已经是大 V 才能开始。随便找 5 个你关心的话题，坐下来手写 500 字以上的短文。不要先想好结构再写，想到什么写什么——这才是你的声音。

5 个具体题目建议，帮你破冰：

• **你最近踩的一个坑**——工作上的、生活上的、技术上的都行，写你是怎么掉进去、怎么爬出来的

• **你对某个热门观点的不同意见**——大家都说 A 好，你觉得不对，为什么？把你心里那个不对劲的感觉写出来

• **你用过最好和最烂的产品**——各写一个，为什么好、为什么烂，用你自己的标准评判

• **给半年前自己的一条建议**——如果能穿越回去，你会对自己说什么？为什么？

• **最近学到的让你兴奋的东西**——一个概念、一个工具、一本书、一句话，为什么让你兴奋？

写完这 5 篇，你的风格 DNA 就够用了。记住：关键不是文笔好不好，是像不像你自己在说话。

Q：AI 写的文章朱雀检测 100% 怎么办？

A：检查你的风格指南是否足够具体。如果只写了"用轻松的口吻"，那和没写一样。风格指南需要具体到句式、用词、段落节奏。另外，在关键段落加入个人经历和引用真实用户原话。

Q：每次写作都要把三个文件喂给 AI 很麻烦？

[A：做成 Ski](http://SKILL.md)ll。把风格指南、范文片段和负面约束合并到一个SKILL.md文件中，之后 OpenClaw 自动加载，你不用每次手动喂。

Q：我的风格和咪蒙完全不同，这个教程还适用吗？

A：完全适用。咪蒙只是演示案例。三层架构是通用的——不管你是温柔型、犀利型还是学术型，都是同样的步骤：收集语料 -> 分析 DNA -> 生成配置 -> 注入写作。

Q：公众号 API 只能发草稿，不能直接发布怎么办？

A：这是微信的限制，目前无解。但草稿箱工作流也有好处——你可以在手机上最后检查一遍再发布，这是最后一道质量关卡。

**Q：一个月的成本大概多少？**

A：按每周 3 篇估算，约 $17-35/月（采集+写作+配图）。主要成本在文章写作环节，用 Sonnet 比 Opus 便宜很多且质量足够。

Q：多个公众号可以用同一套工具吗？

A：可以。但每个公众号应该有自己的风格档案。如果两个号风格不同，需要分别建立三层配置。工具链复用，风格配置独立。

附录：深入理解

前面正文为了保持节奏，很多细节被略过了。如果你想深入了解某个部分的完整信息，展开对应的折叠块。

封面图 5 维参数完整表

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

图像生成后端供应商详情表

![](img/a0ded9a683ce043c3c7b35b354746ed4.png)

**选择建议**

：•日常出图：Seedream（默认，够用了）

• 需要自然场景：Gemini

• 网络环境受限：通义万相

• 探索特殊风格：Replicate

Skill 完整清单表

![](img/68de76f32c3af9663e76c607aad87c36.png)

完整架构图

Plain Text

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

**每次使用前的检查清单**

**每天（自动化运行前）**

：•MediaCrawler 服务正常运行（在 OpenClaw 中说"帮我检查 MediaCrawler 状态"）

• 网络配置环境已开启（仅当需要搜索海外内容时）

• OpenClaw 实例正常运行

**每周（风格维护）**

：•检查本周文章是否有风格漂移（重点：口语化程度、禁止词）

• 更新负面约束清单（把这周新发现的 AI 味表达补进去）

• 检查朱雀 AI 率（如果有条件）

**每月（系统维护）**

：•更新风格指南（你的风格也在成长，好文章会让风格越来越清晰）

• 补充范文样本（把最近写得满意的文章加进去，淘汰早期不够好的）

• 检查 API 额度和成本

• 更新 Skill 到最新版本

### 03.进阶：OpenClaw 实现业务自动化

**注意：进阶篇的案例难度都较大，新手圈友，只需要完成实战篇的一个案例即可，进阶**篇不需要完全掌握，可以作为拓展内容学习，如果在实操中遇到问题，直接截图问 AI。

1.用 OpenClaw 搭建企业知识库+数字员工（企业内部）

本节的重点在于，给企业搭建知识库，从而打造企业 AI 数字员工

1.1 企业知识库的搭建

小龙虾的能力越来越强，它有了很多内置功能可以操作浏览器，修改 Excel，可以识别语音等越来越像一个人，有了基本的感知能力，而且我们可以给他安装一些特定的 Skill， 这样你的小龙虾就掌握了各种专业技能，可以在日常工作中充当你的个人助理，甚至可以帮助你解决一些日常工作问题，充当你的数字人员工，虽然现在 OpenClaw 还有很多不完善的地方，但现在你可以把它当成一个实习生，可以在你的监督和教导下不断成长，越来越接近人类员工的水平。

这个案例我们就来给大家介绍怎么通过搭建自己的私有化知识库让龙虾掌握你的私有知识，比如我们可以把你的商品资料、公司文档知识库给到小龙虾调用，它就变成了最懂你的数字助理，然后通过开发 Skill 让小龙虾自动调用知识库和总结经验等，让知识和经验更好的沉淀，最后根据不同的应用场景接入飞书、企业微信等平台来解决不同的业务场景问题。

这里我们给出了 2 种知识库的搭建方案：

一是通过云端服务搭建，火山引擎提供的知识库可以支持 API 调用和服务调用，这个方案比较简单，适合新手入门。

另一个方案是通过 Aanything LL 在本地部署自己的私有知识库，这个方案的优势就是成本更低，而且数据存在你的本地，安全性比较有保障。

**首先我们来演示第一种方案：**

（一）火山引擎部署知识库

1.  登录火山方舟控制台， 进入知识库页面

![](img/035155317bb23e4b9050681ea4e91d2d.png)

1.  创建知识库，知识库分为标准版和旗舰版，标准版是包天 1 块/天， 旗舰版适合企业包月，这里我们选标准版就可以了，而且支持 30 天免费试用

![](img/88e65b3e6db1b9e5735d9c31c6af3bf5.png)

![](img/27161e628c37b2db138bac61933f899b.png)

选择标准版，输入名称和描述就可以了，也可以查看更多配置，进行更详细的配置，没有特殊需求，用默认配置就好了

![](img/028737242c623aa88a992f34fc2d7d7a.png)

![](img/6d68485c07b748349c2c3ee7d646c246.png)

创建好知识库之后，下一步导入文档

![](img/20e4c7589a8268130ec9f7f7908520d9.png)

这里选择从本地导入，支持 PDF， Word， Excel， TXT， CSV 等、

![](img/fa4a6c42851e76d1f2c2d26b5a54d173.png)

也可以直接从飞书文档导入，注意第一次导入的时候需要账号授权，这里比较方便的是可以直接导入飞书知识库和多维表格

![](img/576b2162fff4fe45e34cd288d855b004.png)

![](img/f6c116d2475d4201bec7c76d4028e4cf.png)

选择好文档之后，点击底部的导入

![](img/553ee1966116d61d4e9226be970344e0.png)

然后等一会，就开始处理了，会先进行文档切片，然后做向量化，并存到数据库，可以看到文档的处理状态

![](img/fbdfa6bdb35a52eb17d9a4baad3b7ae0.png)

然后可以切到切片详情，查看切片结果

![](img/5cd264d1f855af3386a9f2ff830ca1a7.png)

下一步我们通过知识检索功能测试一下知识库的检索功能

![](img/c602cfba4d6a96b917030e79e7a00548.png)

火山引擎知识库还集成了 AI 大模型问答功能，基于知识库检索结果可以直接生成答案，这个功能就可以直接通过 API 提供给微信客服来做直接问答

![](img/1c4c6837f3057a28858e8bbc7db6c099.png)

但我们的目的是提供知识库检索结果给小龙虾，所以下一步就是把知识库的 API 给到小龙虾调用

![](img/80e7cd570ac13d76e4589c585c4994cd.png)

当然小龙虾不能直接调 API，所以我们需要开发一个 Skill 来进行业务逻辑的处理，调用这个 API，让小龙虾来使用这个 Skill

![](img/c6cb1752ab249a1902ab239fd217d37d.png)

复制这段代码，给到 Claude Code， 让 CC 来帮我们开发一个 Skill

![](img/3f864fddb338061e01f853ae5589dd65.png)

![](img/dff3f8e6446578b3e0914005b15591a6.png)

Skill 写好之后，需要配置访问 AK 和 SK， CC 会让你提供

![](img/f200a65902396bf92b5391747253be4e.png)

下一步 我们在火山引擎 控制台找到 Access Key， 点击右上角头像，再找到 API 访问秘钥

![](img/4a1d038586687c3888548706c6e35d34.png)

![](img/3369f10c7fb377f36ba60bedbcfabb05.png)

配置完之后，让 CC 测试一下这个 Skill， 是否可以正常调用

![](img/dcce3aa3a53f1920b553b5206229a2c9.png)

中间如果遇到问题就继续让 CC 修改，知道 Skill 调通

![](img/9759e857f814fc9cfe8304e76472fc17.png)

然后我们就可以在小龙虾后台看到我们刚才创建的 Skill

![](img/a6f592c125c274ccea9902147b7e54aa.png)

下一步我们在小龙虾中测试 Skill 是否可以正确调用

![](img/49bb835f02fa7c43ef6b4c456bd098dc.png)

![](img/efbb68970ed6f8f9b45067f52956d4fa.png)

（二）Anything LLM 本地部署知识库

AnythingLLM 是一个全栈应用程序，您可以使用现成的商业大语言模型或流行的开源大语言模型，再结合向量数据库解决方案构建一个私有 ChatGPT，不再受制于人：您可以本地运行，也可以远程托管，并能够与您提供的任何文档智能聊天。

AnythingLLM 将您的文档划分为称为workspaces（工作区）的对象。工作区的功能类似于线程，同时增加了文档的容器化。工作区可以共享文档，但工作区之间的内容不会互相干扰或污染，因此您可以保持每个工作区的上下文清晰。

可以把 Anything LLM 当做你的私人图书馆，可以存储你的所有文档和资料，然后这个博物馆还配置了一个强大的 AI 文档引擎可以直接根据知识库的内容进行回答，可以介入 ChatGPT 等大模型 API，也可以本地部署开源模型。

我们需要用到的就是 Anything LLM 提供的知识库 API

首先我们需要安装客户端，是的 Anything LLM 提供了 客户端安装，这就很方便了

打开官网https://anythingllm.com/

![](img/3c5438810890d67293eca11c71a5bcb9.png)

下载适合你电脑环境的客户端，安装之后就是这个界面

![](img/f6d089e8e4b980e243b58f61a3e07e7d.png)

然后开始，这里就用它推荐的模型，下载 Qwen 模型部署到本地，或者你也可以用其他模型的 API

![](img/870b8d8a39b723a508e98dca6e1d8b52.png)

继续下一步，Provider 和 向量模型都用默认的 Aanything LLM 提供的

![](img/5a170e7efb716de29e25b2c1cbc5d9ee.png)

这一步可以跳过

![](img/b9ef729bd759d4859d387433667651d2.png)

然后就进入到了主界面

![](img/46cddc08251b1095ac06ab6ca654e852.png)

安装之后啥也没有，我们首先需要添加一个工作空间

![](img/ab6476daca7b4eec47af3f52cdb8f446.png)

随便起个名字，比如就用产品名

![](img/42a6af4f29f98a346592416588f7ceb9.png)

下一步点击上传文档按钮，导入我们的知识库文档

![](img/6013986522c8f2fd6f185883c86cb2db.png)

如果是飞书文档的话需要下载到本地再导入，虽然它有导入链接的功能，但好像解析不了飞书文档

![](img/f59c1ab1f1b8338c713c048c3287ad78.png)

Anything LLM 还支持 多个笔记仓库的数据同步，如果你的文档存在只写平台可以直接同步过来

![](img/fee978be9d0913ed0c57436244e159f9.png)

导入文档后，选择刚才导入的文档，然后点击下面的 Move to Workspace 按钮，移动到工作空间

![](img/0f039514e15cb7f8c2897cb859cfb604.png)

然后下一步，Save and Embed 进行向量化存储

![](img/d465f633498497cf82f03a5e53c2dc3d.png)

然后我们用系统自带的问答功能来测试一下知识库是否可以正常调用，因为前面我们安装了 Qwen 7b 的本地模型，可以在本地进行一些基础的问答

![](img/556da8df8de5397bfde2c419abcb8550.png)

下一步设置 API 调用，点击左下角的设置按钮

![](img/77c78796fdc05f169db8121f959517a8.png)

找到 Development API 菜单，然后生成一个 API Key

![](img/94fc92686aeb8a5337499751ea90c7b9.png)

可以在这里看到详细的 API 文档

![](img/294557ac665bbe47b7864c86299e3097.png)

如果要开发更多功能，可以参考这个文档

![](img/7871c32b259e5bd311d65c9969ea0a39.png)

Anything LLM 默认的 API 地址是http://localhost:30001/api/v1, 我们把这个 Base Rul 和生成的 API Key 给到 CC 测试一下

Plain Text

```
http://localhost:30001/api/v1
```

![](img/f395528c3960ce32fb8393aa36aa49ab.png)

测试成功就说明我们的本地知识库 API 可以用了

![](img/bad8d0a63f078b9dbbfbb4b34e607d27.png)

同样，我们让 CC 写个 Skill 让小龙虾调用

![](img/d1ae1cda461bd314612981e23d812898.png)

重启 OpenClaw 之后就可以在后台看到创建的 Skill 了

![](img/e4dacbb2b2432cc043e242edc870bd42.png)

![](img/e5163fc559e6e5bde8c5e8f4da7765c6.png)

然后小龙虾里测试一下是否可以正常访问知识库

![](img/e51dd4b30132b51b03daff61d75414c7.png)

小龙虾接入了知识库的能力之后，就可以有很多应用场景

**个人 AI 助理：**

把你的个人笔记，聊天记录等导入到知识库，小龙虾就可以作为你的个人 AI 助理，比如在执行某些任务的时候可以调用知识库的资料加入你自己个性化的内容

**企业 AI 数字员工**

可以把小龙虾接入企业微信，实现企业内部的 AI 员工助理，比如行政问答助手、财务流程助手、IT 答疑助手、客服帮手等岗位和应用场景

![](img/4f3cfb588fadc7d00465513701907817.png)

1.2 打造**企业 AI 数字员工**

首先，我们需要创建一个智能机器人

在工作台菜单，找到智能机器人，如果找不到可以在右上角搜索

![](img/67f9d8aae8a1f936b125a58326b642c7.png)

下一步，创建机器人

![](img/211982513e01b6fb0325bd1f059565f4.png)

选手动创建

![](img/59880baf88c190a69be5d61747566f20.png)

下一步，选择 API 模式创建

![](img/ea11523a6b5b8c4eec43272053a98cd3.png)

选择以 长连接 方式创建，并获取 Bot ID 和 Secret。

![](img/2c45a1f0f0366f660cdc0b9f470ddf5e.png)

注意这里要设置可见范围，即你要在企业内部使用范围，比如员工群里应用

然后回到小龙虾终端，安装企业微信插件

Ada

```
openclaw plugins install @wecom/wecom-openclaw-plugin
```

![](img/79c32d958090b8a25e56d0e77910d6c8.png)

在终端中，输入以下命令，重启 OpenClaw。

Ada

```
openclaw gateway restart
```

在终端中，输入以下命令，添加渠道。

Ada

```
openclaw channels add
```

![](img/c39822b284c10947a9e0a6c5d7755dda.png)

在 select channel 步骤，选择 channel 为企业微信。随后输入企业微信机器人 Bot ID、Secret，并选择 finish。

![](img/d38a9d6fa2ca859e83a534505afc51ed.png)

选择配对方式，选择 Pairing。完成后继续配置，并可看到配置渠道成功提示。

![](img/361bbf9de537e3a278c051c48dbbccae.png)

![](img/55ec87bb48c0f1257f8077a850e1a53b.png)

在企业微信中，保存机器人，并跟它发消息，会收到一个配置密钥。

![](img/636b1407f9d1088c0b1a703ded4e1f1d.png)

复制此消息最后一行，并输入在终端中。完成配对后，即可在企业微信中与机器人正常对话。

![](img/d24f9a214d67bbc98019cd9f10aa5d85.png)

![](img/3176d94e44b37d940f0f61c113278fa8.png)

然后我们就可以企业群里@添加的小龙虾员工来执行任务了

![](img/eeebab733531fa6e9b625d36fcd0cdc3.png)

可以把小龙虾接入微信客服，直接回答用户问题，之前的航海我有分享过如何通过扣子搭建客服工作流并接入微信客服，现在同样可以把小龙虾接入微信客服，由于官方没有提供插件，有一个开源的插件是可以实现这个功能，不过由于配置过程比较复杂，属于进阶内容，这里我们就介绍一下，感兴趣的同学可以研究研究：

[https://github.com/rcfcu20](https://github.com/rcfcu2000/openclaw-wecom-kf)00/openclaw-wecom-kf

openclaw-wecom-kf

微信客服（WeCom Customer Service）渠道插件，让外部微信用户通过企业微信客服系统与 OpenClaw AI 智能体交互。

与 wecom-app 的区别

接入其他客服系统，比如淘宝、抖音等电商客服系统，由于大部分客服系统没开发 API， 我们直接用小龙虾接入还有一定难度，小龙虾还没有 RPA 的能力，虽然可以操作浏览器，有一些客服系统也支持 Web 端，那可能需要一点开发能力让小龙虾获取和发送客服消息的能力

![](img/833489d4b04c9b82643a8fb6075cd7bc.png)

2.用 OpenClaw 打造你的专属 AI 客服（企业对外）

这一节我们来学习如何让企业微信客服接入 AI，客户扫码就能跟你调好的 AI 知识库自动对话。

**先花 2 分钟搞懂原理**

别急着动手，先看看整个链路是怎么跑的。搞懂了后面就不会卡：

Plain Text

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

有三个词后面会反复出现，我们先混个脸熟就行：

| 概念 | 一句话解释 | 打个比方 |
| --- | --- | --- |
| 微信客服 | 企微里的一个功能模块，专门服务外部微信用户 | 就像淘宝店的&quot;在线客服&quot;入口 |
| 回调 | 企微收到消息后，主动推给你服务器上的一个网址 | 你留了个收件地址，快递员直接送上门 |
| OpenClaw | 开源的 AI Agent 平台，你的 AI 客服跑在上面 | 一个&quot;AI 调度中心&quot; |

先别急，先分清两个后台，不然后面很容易配错地方：

1.  企业微信管理后台：[https://work.weixin.qq.co](https://work.weixin.qq.com/wework_admin/loginpage_wx?redirect_uri=https%3A%2F%2Fwork.weixin.qq.com%2Fwework_admin%2Fframe)m/wework_admin/frame

主要用来创建自建应用，后面补可信 IP。

1.  微信客服后台：https://kf.weixin.qq.com/

这才是这篇教程的主战场。创建客服账号、找openKfId、配置回调 URL、生成Token和EncodingAESKey、拿corpSecret，都优先在这里完成。

你需要收集 5 个值

从微信客服后台为主，把下面这 5 个值收齐，再填到 OpenClaw 里：

| 序号 | 配置项 | 值 | 建议获取位置 |
| --- | --- | --- | --- |
| 1 | 企业 ID（corpId） | 待填 | 微信客服后台 → 企业信息 |
| 2 | 客服账号 ID（openKfId） | 待填 | 微信客服后台 → 客服详情；如果页面没显示，就用接口兜底查询 |
| 3 | 回调 Token | 待填 | 微信客服后台 → API 配置 |
| 4 | 回调 EncodingAESKey | 待填 | 微信客服后台 → API 配置 |
| 5 | 微信客服 Secret（corpSecret） | 待填 | 微信客服后台 → API 管理，回调验证通过后获取 |

注意两个坑：

1.  第 5 个 Secret 不是自建应用的 Secret，而是“微信客服”自己的 Secret。

1.  openKfId有时候页面里不明显，甚至一时找不到。别卡在这里，后面可以通过接口把它查出来。

第一步：注册企业微信 + 记录企业 ID

1.1 注册企业微信（有了就跳过）

放心，个人就能注册，不需要真的有公司。

1.  电脑打开 https://work.weixin.qq.com/

Plain Text

```
https://work.weixin.qq.com/
```

1.  点页面中间那个**「立即注册」**蓝色按钮

1.  类型选**「企业」**— 个人也选这个，不影响

1.  填信息：

◦

**企业名称**：随便写，比如"XXX 工作室"

◦

**行业类型**：随便选

◦

**员工规模**：选最小的

1.  用你的**个人微信**扫页面上的二维码

1.  扫完按提示确认，完事

![](img/43878f357c78e28cc982cce72d4eaebb.png)

1.2 记录企业 ID

1.  注册完你会自动进管理后台。没进去的话，手动打开：https://work.weixin.qq.com/wework_admin/frame

1.  看左侧菜单，**拉到最下面**，点**「我的企业」**

1.  进去之后**往下翻**，找到**「企业 ID」**这个字段

1.  长这样：ww1a2b3c4d5e6f7890，ww开头的一串

1.  **复制它**，先存到备忘录里

![](img/e63d4b63ed769499dccc18fd66db4ebc.png)

搞定，回去把企业 ID 填到表格第 1 行。

第二步：创建自建应用

1.  左侧菜单 →**「应用管理」**

1.  往下翻，找到**「自建」**那个区域

1.  点**「创建应用」**

![](img/426b422b670b65d48d9e8c858c36070f.png)

1.  填表：

◦

**应用名称**：写AI客服助手或你喜欢的名字

◦

**应用 Logo**：随便传个图标

◦

**可见范围**：选「全公司」最省事

![](img/3165e60af056d34520838d99985f84d8.png)

1.  点**「创建应用」**，搞定。

第三步：开通微信客服 + 创建客服账号

3.1 开通微信客服

1.  左侧菜单 → 找**「微信客服」**

◦没看到的话，点「应用管理」→ 在列表里翻，找到「微信客服」

1.  第一次进会让你开通，点**「开通」**就行

![](img/a785f1dd20102d3a4af94461f9637b18.png)

![](img/ee2ec29611d1478cc8f961af06b6cd4f.png)

3.2 创建客服账号

1.  点**「添加客服账号」**

1.  填一下：

◦

**客服名称**：客户会看到的名字，比如在线客服、智能客服

◦

**客服头像**：传一个（客户聊天时看到的就是这个头像）

1.  **添加接待人员**→ 选你自己

这里有个坑：你选的人必须在第二步那个应用的「可见范围」里。如果你之前选了「全公司」，这里就没问题。

1.  点**「确定」**

![](img/f064980b588be68b8ed767eeb5cdef25.png)

3.3 记录客服账号 ID

1.  点刚创建的客服账号，进详情页

1.  找到**open_kfid**— 长这样：wkABCDEF1234567890，wk开头

1.  **复制它**

找不到 open_kfid 也正常，别卡在这一页死找。

如果页面里没显示，你有两个办法：

1.  先记住客服名称，后面再回来看一次

1.  直接通过接口把客服账号列表拉出来拿 ID

我自己最后就是让小龙虾通过接口请求，把 ID 查出来的。

搞定，回去把客服账号 ID 填到表格第 2 行。

第四步：去微信客服后台生成回调参数

做完这步你拿到：Token（第 3 个值）+ EncodingAESKey（第 4 个值）

注意：这一步要去微信客服后台https://kf.weixin.qq.com/，不是去自建应用详情页。

1.  进入微信客服后台

1.  找到 API 配置相关页面

1.  生成Token

1.  生成EncodingAESKey

1.  先复制保存

1.  先不要急着点「完成」或「开始使用」

![](img/dab2bd65131ae202404af7782d06e36b.png)

为什么先别点？因为点完成的一瞬间，微信客服会去验证你填的回调 URL。你的 OpenClaw 还没配置好时，这一步大概率会失败。

这里顺手再提醒一次：回调 URL、Token、EncodingAESKey这几个值，优先在微信客服后台这一侧处理，不是在自建应用的「接收消息」里处理。

![](img/734424485cef011cc7ca6b221fc45e1c.png)

![](img/158350185231cfb48dc4630147106727.png)

![](img/b4392cecf38af3057a3cefd7475fdea2.png)

第五步：配置 IP 白名单

企微有个安全规则：只有白名单里的 IP 才能调 API。你的服务器不在名单里，接口直接拒绝你。所以得加一下。

1.  左侧菜单 →**「应用管理」**→ 点你的应用

1.  点进你自己创建的那个应用

1.  往下翻，找**「企业可信 IP」**

1.  点**「配置」**

1.  填你服务器的**公网 IP**（只填 IP，别加端口号）

1.  点**「确认」**

![](img/89a73a163668fba13fa391420d9b1f0f.png)

不知道服务器 IP？去你的云服务商控制台看，服务器详情里就有"公网 IP"。

![](img/fd4d7ff39f8a400cf530c06bd1829c92.png)

第六步：进一次终端，复制粘贴搞定

这是整个教程唯一要进终端的地方。

就是复制粘贴一段命令，不用你写任何代码。

6.1 登录你的服务器

终端是啥？就是个黑色窗口，你输命令，服务器执行。跟"给服务器发指令"一样。

怎么登录：

• **Mac**：打开「终端」，输ssh root@你的服务器IP，回车，输密码

• **Windows**：用 PuTTY 或 Windows Terminal 连上去

• **最省事**：很多云服务商（阿里云、腾讯云）有网页版终端，控制台找「远程连接」直接打开

![](img/84bfd09f3ff7dbbf21bdecab0c1d34de.png)

看到root@server:~#之类的提示符，就说明进去了。

6.2 复制粘贴这段命令

先别急！下面这段命令里有 4 个地方要换成你自己的值。先把前面收集的 4 个值准备好。

**整段复制，把 4 个"替换成你的 x**xx"改成你自己的值，粘贴到终端里回车：

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

举个例子，假设你拿到的值是：

| 配置项 | 你的值 |
| --- | --- |
| Token | aBcDeFgHiJkLmN |
| EncodingAESKey | abcdefghijklmnopqrstuvwxyz01234567890ABCDEF |
| 企业 ID | ww1a2b3c4d5e6f7890 |
| 客服账号 ID | wkABCDEF1234567890 |

那你就把"替换成你的Token"改成"aBcDeFgHiJkLmN"，其他几个照着改。

这里没有填corpSecret—— 正常的！这个值下一步才能拿到。不填也不影响回调验证。

6.3 怎么知道成功了

跑完之后你应该看到：

1.  插件安装成功 — 出现installed @openclaw-china/wecom-kf

1.  几个 config set 都没报错

1.  Gateway 重启成功

想确认 Gateway 真的在跑？执行：

Bash

```
openclaw gateway --verbose
```

看到[wecom-kf] webhook registered at /wecom-kf就齐活了。插件已经在等企微送消息过来。

装插件报错了？十有八九是网络问题。先换个国内镜像再试：

Bash

```
npm config set registry https://registry.npmmirror.com
```

第七步：回企微后台验证 + 拿 Secret

7.1 完成回调验证

这里要回的是微信客服后台https://kf.weixin.qq.com/，不是自建应用详情页。

1.  打开微信客服后台的 API 配置页面

1.  **URL 那个框填：**

http://你的服务器公网IP:18789/wecom-kf

比如 IP 是 123.45.67.89，就填：

http://123.45.67.89:18789/wecom-kf

1.  **确认**Token**和**EncodingAESKey**都填的是你前面保存的那两个值**

1.  **点「保存」或「完成」**

![](img/c2648b6f246c1a89e9764de3972d268d.png)

**关键提醒：**

• 回调 URL 要配在微信客服后台

• 如果你之前是在自建应用里配的，先别沿着那条路继续折腾了，按这里重新配

• 我一开始就是在应用里设置回调 URL，结果客户发消息一直没回应；后来改成在微信客服后台设置，才成功

看结果：

![](img/095a95b6e01df2546a25a0fc2df996f2.png)

**验证没过？一个一个排除：**

1.  Gateway 在跑吗？回终端看看有没有日志

1.  执行了openclaw config set gateway.bind lan吗？没执行的话外网访问不到

1.  18789 端口放通了吗？去云服务商安全组检查

1.  IP 填对了吗？去控制台确认

1.  Token和EncodingAESKey跟配置里的一样吗？别多空格少字符

![](img/78e65b56f91ab6894c8e7c20d35ca640.png)

7.2 补充可信 IP 和应用授权

如果你这时发现应用还不能正常调用微信客服接口，再补这两个：

1.  回企业微信管理后台

1.  打开你的自建应用

1.  配置「企业可信 IP」

1.  再回微信客服后台，把这个应用设成「可调用接口的应用」

这里容易绕，所以你记一句就行：

回调先通，再补可信 IP 和应用授权。

![](img/f9174c5899f43db07d1aaa6b89f16628.png)

7.3 拿微信客服 Secret

这个 Secret 我最后是在微信客服后台拿到的，不是在企微应用页里拿到的。

1.  回到微信客服后台

1.  找 API 管理相关页面

1.  找到微信客服的corpSecret

1.  按提示验证后复制

再说一遍：这个 Secret 是“微信客服”的，不是第二步那个自建应用的。长得很像，但不是一个东西，别搞混。

搞定！5 个值全齐了！

7.4 把 Secret 填进去

最后一次进终端，就两句命令。登录服务器，粘贴（把值替换掉）：

Bash

```
openclaw config set channels.wecom-kf.corpSecret &quot;替换成你的Secret&quot; &amp;&amp; \
openclaw gateway restart
```

Gateway 重启成功，关掉终端。后面全在浏览器和手机上搞定。

第八步：拿客服入口

方式一：二维码（最常用）

1.  「微信客服」→ 点你的客服账号

1.  找**「客服链接」**或**「获取二维码」**

1.  下载二维码图片

这个码你可以放到任何地方 —— 网站、公众号菜单、朋友圈海报、名片、传单、包装盒，随你。

![](img/112a40f47180d8c1c424bb28ab0e8bff.png)

方式二：链接

同一个页面能拿到链接 URL。可以放到：

• 网站上的"在线咨询"按钮

• 短信里发给客户

• 公众号菜单（自定义菜单 → 跳转网页 → 填这个链接）

方式三：嵌入网页或小程序

网页里加个链接就行：

HTML

```
&lt;a href=&quot;客服链接URL&quot;&gt;在线咨询&lt;/a&gt;
```

小程序的话：

JavaScript

```
wx.openCustomerServiceChat({ extInfo: { url: &#x27;客服链接URL&#x27; }, corpId: &#x27;你的企业ID&#x27; })
```

第九步：测试！

1.  掏出手机，打开**个人微信**（不是企业微信哈）

1.  扫上一步保存的二维码

1.  进入对话 — 欢迎语应该自动弹出来了

1.  随便问一句，比如："你好，你们有什么产品？"

1.  等几秒

1.  AI 回复了！

没回复的话，去下面的"常见问题"里找答案。正常情况几秒就有回复。

看到回复了？恭喜！整个工作流搭完了。

下面的内容是排查和进阶，用到了再看。

![](img/4edae389207a542f273f64532b1c4560.png)

常见问题

找不到 openKfId 怎么办？

这不是你一个人的问题。有时候页面里就是不好找，甚至不直接展示。

解决办法：

1.  先确认客服账号已经创建成功

1.  记住客服名称

1.  通过接口把客服账号列表拉出来查 ID

别因为 UI 里没看到，就怀疑自己前面全做错了。

回调明明配了，为什么发消息没反应？

先看你把回调 URL 配在哪。

如果你是配在自建应用里，而不是微信客服后台，这就是高概率原因。wecom-kf这条链路里，回调 URL 要优先在微信客服后台配置。

**客户发消息了，AI 没回复**

三关排查法，哪关断了修哪关：

第 1 关：消息到你服务器了吗？

看日志有没有[wecom-kf] callback received

• 没有 → 消息压根没到。查：URL 对不对、端口开没开、Gateway 在不在跑

• 有 → 到了，查下一关

**第 2 关：消息拉取成功了吗？**

看日志有没有sync_msg

• 报错 → 一般是 corpId 或 corpSecret 填错了，或者 IP 没加白名单

• 正常 → 继续

**第 3 关：AI 处理了吗？**

看日志有没有dispatching to agent或reply sent

• agent 报错 → AI Agent 自己的问题，跟微信客服没关系。查 Agent 配置

• reply sent 但客户没收到 → 看错误码，对照下面的

**报错 95017**

48 小时窗口过期。客户最后一条消息超过 48 小时了，企微不让你再回。

正常客服场景碰不到这个。调试时遇到了，让客户重新发一条就行。

**报错 60030**

接待人员不在应用的可见范围内。

回第二步的应用 → 改「可见范围」→ 把接待人员的部门加进去。

**回复格式乱了（星号井号满天飞）**

微信客服不支持 Markdown。插件会自动转（标题变【标题】，加粗去星号），但有时候不太完美。

解决：在 Agent 的系统提示词里加一句 —— "回复客户用纯文本，不要用 Markdown。"

**回复太长被截断**

企微单条消息限制 2048 字节（大约 680 个汉字）。插件会自动拆成多条，但超过 5 条就被限制了。

解决：在 Agent 提示词里加 —— "回复控制在 500 字以内。"

**没有公网 IP**

**方案一：ngrok 内网穿透**

Bash

```
ngrok http 18789
```

它会给你一个公网地址（像https://abc123.ngrok.io），填到企微回调 URL 里：

Plain Text

```
https://abc123.ngrok.io/wecom-kf
```

注意免费版每次重启地址会变。正式用建议上云服务器。

方案二：VPS + Nginx 反代

用 Nginx 把回调转发到本地，配置里加：

Bash

```
openclaw config set channels.wecom-kf.apiBaseUrl &quot;https://your-vps.example.com&quot;
```

进阶玩法

下面都是可选的。基础功能上面已经搭好了。

**改欢迎语**

Bash

```
openclaw config set channels.wecom-kf.welcomeText &quot;你好呀！我是 XX 品牌的 AI 客服，有啥问我~&quot;
```

小提示：欢迎语有 20 秒有效期，进来 20 秒内发出去，超时就不发了。正常碰不到。

**白名单模式（只让特定客户聊）**

Bash

```
openclaw config set channels.wecom-kf.dmPolicy allowlist
```

然后在配置文件里加：

JSON

```
&quot;allowFrom&quot;: [&quot;external_userid_1&quot;, &quot;external_userid_2&quot;]
```

external_userid在 Gateway 日志里能看到，每个外部用户都有一个。

多客服账号（不同业务线不同 AI）

比如"销售客服"和"技术支持"分别接不同的 AI：

JSON

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
}}}}}```每个账号要在企微后台单独建客服、单独配回调 URL。

分流到不同 Agent：
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

**加粗 / 斜体 / 删除线**

Plain Text

```
**加粗**
*斜体*
~~删除线~~
```

**列表（超常用）**

**无序列表：**

Plain Text

```
- 苹果
- 香蕉
  - 小香蕉（缩进两个空格或一个 Tab）
```

**有序列表：**

Plain Text

```

1. 第一步
2. 第二步
3. 第三步
```

**引用（像“引用一句话”）**

Plain Text

```
&gt; 这是一段引用
&gt; 可以多行
```

**超链接**

Plain Text

```
[显示文字](https://example.com)
```

**图片**

Plain Text

```
![图片说明](图片链接或本地路径)
```

行内代码 / 代码块（写技术内容必备）

Plain Text

```
用 `pip install` 安装依赖
```

**代码块（多行代码）：**

Python

```
print(&quot;hello&quot;)
```

**新手最常踩的坑（提前避雷）**

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

1.2Obsidian 介绍

**Obsidian 是一**款非常受欢迎的本地知识管理和笔记软件，特别适合喜欢用 Markdown 写作、构建个人知识库的人。下面从几个方面帮你快速了解它：

**它是什么？**

Obsidian 本质上是一个 Mar**kdow**n 编辑器，但它最大的特色是支持双向链接——你可以用[[]]语法把笔记之间互相关联起来，形成一张知识网络。它还有一个很酷的"关系图谱"视图，能把你所有笔记之间的关联可视化地展示出来。

**核心优势**

• **数据完全在本地**：笔记以纯 Markdown 文件存储在你自己的电脑上，不依赖任何云服务，隐私性强，也不用担心服务商跑路。

• **双向链接 + 知识图谱**：这是它区别于普通笔记软件的核心功能，帮助你把零散的笔记编织成体系。

• **插件生态极其丰富**：社区开发了上千个插件，从日历、看板、数据库视图、思维导图到与各种服务集成，几乎无所不能。

• **高度可定制**：主题、快捷键、工作区布局都可以自由调整，打造完全属于你的工作流。

**适合谁用？**

• 想搭建"第二大脑"或个人知识库的人

• 喜欢 Markdown 写作的人

• 学生、研究者、写作者、程序员

• 对数据隐私比较在意，不想把笔记交给云端的人

**免费吗？**

个人使用完全免费。如果你需要官方的多设备同步服务（Obsidian Sync）或发布功能（Obsidian Publish），这些是付费的，但你也可以用 iCloud、Git 等免费方案自己实现同步。

**和其他工具对比**

和 Notion 比，Obsidian 更注重本地存储和链接思维，Notion 更偏在线协作和数据库。和 Logseq 比，两者理念相近，但 Obsidian 的插件生态更成熟，Logseq 则默认以大纲模式组织内容。

**上手建议**

刚开始不用追求完美的笔记体系，先随手记，慢慢用双向链接把相关内容串起来，知识网络会自然生长。可以从了解几个核心插件开始，比如日记（Daily Notes）、模板（Templates）、大纲（Outliner）等。

总之，Obsidian 是一个"起点简单、上限极高"的工具，值得尝试。

1.3 Obsidian 的安装

官网链接：https://obsidian.md/

**windows 安装**

下载链接：https://obsidian.md/download

下载安装包

![](img/2d0aa9e4ba78ce221be0a4033e7de832.png)

开始安装

![](img/d95f66b6dd82fceb877bab251a457c4f.png)

提示你权限，选择「是」

![](img/b42603529a5cf872a244eeede38f91df.png)

选择路径

![](img/e2e1f3aa2b9186eca5691c71afe65308.png)

等待完成安装

![](img/7dd0231cb4b0b13953a3b51716d6241e.png)

点击「完成」就可以

![](img/584003ccbbb0edea390d943390cade51.png)

并且完成安装以后，桌面可以看到 Obsidian 的快捷键

![](img/7a99f23c00b577144644b7ec26af21f7.png)

下面的设置可以看下面的章节继续操作

**mac 安装**

下载链接：https://obsidian.md/download

访问以后直接点击下载

![](img/61a9f3a448ea5212e97e4c069d87d0e3.png)

跟其他软件一样，双击打开 DMG 文件

![](img/3a320735428a03718f97f7d3e2ddb567.png)

然后直接拖拽到右边的 Applications 文件夹。

![](img/12e0b50d73b80311282e3befba4c267f.png)

安装就完成了。打开电脑「启动台」，就可以看见 Obsidian 的图标。

![](img/229d6255c8e2b31e87fb0f571c11c6e8.png)

1.4 Obsidian 的初步设置

Obsidian 的所有文档都需要在「仓库」的建立之下，所以需要提前建立好仓库

点击下面的“创建”

![](img/5f897bbcad267ab9bc047d9056995d49.png)

下一步操作

![](img/24684622d15a9b95072d7b2f424cb1fe.png)

浏览的操作步骤如下：可以创建一个目录专门用于保存 Obsidian 的文件

![](img/c053d17b5a5c10e04dcc8ac4893f6892.png)

默认进来的首页：

![](img/1b356fb1829ccd1285b0c4589231a797.png)

1.5 Obsidian 的简单操作

Obsidian 的操作其实很简单

**新建笔记**

在左侧的列表直接右键，就可以看到新建笔记的按钮，直接点击就可以新建笔记

![](img/3ad0fd10eef44f2e4317f2dac6986547.png)

默认如下图

![](img/b053240c83bf212dae4e7c4e5a3725cf.png)

下一步就可以直接修改笔记了

**修改笔记**

直接就输入内容就可以

![](img/e77865d5c3015f7de184b5692c51547e.png)

**插件安装**

按照下面的图操作，注意默认第一次进来，插件需要先关闭安全模式

![](img/42c2db14af3e4b8458c59d48ddca0fb7.png)

下面可以看到“浏览”按钮，点击即可浏览社区插件。

![](img/a1d171912a10d58d943ff874df404dbd.png)

![](img/5bdad991f4a74ef3d04f1f3b216f00c7.png)

2.Claude Code + Obsidian 的实操准备

到这里重头戏才来

Obsidian 作为知识库的管理，Claude Code 相当于作为 AI，我们的助手，助理，更好的辅助的进行知识库管理

让 Obsidian 成为你的大脑

💡Claude Code + Obsidian 的组织管理方式有很多种

我们下面介绍的只是我认为作为大部分最能够接受、最容易接受的一种

后面大家可以灵活运用的关键点如下

1.  Obsidian 的一些特性，比如 canvas 画图的特点，base 数据库。

1.  关于Claude Code，相信前面大家学习的都差不多了，把 Obsidian 的仓库当做一个项目来做就行，原理和方法都是一样的。

2.1准备工作：下载 Obsidian 的仓库模板

为了大家更好的上手 Claude Code + Obsidian 的操作

需要有些准备工作先弄好

主要就是仓库模板

💡

准备好一个新的 Obsidian 的 vault 仓库

这里是别人做好的一个知识库管理的模板

大家如果没有自己的知识管理的可以基于这个模板来搭建

后面掌握好了，可以慢慢的调整属于自己的目录

当前也可以选择其他模板，主要就是要用起来

如果你的 Obsidian 已经有很多的文件，可以让 Claude Code 结合一些知识管理/卡片管理等知识管理理论，帮你梳理，重新整理整个知识体系的层次目录

仓库模板地址：[h](https://github.com/MarsWang42/OrbitOS/blob/main/README_CN.md)ttps://github.com/MarsWang42/OrbitOS/blob/main/README_CN.md

我们在电脑上找好一个目录来存放这个仓库模板

如下图所示，找好一个目录后，直接在地址栏输入「powershell」就可以打开终端

因为下面的操作需要在终端执行

![](img/c49318ae702a9b273da9b1fd3c8f1fbc.png)

mac 苹果电脑可以直接在目录右键，在终端打开

就可以打开终端了，如果没有在终端打开，请安装 iRightMouse 软件

2.1.1 windows 电脑操作

windows 的命令操作会失效，所以这里采用下载直接解压的方式

访问地址：[https://github.co](https://github.com/MarsWang42/OrbitOS)m/MarsWang42/OrbitOS

然后点击下面的下载按钮

![](img/a200b29eca4c6f7bad62254557bf600c.png)

下载完成后如下，其实可以看到是跟网页上显示的看到的是一样的

![](img/2592891c3f7468dbdd27701cf27f1263.png)

我们直接拷贝 CN 的目录，因为这个目录就是最后的 Obsidian 的仓库目录

![](img/19561b84af61358b26ecb895103c154a.png)

然后我重命名为了 orbitos-vault 这个目录

你可以命名成自己想要的目录

目录名都最好都是英文的

![](img/8eb674372d5b89cb69855d76b37d2d56.png)

2.1.2 mac 苹果电脑操作

Plain Text

```
npx degit MarsWang42/OrbitOS/CN orbitos-vault
```

在终端的地方直接粘贴上面的命令

然后进行回车

不要手敲，直接全部复制，不要复制多，不要复制少

windows 直接Ctrl + v就可以粘贴

mac 苹果电脑直接cmd + v粘贴

![](img/739a844944af0658919b0f2a8ad14ad4.png)

然后就可以看到文件夹有一个叫orbitos-vault的目录，就表示已经下载成功。

![](img/b99c8706e75a9f967895426a28337d20.png)

2.2安装 Obsidian 插件：Claudian

前面的步骤完成后，我们可以看到 orbitos-vault 的目录的内容如下：

![](img/f8200a3fb16635b5663435878ff0225f.png)

下面我们就是要安装一个 Obsidian 的插件

💡这个插件就是丝滑的在 Obsidian 上使用 Claude Code

在 Obsidian 的右侧有个对话框，丝滑的对话使用

不过这个插件需要手动安装

比较麻烦

我们就直接交给 Claude Code 安装

![](img/8d2e48381745d7c1ac666f4758486aca.png)

然后就弹出了终端

在终端直接复制下面的命令进入 Claude Code 的 yolo 模式

Plain Text

```
claude  --dangerously-skip-permissions
```

![](img/0a3784fb2cd778bdcb38e3ff0d8034c9.png)

第一次进来会有提示

记得选择 yes 的选项，然后再回车继续

![](img/b477c0729f3442772bd6a3451c1b0989.png)

直接输入如下提示词，等待安装完成

Plain Text

```
https://github.com/YishenTu/claudian
这个是 Obsidian 的插件，帮我安装到当前目录的 vault 下
```

![](img/56f7ff99d4ad168fb22fcc6350c54212.png)

等待完成就可以看到类似如下的总结信息

表示已经安装完成

![](img/75eec54503c8e19d35bb2ce90e888587.png)

下面我们先打开准备好的仓库目录

![](img/c32b197442d1736b6d1ebd2cd2acebd5.png)

弹出下面的界面

点击「打开」按钮

![](img/d00bfa2cb0bdb46c28fca70b82e83881.png)

选择前面准备的目录

![](img/d0b73f8661705075109f13c9beca1cae.png)

如果看到下面的提示这个

需要选择信任插件

![](img/e8ebf959dadc654b3eaf9d47de2d4254.png)

然后就可以看到如下界面

我们打开 Claudian 的插件的开关

![](img/71d0c6f71e380b15f545747f0ecadcdb.png)

然后关闭上个页面

回到首页

按照如下图操作

![](img/491205da989ec2e61aa2145dd520d409.png)

如果能正常回复，就表示插件已经安装成功了

另外 windows 的还需要额外的拷贝下 skills 的目录

![](img/3455e15c760c6b75db9f979a695d31ef.png)

![](img/b9583346c0d709c0709e5cc4a3c74d76.png)

![](img/9e79955cdfa1acd9ffe6738710cb4e72.png)

2.3安装需要的 skills

需要先给 Claude Code 安装 skills

地址：[h](https://github.com/kepano/obsidian-skills?tab=readme-ov-file)ttps://github.com/kepano/obsidian-skills?tab=readme-ov-file

这个 skills 来自于 Obsidian 的官方。所以它肯定是最权威的。

Plain Text

```
https://github.com/kepano/obsidian-skills
这个下面的 skills 帮我安装到这个项目下
```

截图如下：

![](img/733c813fde0ccdd72753e30b6c6f2755.png)

前面的基本准备工作就弄好了

下面就可以开始你的 Obsidian 的大脑了

![](img/fae40898690cb1aee6467cd4e7f82a89.png)

3.Claude Code+Obsidian 初级玩法

💡下面的案例都都是带领大家入门

大家用熟悉之后可以按照自己的思路来玩

并且 Obsidian 的玩法很多

Claude Code 当前作为通用 agent 后玩法也很多

所以综合两者，玩法其实很多，所以大家后面玩熟悉了

可以有很多的玩法的

3.1开启今日之路

这个很简单，已经配置好自定义命令。

直接使用就可以

![](img/08ae8181c74b6f5f3061148685b5ead2.png)

主要就是去搜集相关资料

你有什么想法没有

然后沉淀到对应的目录里

Plain Text

```
/start-my-day
```

然后就开启了今日的规划

![](img/0727407901547dadc0ae51e88eb6f3e3.png)

详细的截图大概操作如下：

![](img/9d89148954cd488b8de8fc1352b66c82.png)

显示的结果信息：

![](img/03c374a8928b43d566147140af1b5020.png)

并且还有个 0305 的日记

![](img/8656025e0edcc3d2e1f6dae75e9f9da6.png)

并且你的想法是记录到收件箱的

方便后续整理

![](img/a958b31db3c266d1868843c05f6d6fff.png)

3.2回顾 2025

Plain Text

```
帮我回顾下 2025 的内容
```

![](img/c87cf34d0e24156b69d107aad2f52210.png)

总结内容如下：

![](img/b0b9c6197e6a9715c83fba43bea2a456.png)

3.3创建 canvas 画布内容

直接就输入如下的提示词就

Plain Text

```
帮我画一个明代的历史以及各个皇帝的canvas
```

![](img/d92deaa310bcafe95189cfb21f7baf48.png)

生成以后就可以打开了

![](img/bd8f7c401ed843708bcfff3ee2de7546.png)

![](img/6813aff78c3965af0508a28ca159d3cc.png)

4.Claude Code+Obsidian 进阶玩法

这里还是以我们整体的主题：搭建我们的第二大脑

首先需要的是思考下目录是否合适的问题

4.1 再次思考目录

[我们再来回顾看下之前下载的模板，地](https://github.com/MarsWang42/OrbitOS)址是：https://github.com/MarsWang42/OrbitOS

这个项目的目录是这样参考的：

OrbitOS 用自创的

**C.A.P 项目结构**

（Context/Actions/Progress），并将知识拆分为 Research（研究笔记）、Wiki（原子概念）、Resources（精选内容）三层

![](img/ee9707a7e67ec856b548e51b7dfaac5c.png)

[另外我们还可以参考到另外一个项目：https](https://github.com/heyitsnoah/claudesidian)://github.com/heyitsnoah/claudesidian

它的目录是这样参考的。

**Claudes**idian 用经典PARA 方法（Projects/Areas/Resources/Archive）

![](img/f285444de05e61ca52be9be4fbd35653.png)

其实两者差不多，我用 Claude Code 来了分对比总结

大家可以参考下。

![](img/2c873fcc0af4d4e82a48f8a81cb0e438.png)

其实对比下来，都有各自的优势

如果你还不知道怎么弄，我觉得就用 OrbitOS 的也可以，后面都是可以随时调整的

然后我这里也公布下我的目录，大家可以参考

我主要就是关注的是几个点：

1.  内容创作：我的主要平台就是：公众号/推特/Youtube/B 站

1.  建站变现：主要就是 AI 产品/Saas 类服务

1.  工具箱：会存储一些电脑使用软件，以及一些其他信息

1.  学习笔记：一些学习知识的笔记

1.  收藏箱：这个是重点，有时候会看公众号文章，后者是一些有用的聊天记录，或者是 x 好的文章，都需要收藏，然后做整理用

![](img/300be55a57e279ed0528b7a246c04d2e.png)

4.2 内容创作流程

这里就说下内容创作的主要过程，其实主要就是两个点

1.  内容创作，你的文章如何写，你的小红书图片如何配置

1.  平台分发，内容写好后，如何快速发到平台，比如公众号排版

下面来分开说下具体怎么弄了

4.2.1 内容创作

这里其实借鉴的是「李默 AI 实战」公众号的文章里面的内容创作。

当然这里的形式也有很多，主要核心就是：使用 AI 工具来对我们想要写的主题生成文章，包括里面的配图

当然这里重要的还是使用 skills 技能来抽取

提示词感谢 钱塘江鲤 提供，并且经得本人同意拿来到此

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

下面就是在 Claudian 直接发过去后，生成的记录

![](img/01ee70e0b12690131279a93a0b5f28c5.png)

可以最后看到还需要一个 key

直接访问这个地址：

[ht](https://signin.volcengine.com/auth/login?redirectURI=https%3A%2F%2Fconsole.volcengine.com%2Fark%2Fregion%3Aark%2Bcn-beijing%2Fmodel%2Fdetail%3FId%3Ddoubao-seedream-4-5)tps://console.volcengine.com/ark/region:ark+cn-beijing/model/detail?Id=doubao-seedream-4-5

如下图所示，找到「API 接入」按钮，点击后，如下图所示

然后点击「创建 API Key」，如果是已经有了，就会像这张截图类似，会有一个存在的 key，复制

![](img/567ba9989188e2a4bc54bbe9ed8309ef.png)

复制完上面的 key 后，就可以直接粘贴到 Claudian 对话框，CC 会替你直接保存 key 信息

![](img/e5f6faa11bb95a1a45e7de0cedf882cd.png)

然后重启 Obsidian

直接使用 /rewirtepost 这个命令，后面跟上你需要写的主题的文章链接就可以

Markdown

```
/rewritepost https://claude.com/blog/1m-context-ga
```

![](img/a1341f949be00ea139d59a9854e37499.png)

当然最后的文章看了下有封面，剩下就是文字，后面可以继续优化这个 skills，让文章中间也生成图片。

这个可以留给大家继续优化了。

4.2.2 平台分发

上面写好文章了，那么下面就需要发布到公众号。

这里我们用公众号来举例。

当然我们也是使用 skills 来做这件事情

💡为什么要用 skills 做这件事情：

1.  比插件更灵活，有什么问题、或者有什么需要调整的，自己直接调整就行

1.  结合 Claude Code/Codex 工具更加智能

我们要安装的也是前面介绍过的 baoyu-skills，里面就有发布微信公众号的 skills，当然也有发布微博、发布 x 的，大家都可以尝试下。

下面我们来用发布微信公众号来举例，进行演示

首先我们需要安装 skills，直接发送下面的提示词到 Claudian 就可以

Markdown

```
帮我安装下面的 skills 到这个项目级别
https://github.com/JimLiu/baoyu-skills
```

![](img/fc76fd06b9d1dd20ed53e0991f284014.png)

到此，就完全安装成功了。

下面直接可以用提示词来让 Claude Code 给我们发微信公众号文章。

Markdown

```
@claude-1m-context_story.md 这篇文章发送到公众号草稿箱
```

肯定会提示你 AppID 和 AppSecret 的问题，我们按照手册的步骤去操作就行

![](img/0a0253b37e71176334a898401304faf3.png)

但我们打开微信公众平台的时候

找到「账号设置」，就会有 AppID 信息

但是我们发现没有 AppSecret 信息

那是因为换地方了

![](img/7d19b1fe44829840cb010fffc6bd0501.png)

我们打开一个新的网站，那句是微信开发者平台

https://developers.weixin.qq.com

点击公众号进去

![](img/0a6e21840fbde8b9924852f3ed7c864d.png)

下面的图就可以看到 AppSecret 了

如果是第一次，应该有个激活的，激活下就行

特别注意这个是一次性的，第一次复制后，好好保存到本地

你看下面的图就是第二次打开，是没法复制的，只能重置

要是你实在忘记了，没办法，就只能重置了。

![](img/90da345486bec53393831c1880269011.png)

然后我们使用 vscode 打开仓库目录下的 。baoyu-skills

看到如下图的操作

注意：最后要记得保存文件

文件内容模板：（记得把{xxx}的内容换成你的就行，注意括号也需要全部换掉）

Markdown

```
WECHAT_APP_ID={换成你的 app id}
WECHAT_APP_SECRET={换成你的 app Secret}
```

![](img/cf77f929bbc84e983cc5bb2de04915be.png)

保存好文件后，然后再回到 Claudian 的窗口，继续发文章就行

4.3 知识沉淀

沉淀的只是有一部分我理解就是来自于收藏的内容，比如公众号文章、一些有用的对话消息，还有网页的

这里主要讲解的就是“收藏箱”里面的内容，讲一下

4.3.1 浏览器收藏

那就是下载一个插件就行

直接谷歌浏览器市场搜索：Obsidian Web Clipper

直接下载安装就可以

![](img/551ffea4fa50b32a1d3bce7bedf4da16.png)

如何使用了？

打开一个网页后，如果想收藏。

那么就直接点击插件图标。

然后就会出现这个网站的一些信息，有些网站还能把内容都提取出来。

直接点击下面的按钮：「Add to Obsidian」就可以。

![](img/bb6c8a1eed7448baface0c729292fb68.png)

然后会提示你打开 Obsidian 的 app

![](img/4a60eaf54842e2ccb6db5e89023d2b1c.png)

然后就会收藏到 Obsidian 的目录下了

默认是在 Clippings 目录下，你也可以修改

修改就是在插件下面有个目录是可以修改的

![](img/b87d8da603de3613d605c506376269f1.png)

4.3.2 微信收藏

下面这里说微信公众号文章和微信消息如何收藏

这里我用的是一个插件

怎么使用了，直接将需要的文章和信息，或者是链接直接发送到这个 MpClipper 的对话框

![](img/935f5d7bff4910130696be6dacc668b5.png)

然后再 Obsidian 需要安装一个 MpClipper Sync 的插件

就可以把公众号文章和消息同步到 Obsidian 的目录下

![](img/72557273702bc80e7d4cd25ce419934a.png)

看下我同步的文章

我把他都同步到了90.收藏箱/微信剪藏的目录下，并且可以按照时间目录整理

![](img/03c2189ffdff8df131ba2da036e7a2dd.png)

下面详细说下步骤如何弄，步骤有点麻烦，大家可以耐心操作

💡注意事项：这个插件提供 30 条的收藏免费次数

额外使用时需要付费的，介意的童鞋请注意

**🔧 第一步：小程序端配置**

在微信里搜索**NotionMpClipper**小程序，并点击打开

1.  进入 【NotionMpClipper 小程序】-【我的】-【Obsidian】页面。按照提示配置图床，支持阿里云、腾讯云、缤纷云、cloudflare r2、以及各类兼容 S3 协议的对象存储服务。

![](img/660f9a99c854ab7f59e88a62dcaa2814.png)

![](img/f6290e138b5b76bd5b6b3004669554cc.png)

• 会员权限，这个是需要会员的

• 图床可以选择 bitiful，或者腾讯云的阿里云的都可以，地址：https://www.bitiful.com/，有 50G 的免费额度

• 打开保存到 Obsidian 的开关

1.  进入【NotionMpClipper 小程序】-【我的】-【个性设置】页面。将【保存到 Obsidian】这个开关打开。

![](img/3cabf5bb2057cb1fed48a090fcd92e50.png)

💻 第二步：Obsidian 插件安装

可以直接从这里下载

[

![](img/246675fa31e37c67e5328d91bae926e3.png)

mpclipper-sync(1).zip](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/CnT8bh6FzoZeLFxoJe1cQ465ndh?response-content-disposition=attachment%3B%20filename%3D%22mpclipper-sync%281%29.zip%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260526%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260526T134041Z&x-oss-expires=86400&x-oss-signature=4d1b27630d2b18cb403badb82ef73bcc25d67d26626c6cb933d62525ac3809e0&x-oss-signature-version=OSS4-HMAC-SHA256)

下载插件后导入安装到 Obsidian 中，然后完成插件的配置。

为了方便用户配置插件，我在小程序-【我的】-【Obsidian】页面提供了一个复制 Obsidian 配置的按钮，你可以直接复制到剪贴板中，然后保存到你的记事本里，再复制到 Obsidian 插件配置表单。

![](img/9696a5acb7a8255026d0396626b2fc41.png)

⚠️ 第三步：图床 CORS 配置

有一个特别需要注意的配置：无论你使用什**么图床，你都需要去**图床平台增加一项配置：CORS 跨域配置。

比如这里使用的就是：https://www.bitiful.com/

![](img/435b06ca2b66b03519e83e5d4bae8b88.png)

我这里给了一份缤纷云的参考，其他图床也是这样配置。

配置好之后，剪藏流程和之前完全一样。你可以把文章链接发送给小程序剪藏，也可以通过微信收藏助手来剪藏。

**请注意**

：开启 Obsidian 剪藏后，Notion 的剪藏功能将自动停用，反之亦然。两者是互斥关系，你可以随时在设置中切换回来。

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
/bin/bash -c &quot;$(curl -fsSL https://raw.githubusercontent.com/trycua/cua/main/libs/lume/scripts/install.sh)&quot;
```

如果~/.local/bin不在你的 PATH 中：

Ada

```
echo &#x27;export PATH=&quot;$PATH:$HOME/.local/bin&quot;&#x27; &gt;&gt; ~/.zshrc &amp;&amp; source ~/.zshrc
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
ssh youruser{&quot;id&quot;:117325,&quot;name&quot;:&quot;锋度&quot;,&quot;xq_group_number&quot;:192,&quot;avatar&quot;:&quot;https://search01.shengcaiyoushu.com/upload/avatar/FpBm3I9cPVn9OGK9x22S3md6Eahb&quot;}.168.64.X
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
npx -y @larksuite/openclaw-lark-tools install
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
第一阶段：环境准备 ────────────── 🏁 看到 waoowaoo 首页，API 连接全绿
↓第二阶段：故事变分镜 ─────────── 🏁 看到 AI 分析出的角色和画面描述
↓第三阶段：分镜变画面和声音 ──── 🏁 看到第一张漫画图 + 听到角色配音
↓第四阶段：画面变完整视频 ────── 🏁 下载到一个完整的 MP4 文件
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
ssh root@你的服务器IP
```

回车，输密码。看到类似root@server:~#的东西，就进去了。

连不上？先看看 IP 有没有打错。提示Connection refused的话，多半是服务器的 22 端口没开，找你的 VPS 服务商开一下就行。

**然后一键装 waoowaoo。**

把下面这行复制粘贴进去，回车：

Bash

```
curl -fsSL https://cnb.cool/fuliai/waoowaoo/-/git/raw/main/install.sh | bash
```

脚本会自动帮你装 Docker、下载 waoowaoo、把所有服务拉起来。大概 3-5 分钟。

装的过程中会问你几个问题，一路回车就行。装完会告诉你访问地址。

如果你的服务器已经装过了，跳过安装，直接确认服务还活着：

Bash

```
cd /opt/waoowaoo &amp;&amp; docker compose ps
```

看到所有服务状态都是Up或running就行。有没跑起来的：

Bash

```
docker compose up -d
```

**打开浏览器看看。**

在你自己的电脑上，浏览器访问：

Plain Text

```
http://你的服务器IP:13000
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
# 把邮箱和密码换成你自己的
MY_EMAIL=&quot;你的邮箱&quot;
MY_PASSWORD=&quot;你的密码&quot;

rm -f /tmp/auth_cookies.txt
CSRF=$(curl -s -c /tmp/auth_cookies.txt http://localhost:13000/api/auth/csrf | python3 -c &quot;import json,sys; print(json.load(sys.stdin)[&#x27;csrfToken&#x27;])&quot;)
curl -s -c /tmp/auth_cookies.txt -b /tmp/auth_cookies.txt \
  -X POST http://localhost:13000/api/auth/callback/credentials \
  -H &quot;Content-Type: application/x-www-form-urlencoded&quot; \
  -d &quot;csrfToken=$CSRF&amp;username=$MY_EMAIL&amp;password=$MY_PASSWORD&amp;callbackUrl=http%3A%2F%2Flocalhost%3A13000&quot; &gt; /dev/null
echo &quot;✅ 登录完成&quot;
```

然后配 Key：

Bash

```
# 把三个 Key 换成你自己的
curl -s -b /tmp/auth_cookies.txt \
  -X PUT http://localhost:13000/api/user/api-config \
  -H &quot;Content-Type: application/json&quot; \
  -d &#x27;{
    &quot;providers&quot;: [
      {&quot;id&quot;: &quot;ark&quot;, &quot;name&quot;: &quot;火山引擎 Ark&quot;, &quot;apiKey&quot;: &quot;你的ARK_API_KEY&quot;},
      {&quot;id&quot;: &quot;google&quot;, &quot;name&quot;: &quot;Google&quot;, &quot;apiKey&quot;: &quot;你的GOOGLE_API_KEY&quot;},
      {&quot;id&quot;: &quot;fal&quot;, &quot;name&quot;: &quot;FAL&quot;, &quot;apiKey&quot;: &quot;你的FAL_API_KEY&quot;}

]}&#x27;echo &quot;✅ API Key 配置完成&quot;
```

1.4 环境检查

正式开干之前，跑一下这个，确认工具都在：

Bash

```
echo &quot;=== 环境检查 ===&quot;
for cmd in curl python3 docker ffmpeg; do
  if command -v $cmd &gt; /dev/null 2&gt;&amp;1; then
    echo &quot;✅ $cmd 已安装&quot;
  else
    echo &quot;❌ $cmd 未安装，请先安装&quot;
  fi
done
echo &quot;&quot;
echo &quot;=== 服务检查 ===&quot;
HTTP_CODE=$(curl -s -o /dev/null -w &quot;%{http_code}&quot; http://localhost:13000)
if [ &quot;$HTTP_CODE&quot; = &quot;200&quot; ] || [ &quot;$HTTP_CODE&quot; = &quot;302&quot; ]; then
  echo &quot;✅ waoowaoo 服务正常（HTTP $HTTP_CODE）&quot;
else
  echo &quot;❌ waoowaoo 服务异常（HTTP $HTTP_CODE），请运行: cd /opt/waoowaoo &amp;&amp; docker compose up -d&quot;
fi
```

ffmpeg 没装的话：

Bash

```
apt update &amp;&amp; apt install -y ffmpeg
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
MY_EMAIL=&quot;你的邮箱&quot;
MY_PASSWORD=&quot;你的密码&quot;

rm -f /tmp/auth_cookies.txt
CSRF=$(curl -s -c /tmp/auth_cookies.txt http://localhost:13000/api/auth/csrf | python3 -c &quot;import json,sys; print(json.load(sys.stdin)[&#x27;csrfToken&#x27;])&quot;)
curl -s -c /tmp/auth_cookies.txt -b /tmp/auth_cookies.txt \
  -X POST http://localhost:13000/api/auth/callback/credentials \
  -H &quot;Content-Type: application/x-www-form-urlencoded&quot; \
  -d &quot;csrfToken=$CSRF&amp;username=$MY_EMAIL&amp;password=$MY_PASSWORD&amp;callbackUrl=http%3A%2F%2Flocalhost%3A13000&quot; &gt; /dev/null
echo &quot;✅ 登录完成&quot;
```

这个命令干了什么事呢？它在/tmp/auth_cookies.txt里存了一张临时"身份证"。后面每个命令都会带着这张身份证去请求。

关了终端窗口重新连的话，这张身份证就作废了，得重新跑一遍这个登录。

2.2 创建项目

Bash

```
PROJECT=$(curl -s -b /tmp/auth_cookies.txt \
  -X POST http://localhost:13000/api/projects \
  -H &quot;Content-Type: application/json&quot; \
  -d &#x27;{&quot;name&quot;: &quot;我的第一条AI漫剧&quot;, &quot;description&quot;: &quot;第一次尝试&quot;}&#x27;)
PROJECT_ID=$(echo $PROJECT | python3 -c &quot;import json,sys; print(json.load(sys.stdin)[&#x27;project&#x27;][&#x27;projectId&#x27;])&quot;)
echo &quot;✅ 项目创建成功，ID = $PROJECT_ID&quot;

# 把 ID 保存到文件，防止终端断开后丢失
echo &quot;PROJECT_ID=$PROJECT_ID&quot; &gt; /tmp/waoowaoo_session.env
```

我的第一条AI漫剧你可以换成自己喜欢的名字。

**终端断开了怎么办？**

别慌。重新连上后先跑登录命令，然后：

Bash

```
# 方法1：之前保存过的话
source /tmp/waoowaoo_session.env
echo $PROJECT_ID

# 方法2：查所有项目列表
curl -s -b /tmp/auth_cookies.txt http://localhost:13000/api/projects | python3 -c &quot;
import json,sys
for p in json.load(sys.stdin)[&#x27;projects&#x27;]:
    print(p[&#x27;projectId&#x27;], p[&#x27;name&#x27;])
&quot;
# 然后手动设置：PROJECT_ID=你看到的那个ID
```

2.3 创建剧集并写入故事

**先创建一个剧集。**

Bash

```
EP=$(curl -s -b /tmp/auth_cookies.txt \
  -X POST &quot;http://localhost:13000/api/novel-promotion/$PROJECT_ID/episodes&quot; \
  -H &quot;Content-Type: application/json&quot; \
  -d &#x27;{&quot;name&quot;: &quot;第一集&quot;}&#x27;)
EPISODE_ID=$(echo $EP | python3 -c &quot;import json,sys; print(json.load(sys.stdin)[&#x27;episode&#x27;][&#x27;id&#x27;])&quot;)
echo &quot;✅ 剧集创建成功，ID = $EPISODE_ID&quot;

# 保存 ID
echo &quot;EPISODE_ID=$EPISODE_ID&quot; &gt;&gt; /tmp/waoowaoo_session.env
```

**然后写你的故事。**

用nano打开一个文件：

Bash

```
nano /tmp/story.txt
```

把你的故事粘贴进去。下面是示例，你换成自己的就行：

Plain Text

```
在一片古老的森林边缘，住着一只小狐狸叫阿金。阿金有着橙红色的毛和一条蓬松的大尾巴，最喜欢在傍晚时分坐在大石头上，望着夕阳发呆。

这天傍晚，阿金正在发呆，突然看见一只小松鼠跑了过来，气喘吁吁地说：「阿金阿金！森林深处有一棵会说话的树，你敢去看看吗？」

阿金想了想，笑着说：「当然敢！不过我们要带上蜂蜜饼干，万一那棵树喜欢甜食呢？」

两个小家伙就这样出发了，踏上了一段没有人知道结局的冒险。
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
STORY_TEXT=$(cat /tmp/story.txt)
curl -s -b /tmp/auth_cookies.txt \
  -X PATCH &quot;http://localhost:13000/api/novel-promotion/$PROJECT_ID/episodes/$EPISODE_ID&quot; \
  -H &quot;Content-Type: application/json&quot; \
  -d &quot;{\&quot;novelText\&quot;: $(python3 -c &quot;import json; print(json.dumps(open(&#x27;/tmp/story.txt&#x27;).read()))&quot;)}&quot; &gt; /dev/null
echo &quot;✅ 故事写入成功&quot;
```

2.4 让 AI 分析故事

接下来让 AI "读"你的故事。它会分析出有哪些角色、长什么样、每个场景在讲什么。

Bash

```
echo &quot;⏳ AI 正在分析你的故事...&quot;
TASK=$(curl -s -b /tmp/auth_cookies.txt \
  -X POST &quot;http://localhost:13000/api/novel-promotion/$PROJECT_ID/analyze-global&quot; \
  -H &quot;Content-Type: application/json&quot; \
  -d &quot;{\&quot;episodeId\&quot;: \&quot;$EPISODE_ID\&quot;, \&quot;locale\&quot;: \&quot;zh\&quot;}&quot;)
TASK_ID=$(echo $TASK | python3 -c &quot;import json,sys; print(json.load(sys.stdin).get(&#x27;taskId&#x27;,&#x27;?&#x27;))&quot;)

# 自动等待完成（最多等 3 分钟）
for i in $(seq 1 36); do
  sleep 5
  STATUS=$(curl -s -b /tmp/auth_cookies.txt &quot;http://localhost:13000/api/tasks/$TASK_ID&quot; | python3 -c &quot;import json,sys; print(json.load(sys.stdin).get(&#x27;task&#x27;,{}).get(&#x27;status&#x27;,&#x27;&#x27;))&quot;)
  if [ &quot;$STATUS&quot; = &quot;completed&quot; ]; then echo &quot;✅ 故事分析完成！&quot;; break; fi
  if [ &quot;$STATUS&quot; = &quot;failed&quot; ]; then echo &quot;❌ 分析失败，请检查 Google API Key 是否配置正确，以及服务器是否能访问 Google&quot;; break; fi
  echo &quot;  等待中... ($i/36) 状态: $STATUS&quot;
done
```

失败了？十有八九是 Google API 连不上。检查一下你的服务器是不是在海外，或者有没有配代理。

2.5 生成片段

AI 读完故事后，要把故事切成一个个小片段。每个片段对应一张图。

Bash

```
echo &quot;⏳ 正在切分故事片段...&quot;
CLIP_RESULT=$(curl -s -b /tmp/auth_cookies.txt \
  -X POST &quot;http://localhost:13000/api/novel-promotion/$PROJECT_ID/clips&quot; \
  -H &quot;Content-Type: application/json&quot; \
  -d &quot;{\&quot;episodeId\&quot;: \&quot;$EPISODE_ID\&quot;, \&quot;locale\&quot;: \&quot;zh\&quot;}&quot;)

# 等待并确认片段生成完成
for i in $(seq 1 12); do
  sleep 5
  CLIP_COUNT=$(curl -s -b /tmp/auth_cookies.txt \
    &quot;http://localhost:13000/api/novel-promotion/$PROJECT_ID/episodes/$EPISODE_ID&quot; | \
    python3 -c &quot;import json,sys; d=json.load(sys.stdin); print(len(d.get(&#x27;episode&#x27;,{}).get(&#x27;clips&#x27;,[])))&quot; 2&gt;/dev/null)
  if [ &quot;$CLIP_COUNT&quot; != &quot;0&quot; ] &amp;&amp; [ -n &quot;$CLIP_COUNT&quot; ]; then
    echo &quot;✅ 片段生成完成，共 $CLIP_COUNT 个片段&quot;
    break
  fi
  echo &quot;  等待中... ($i/12)&quot;
done
```

这步特别容易被跳过。但你不能跳——不做这步，下一步会直接报错No clips found。别问我怎么知道的。

2.6 生成分镜

现在 AI 要给每个片段写一份"分镜"：这张图画什么构图、什么角色、什么表情动作。

就像导演拿着剧本画分镜头脚本。AI 就是那个导演。

Bash

```
echo &quot;⏳ 正在生成分镜（约 2 分钟）...&quot;
TASK=$(curl -s -b /tmp/auth_cookies.txt \
  -X POST &quot;http://localhost:13000/api/novel-promotion/$PROJECT_ID/script-to-storyboard-stream&quot; \
  -H &quot;Content-Type: application/json&quot; \
  -d &quot;{\&quot;episodeId\&quot;: \&quot;$EPISODE_ID\&quot;, \&quot;locale\&quot;: \&quot;zh\&quot;}&quot;)
TASK_ID=$(echo $TASK | python3 -c &quot;import json,sys; print(json.load(sys.stdin).get(&#x27;taskId&#x27;,&#x27;?&#x27;))&quot;)

for i in $(seq 1 36); do
  sleep 5
  STATUS=$(curl -s -b /tmp/auth_cookies.txt &quot;http://localhost:13000/api/tasks/$TASK_ID&quot; | python3 -c &quot;import json,sys; print(json.load(sys.stdin).get(&#x27;task&#x27;,{}).get(&#x27;status&#x27;,&#x27;&#x27;))&quot;)
  if [ &quot;$STATUS&quot; = &quot;completed&quot; ]; then echo &quot;✅ 分镜生成完成！&quot;; break; fi
  if [ &quot;$STATUS&quot; = &quot;failed&quot; ]; then echo &quot;❌ 分镜生成失败，请重新运行本步骤&quot;; break; fi
  echo &quot;  等待中... ($i/36) 状态: $STATUS&quot;
done
```

![](img/fb2cf072a4fc6c31bcbc9a84f547f8db.png)

第三阶段：分镜变画面和声音

这个阶段结束后，每个分镜都会有一张漫画图片，每个角色都有了自己的声音。

如果说上一步是导演画分镜，这一步就是画师照着分镜一张一张画，配音演员照着台词一句一句录。只不过画师和配音演员都是 AI。

3.1 生成所有图片

每张分镜会发给火山引擎的 Seedream 4.5 模型。AI 根据描述画一张漫画风格的图。大概 30 张图并发着跑，3-5 分钟搞定。

Bash

```
echo &quot;⏳ 正在生成图片...&quot;

cat &gt; /tmp/submit_panels.py &lt;&lt; &#x27;PYEOF&#x27;
import json, subprocess, sys, time

PROJECT_ID = sys.argv[1]
EPISODE_ID = sys.argv[2]

d = json.loads(subprocess.check_output([
    &quot;curl&quot;, &quot;-s&quot;, &quot;-b&quot;, &quot;/tmp/auth_cookies.txt&quot;,
    f&quot;http://localhost:13000/api/novel-promotion/{PROJECT_ID}/episodes/{EPISODE_ID}&quot;
]).decode())

panels = []
for sb in d.get(&quot;episode&quot;, {}).get(&quot;storyboards&quot;, []):
    for p in sb.get(&quot;panels&quot;, []):
        if not p.get(&quot;imageUrl&quot;):
            panels.append(p[&quot;id&quot;])

if not panels:
    print(&quot;所有图片已生成，无需重复操作&quot;)
    sys.exit(0)

print(f&quot;共 {len(panels)} 张图片需要生成&quot;)
for i, pid in enumerate(panels):
    r = json.loads(subprocess.check_output([
        &quot;curl&quot;, &quot;-s&quot;, &quot;-b&quot;, &quot;/tmp/auth_cookies.txt&quot;,
        &quot;-X&quot;, &quot;POST&quot;, f&quot;http://localhost:13000/api/novel-promotion/{PROJECT_ID}/regenerate-panel-image&quot;,
        &quot;-H&quot;, &quot;Content-Type: application/json&quot;,
        &quot;-d&quot;, json.dumps({&quot;panelId&quot;: pid, &quot;locale&quot;: &quot;zh&quot;, &quot;count&quot;: 1})
    ]).decode())
    print(f&quot;  [{i+1}/{len(panels)}] 已提交&quot;)
    time.sleep(0.3)

print(&quot;全部提交完毕，等待 AI 画图中...&quot;)
PYEOF

python3 /tmp/submit_panels.py $PROJECT_ID $EPISODE_ID
```

然后等它画完：

Bash

```
echo &quot;⏳ 等待图片生成（每 15 秒检查一次）...&quot;
for i in $(seq 1 20); do
  sleep 15
  RESULT=$(curl -s -b /tmp/auth_cookies.txt \
    &quot;http://localhost:13000/api/novel-promotion/$PROJECT_ID/episodes/$EPISODE_ID&quot; | \
    python3 -c &quot;
import json,sys
d = json.load(sys.stdin)
panels = [p for sb in d[&#x27;episode&#x27;][&#x27;storyboards&#x27;] for p in sb[&#x27;panels&#x27;]]
done = sum(1 for p in panels if p.get(&#x27;imageUrl&#x27;))
print(f&#x27;{done}/{len(panels)}&#x27;)
if done == len(panels): sys.exit(0)
else: sys.exit(1)
&quot;)echo &quot;  图片进度: $RESULT ($i/20)&quot;
  if [ $? -eq 0 ]; then echo &quot;✅ 所有图片生成完成！&quot;; break; fi
done
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
pip install edge-tts -q 2&gt;/dev/null

# 生成一个少年男声（给男性角色用）
edge-tts --voice zh-CN-YunxiNeural --text &quot;你好，我是这个故事里的角色，我的声音听起来是这样的&quot; \
  --write-media /tmp/voice_male.mp3

# 生成一个活泼女声（给女性角色用）
edge-tts --voice zh-CN-XiaoxiaoNeural --text &quot;你好，我是这个故事里的角色，我的声音听起来是这样的&quot; \
  --write-media /tmp/voice_female.mp3

echo &quot;✅ 参考音频生成完成&quot;
```

然后传到 waoowaoo 的存储里：

Bash

```
# 上传到 MinIO 存储（waoowaoo 的文件服务）
docker cp /tmp/voice_male.mp3 waoowaoo-minio:/data/uploads/voice_male.mp3 2&gt;/dev/null || \
  cp /tmp/voice_male.mp3 /opt/waoowaoo/data/uploads/voice_male.mp3

docker cp /tmp/voice_female.mp3 waoowaoo-minio:/data/uploads/voice_female.mp3 2&gt;/dev/null || \
  cp /tmp/voice_female.mp3 /opt/waoowaoo/data/uploads/voice_female.mp3

echo &quot;✅ 音频已上传&quot;
```

想要更真实的声音？录一段你自己的（或者你想要的任何声音），5-10 秒就够了，保存成 MP3 替换上面的文件就行。Index TTS 2 会模仿你的声音来念台词，效果好很多。

第二步：看看你的故事里有哪些角色

Bash

```
echo &quot;=== 你的故事里有这些角色 ===&quot;
curl -s -b /tmp/auth_cookies.txt \
  &quot;http://localhost:13000/api/novel-promotion/$PROJECT_ID/episodes/$EPISODE_ID&quot; | \
  python3 -c &quot;
import json,sys
d = json.load(sys.stdin)
vl = d.get(&#x27;episode&#x27;,{}).get(&#x27;voiceLines&#x27;,[])
speakers = sorted(set(v.get(&#x27;speaker&#x27;,&#x27;&#x27;) for v in vl))
for s in speakers:
    count = sum(1 for v in vl if v.get(&#x27;speaker&#x27;)==s)
    print(f&#x27;  {s}（{count}句台词）&#x27;)
&quot;```你会看到类似这样的：
```

Plain Text

```
=== 你的故事里有这些角色 ===
  旁白（4句台词）
  阿金（2句台词）

  小松鼠（1句台词）
```

**第三步：设置每个角色用哪个声音**

下面这个脚本帮你把角色和声音对应起来。你需要改的只有VOICE_MAP那几行：

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
```注意：VOICE_MAP里的角色名必须和第二步看到的一模一样。差一个字都不行。

**第四步：分析配音**

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

**第五步：生成所有配音**

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

到这一步，你已经有了所有的图片和配音。

现在要让静态的图片"动"起来。AI 会把每张漫画图变成 4 秒的动态视频片段，最后你把它们合成一条完整视频。

这就像动画工作室拿着原画做动画，再剪辑合成。只不过这里全是 AI 在干。

4.1 生成视频片段

这是整个流程里最慢的一步。

每张图要发给火山引擎的 Seedance 模型，让 AI 算出怎么让画面动起来。大概 30 段视频，每段 4 秒，全部跑完要 60 分钟左右。

提交完请求后你可以放心去干别的，回来再看。

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

关于generationOptions这三个参数（generateAudio+duration+resolution），必须三个都写。缺一个就会报VIDEO_CAPABILITY_COMBINATION_UNSUPPORTED。我第一次跑的时候少写了一个，找了半天原因。

**随时查看进度：**

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
&quot;```完成 90% 以上就可以进下一步了。剩下几段没完成的不影响，合并的时候会自动跳过。

4.2 下载并合并成最终视频
```

Bash

```
echo &quot;⏳ 正在下载所有视频片段...&quot;

cat &gt; /tmp/download_and_merge.py &lt;&lt; &#x27;PYEOF&#x27;
import json, subprocess, os, sys

PROJECT_ID = sys.argv[1]
EPISODE_ID = sys.argv[2]

# 获取所有分镜数据
d = json.loads(subprocess.check_output([
    &quot;curl&quot;, &quot;-s&quot;, &quot;-b&quot;, &quot;/tmp/auth_cookies.txt&quot;,
    f&quot;http://localhost:13000/api/novel-promotion/{PROJECT_ID}/episodes/{EPISODE_ID}&quot;
]).decode())

# 收集有视频的 panel
panels = []
for sb in d.get(&quot;episode&quot;, {}).get(&quot;storyboards&quot;, []):
    for p in sb.get(&quot;panels&quot;, []):
        if p.get(&quot;videoUrl&quot;):
            panels.append(p)

os.makedirs(&quot;/tmp/panels&quot;, exist_ok=True)
lines = []
skipped = 0

for i, p in enumerate(panels):
    url = &quot;http://localhost:13000&quot; + p[&quot;videoUrl&quot;]
    fname = f&quot;/tmp/panels/{i:03d}.mp4&quot;
    subprocess.run([&quot;curl&quot;, &quot;-s&quot;, &quot;-b&quot;, &quot;/tmp/auth_cookies.txt&quot;, url, &quot;-o&quot;, fname],
                   capture_output=True)
    size = os.path.getsize(fname) if os.path.exists(fname) else 0
    if size &gt; 1000:
        lines.append(f&quot;file &#x27;{fname}&#x27;&quot;)
        print(f&quot;  [{i+1}/{len(panels)}] ✅ 下载完成 ({size//1024}KB)&quot;)
    else:
        skipped += 1
        print(f&quot;  [{i+1}/{len(panels)}] ⚠️ 跳过（文件太小，可能还没生成完）&quot;)

# 写入 ffmpeg 合并列表
with open(&quot;/tmp/filelist.txt&quot;, &quot;w&quot;) as f:
    f.write(&quot;\n&quot;.join(lines))

print(f&quot;\n共下载 {len(lines)} 段视频&quot; + (f&quot;，跳过 {skipped} 段&quot; if skipped else &quot;&quot;))
PYEOF

python3 /tmp/download_and_merge.py $PROJECT_ID $EPISODE_ID
```text
# 合并成一个完整视频
echo &quot;⏳ 正在合并视频...&quot;
ffmpeg -f concat -safe 0 -i /tmp/filelist.txt -c copy /tmp/final_video.mp4 -y 2&gt;/dev/null

FILE_SIZE=$(du -h /tmp/final_video.mp4 | cut -f1)
echo &quot;✅ 视频合并完成！文件大小: $FILE_SIZE&quot;
```

4.3 下载到你的电脑

**方式一：浏览器下载**

```
Bash

```text
cp /tmp/final_video.mp4 /opt/waoowaoo/data/uploads/ 2&gt;/dev/null || \
  docker cp /tmp/final_video.mp4 waoowaoo-minio:/data/uploads/final_video.mp4

echo &quot;✅ 用浏览器打开以下链接下载视频：&quot;
echo &quot;http://你的服务器IP:13000/api/files/final_video.mp4&quot;
```

把"你的服务器 IP"换成实际的 IP。

方式二：scp 直接传到 Mac

在你 Mac 的终端里（不是服务器的）跑：

Bash

```
scp root@你的服务器IP:/tmp/final_video.mp4 ~/Downloads/
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

# 重新配（把 Key 换成你的）
curl -s -b /tmp/auth_cookies.txt \
  -X PUT http://localhost:13000/api/user/api-config \
  -H &quot;Content-Type: application/json&quot; \
  -d &#x27;{&quot;providers&quot;: [{&quot;id&quot;: &quot;ark&quot;, &quot;name&quot;: &quot;火山引擎 Ark&quot;, &quot;apiKey&quot;: &quot;你的新Key&quot;}]}&#x27;
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
# 重新加载之前保存的
source /tmp/waoowaoo_session.env
echo &quot;PROJECT_ID=$PROJECT_ID&quot;
echo &quot;EPISODE_ID=$EPISODE_ID&quot;

# 文件也丢了的话，查 API
curl -s -b /tmp/auth_cookies.txt http://localhost:13000/api/projects | \
  python3 -c &quot;import json,sys; [print(p[&#x27;projectId&#x27;], p[&#x27;name&#x27;]) for p in json.load(sys.stdin)[&#x27;projects&#x27;]]&quot;
```

**附录三：怎么让配音更像真人？**

教程里用的edge-tts是微软的免费合成语音。质量还行，但你一听就知道是机器人。

升级方法很简单：

1.  用手机录一段 5-10 秒的音频，说一句完整的话（比如"今天天气真不错，我们一起去散步吧"）

1.  保存成 MP3，传到服务器/tmp/目录

1.  上传到 waoowaoo 存储：

Bash

```
docker cp /tmp/你的音频.mp3 waoowaoo-minio:/data/uploads/
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

接下来我们需要安装两个 Skills：

**brainstorming：**

帮我们进行头脑风暴，扩展思路。

doc-coauthoring：

帮我们一起撰写和修改文档。

**⚠️ 注意：**

运行以下命令前，请确保你的电脑已经安装了 Node.js（如果未安装，请先查看附录/前置准备教程）。确认无误后，请在终端中依次复制粘贴以下两行代码，每粘贴一行按一次回车执行：

Plain Text

```
npx skills add obra/superpowers
npx skills add anthropics/skills
```

执行 npx skills add **指令安装 skills 的过程**，可以参考1.2 怎么安装 skills部分**。**

让我们先把 brainstorming 装了。

![](img/bd4c8599e05524a3c07973e4e5aa0032.png)

再把 doc-coauthoring 装了。

![](img/33587c9bdee460e920a290962a1ebaa6.png)

当你在终端看到绿色的Done!提示时，说明安装已经全部完成。

![](img/648ab45b1b3b13d3811085fa2e7fbad6.png)

接下来，在终端闪烁的光标处输入代码gemini并按下回车键，启动 gemini-cli。

![](img/1c959684d3bce81d3f0aac8ff6f5687d.png)

成功启动后（你会看到一个巨大的 GEMINI 字母图案）。

![](img/cc32d778d0137080f94831306cdc84b4.png)

我们在输入框中键入/skills list并回车。

![](img/f575c2869798e2cb170c0c76e7b70d09.png)

如果在弹出的列表中看到了brainstorming和doc-coauthoring，恭喜你，准备工作大功告成！

![](img/a9bf0495d09f015c9caef24a862c1faa.png)

完整截图如下：

![](img/4715ce0923d0c8b3a45254b501c56844.png)

哦哦哦哦哦哦哦哦哦！

![](img/7cf0a55040378c6675bdd152fda6362c.png)

好的，它启动了 skill。让我们来一场酣畅淋漓的头脑风暴吧！芜湖！

第一步：输入项目背景提示词进行头脑风暴

先把下面这个提示词给输了，回车。

Plain Text

```
我正在做一个关于飞书多维表格行家俱乐部的club网站，这个网站用于邀请专家进入行家俱乐部，挂行家的模板，博客，名人墙，还提供b端宣传，让大家可以在club网站找到想对接的maker帮自己交付应用。请和我一起头脑风暴一下，这个网站的mvp版本做什么比较合适
```

![](img/4ae5623c12c09f7c2f7dd197e62ff40e.png)

**第二步：授权 brainstorming 和 **doc-coauthoring 技能运行

执行时，gemini-cli 会弹出安全提示，我们直接 Allow for this session 就行，这样在整个项目下都可以用这个 skill。

![](img/bf4f9c044a794fa7308478e04666d5da.png)

然后它会问我们很多问题，我们就正常使用大白话在终端里回答它提出的问题，就和你平常用 coding cli 一样。经过几轮简单的问答交流后，会有一个简易的初稿，如下。

![](img/2a24d1e7c0ac4921507e4616e75d13a4.png)

然后我们基于这个初稿，使用 doc-coauthoring 进行精修。

（Tips：一般如果在[AGENTS.md](http://AGENTS.md)约束了它的使用流程，它不会直接出 mvp plan，而是进入 doc-coauthoring skill 进一步优化，本次没有约束所以 brainstorm 自闭环了）

![](img/695113141ba5fb81bad4c50a1c8ae49b.png)

然后我们基于 doc-coauthoring 继续进行问答。

![](img/8dfd2da3d550735db2e08af0143db3c3.png)

继续。

![](img/9647680513ace6791968d4cc1e4b87c7.png)

Project overview 看看。

![](img/c2af4c50454a361cda663b9b00de611b.png)

很不错，再看看第二章节。

![](img/327263be4d3610cdbb2791a63a0cf0fa.png)

嗯！对味！再看看第三章节。

![](img/9200b2993b118074d3516a1c7e929833.png)

没问题！继续！

![](img/0673ba04e0168939b1995ce8764ba38a.png)

继续！

![](img/beeaadddfdb3ea2b0e687fa54b8d0db4.png)

很好！

![](img/3036fe32efa65d890ef18c90c2bcab35.png)

好了，到最后一步了。

![](img/b28adf48d2c4225945ea37eedb4983df.png)

好了，到此为止，第一步就全部结束了，把我们宝贵的 7kb requirements 复制出来，我们待会在步骤二用。在接下来的步骤二里，我们将让 AI 根据这份“设计图纸”直接帮我们生成前端代码原型。

![](img/c2370bef05706598338c304293611e30.png)

步骤二：从 PRD 到原型（stitch + web-design-guidelines + doc-coauthoring）

让我们进入步骤二。在步骤二里，我们需要用到三个东西。

**stitch**

：Google 出品的前端代码生成利器，专精于把想法变成漂亮的 UI 界面。官网：https://stitch.withgoogle.com/

web-design-guidelines

：网页设计规范，告诉 AI 应该遵循什么样的审美和排版标准。

**doc-coauthoring**

：文档协作技能，帮我们更好地读取和利用刚才生成的 PRD 文档。

让我们开始吧。

**第一步：准备设计文件夹**

回到你项目的根目录，新建一个名为design**的文件夹，**并将我们刚才在步骤一生成的mvp-requirements.md文件复制并粘贴到这个design文件夹中。

![](img/362afee6ea7873596885d05430de92eb.png)

打开 vscode，进入 design 文件夹。

![](img/50213d878f07b67ff30fe395a6d4b00b.png)

确认文件夹内已放入刚才的需求文档。

![](img/61c13e1443618b202e68240003d951c5.png)

**第二步：安装 Skills**

需求文档已经进入 design 文件夹后，我们来安装 skills，现在我们要安装的是 web-design-guidelines 和 doc-coauthoring。

参考步骤一，把这两个 skill 安装一下。

Plain Text

```
npx skills add https://github.com/vercel-labs/agent-skills --skill web-design-guidelines
npx skills add https://github.com/anthropics/skills --skill doc-coauthoring
```

安装过程如下，基本一路按回车就行。

![](img/531defe1478a05f6f063c2e15d24cc67.png)

![](img/d82b576e5c1c1a1972078faa7463f64c.png)

好，启动 claudecode。在终端输入claude回车，进入 claude。

在对话框里输入/skills，回车，检查一下 skills 是否已经可用。如果内容如下图所示，则表示 skills 安装已经成功了。

![](img/5503b73ffffd5d7a8db10a0cabe672ee.png)

**第三步：讨论原型设计**

接着，我们开始讨论原型设计。记得艾特你之前写的 requirements 填充到上下文里。

Plain Text

```
根据 @larkbase-club-mvp-requirements.md 帮我整理一下，我们总共有多少个页面，需要怎么设计。
```

回车。然后 claude 就开始回答我们了。

![](img/82aa6b5d54ca410cbc3bbd6746ba9646.png)

接着，让我们一个一个页面开始讨论。讨论时，你可以要求 claude 按照 ASCII 码给你出原型设计图。比如：

Plain Text

```
请根据你的理解使用ASCII码生成原型的布局，我们来进行讨论。
```

第一个页面看着不错。

![](img/f11990086351d51add2c972a3666abf4.png)

注意这个地方有问题就改，因为非常节省 token，所以你可以让他改很久，比如按钮的位置、文案、组件的大小布局等都可以在这里定下来。

经过一顿处理后，我们就拿到了 3 个 page 的完整版。

![](img/91a8f452c2c80195682e75aa72052301.png)

![](img/6b8c08eef03e53e59bac608fc5b0919a.png)

![](img/a7606277c42a140eb27041c9c5ac1c69.png)

让 claude 把所有 ascII 码和相关要求都导出成一个 markdown 文档。比如我的是这个：

Markdown

```

# Lark Base Club - Homepage (Page 1) 原型设计 ## ASCII 原型图 ``` ╔══════════════════════════════════════════════════════════════════════════════╗ ║ 🔍 Lark Base Club [Square] [Join] [🌙 Light/Dark] 📱 Mobile ║ ╠══════════════════════════════════════════════════════════════════════════════╣ ║ ║ ║ ┌─────────────────────────────────────┐ ║ ║ │ │ ║ ║ │ HERO SECTION │ ║ ║ │ │ ║ ║ │ ┌─────────────────────────┐ │ ║ ║ │ │ │ │ ║ ║ │ │ &quot;连接飞书多维表格专家 │ │ ║ ║ │ │ 与企业需求的平台&quot; │ │ ║ ║ │ │ │ │ ║ ║ │ └─────────────────────────┘ │ ║ ║ │ │ ║ ║ │ &quot;找专家？展示作品？获取客户？ │ ║ ║ │ 这里是飞书多维表格极客的家园&quot; │ ║ ║ │ │ ║ ║ │ [ 🚀 浏览行家广场 ] │ ║ ║ │ │ ║ ║ └─────────────────────────────────────┘ ║ ║ ║ ╠══════════════════════════════════════════════════════════════════════════════╣ ║ ║ ║ ┌────────────────────────────────────────────────────────────────────┐ ║ ║ │ │ ║ ║ │ INTRODUCTION - &quot;什么是 Lark Base Club?&quot; │ ║ ║ │ │ ║ ║ │ ┌─────────────────────┐ ┌─────────────────────┐ │ ║ ║ │ │ │ │ │ │ ║ ║ │ │ 👔 B端老板 │ │ 🛠️ Maker 专家 │ │ ║ ║ │ │ │ │ │ │ ║ ║ │ │ &quot;需要SRM/HR系统？ │ │ &quot;擅长飞书多维表格？ │ │ ║ ║ │ │ 不想从零开发？&quot; │ │ 想展示你的技能？&quot; │ │ ║ ║ │ │ │ │ │ │ ║ ║ │ │ ✓ 浏览专家 │ │ ✓ 展示作品集 │ │ ║ ║ │ │ ✓ 找到现成模板 │ │ ✓ 获取客户线索 │ │ ║ ║ │ │ ✓ 一键预约咨询 │ │ ✓ 加入极客社区 │ │ ║ ║ │ │ │ │ │ │ ║ ║ │ └─────────────────────┘ └─────────────────────┘ │ ║ ║ │ │ ║ ║ └────────────────────────────────────────────────────────────────────┘ ║ ║ ║ ╠══════════════════════════════════════════════════════════════════════════════╣ ║ ║ ║ ┌────────────────────────────────────────────────────────────────────┐ ║ ║ │ │ ║ ║ │ FEATURED EXPERTS - 精选行家 │ ║ ║ │ │ ║ ║ │ ┌─────────┐ ┌─────────┐ ┌─────────┐ ┌─────────┐ │ ║ ║ │ │ [IMG] │ │ [IMG] │ │ [IMG] │ │ [IMG] │ │ ║ ║ │ │ │ │ │ │ │ │ │ │ ║ ║ │ │ 张三 │ │ 李四 │ │ 王五 │ │ 赵六 │ │ ║ ║ │ │ 顾问 │ │ 开发 │ │ 架构师 │ │ 产品经理 │ │ ║ ║ │ │ │ │ │ │ │ │ │ │ ║ ║ │ │ #CRM │ │ #HR系统 │ │ #SRM │ │ #财务 │ │ ║ ║ │ │ #零售 │ │ #制造 │ │ #供应链 │ │ #发票 │ │ ║ ║ │ │ │ │ │ │ │ │ │ │ ║ ║ │ │ [→] │ │ [→] │ │ [→] │ │ [→] │ │ ║ ║ │ └─────────┘ └─────────┘ └─────────┘ └─────────┘ │ ║ ║ │ │ ║ ║ │ ┌─────────┐ ┌─────────┐ │ ║ ║ │ │ [IMG] │ │ [IMG] │ │ ║ ║ │ │ │ │ │ │ ║ ║ │ │ 钱七 │ │ 孙八 │ │ ║ ║ │ │ ... │ │ ... │ │ ║ ║ │ │ │ │ │ │ ║ ║ │ │ #... │ │ #... │ │ ║ ║ │ │ │ │ │ │ ║ ║ │ │ [→] │ │ [→] │ │ ║ ║ │ └─────────┘ └─────────┘ │ ║ ║ │ │ ║ ║ │ [ 查看所有行家 → ] │ ║ ║ │ │ ║ ║ └────────────────────────────────────────────────────────────────────┘ ║ ║ ║ ╠══════════════════════════════════════════════════════════════════════════════╣ ║ ║ ║ © 2025 Lark Base Club | Powered by Feishu ║ ║ ║ ╚══════════════════════════════════════════════════════════════════════════════╝ ``` --- ## 布局说明 ### 1. **Header (全局导航)** - **位置**: 固定在顶部 - **左侧**: Logo + 站点名称 - **中间**: 导航链接 (Square广场, Join加入) - **右侧**: 主题切换器 (🌙/☀️) - **响应式**: 移动端折叠为汉堡菜单 --- ### 2. **Hero Section** - **对齐**: 居中对齐 - **内容**: - 大标题: &quot;连接飞书多维表格专家与企业需求的平台&quot; - 副标题: &quot;找专家？展示作品？获取客户？这里是飞书多维表格极客的家园&quot; - CTA 按钮: &quot;🚀 浏览行家广场&quot; (跳转到 `/square` 页面) - **样式**: 大字号、粗体、飞书蓝色强调 --- ### 3. **Introduction (双栏布局)** - **布局**: 左右两栏，分别面向两类用户 - **左栏 - B端老板**: - 标题: &quot;👔 B端老板&quot; - 痛点问题: &quot;需要SRM/HR系统？不想从零开发？&quot; - 核心利益点: - ✓ 浏览专家 - ✓ 找到现成模板 - ✓ 一键预约咨询 - **右栏 - Maker专家**: - 标题: &quot;🛠️ Maker 专家&quot; - 痛点问题: &quot;擅长飞书多维表格？想展示你的技能？&quot; - 核心利益点: - ✓ 展示作品集 - ✓ 获取客户线索 - ✓ 加入极客社区 --- ### 4. **Featured Experts (网格布局)** - **数据来源**: 从 Lark Base 获取 `is_featured=true` 的行家数据 - **展示数量**: 4-6 位精选行家 - **响应式网格**: - 桌面端 (≥1024px): 4 列 - 平板端 (768px-1023px): 2 列 - 移动端 (&lt;768px): 1 列 - **卡片内容**: - 头像 (圆形/圆角方形) - 姓名 - 职位/头衔 - 标签 (2-3个，徽章样式) - 查看详情按钮 (→) - **底部**: &quot;查看所有行家 →&quot; 按钮，跳转到 `/square` 页面 --- ### 5. **Footer** - **内容**: - 版权信息: &quot;© 2025 Lark Base Club&quot; - 技术支持: &quot;Powered by Feishu&quot; - **样式**: 简洁、居中对齐、灰色文字 --- ## 技术实现要点 ### 响应式断点 - **Mobile**: &lt; 768px - **Tablet**: 768px - 1023px - **Desktop**: ≥ 1024px ### 数据获取 - **Server Component**: 使用 Next.js App Router - **数据源**: Lark Base Bitable API - **缓存策略**: ISR, `revalidate: 60` 秒 ### SEO 优化 - **Meta Title**: &quot;Lark Base Club - 连接飞书多维表格专家与企业需求&quot; - **Meta Description**: &quot;找专家？展示作品？获取客户？这里是飞书多维表格极客的家园&quot; - **Keywords**: 多维表格, 飞书Base, 行家, 极客社区
```

第四步：使用 stitch 生成 UI

然后我们登录 stitch。接着直接把整个 page 的内容扔给 stitch，回车。

![](img/e386288da299cdce3dcf5ae8728af1f5.png)

然后我们在 stitch 里继续口喷需求，一段时间之后，我们就得到了下面的设计稿。

![](img/7bd6e8a6138c31cc481f4875be3fd51c.png)

大概长下面这样。

![](img/d00ea00a5c7ecdc65b4a20c7da3f5315.png)

![](img/03ac0b82ce9c9b6d9eb1a2e645a0d343.png)

![](img/90e6cd968326570ad512f296628341c3.png)

可以了，下载下来。

**第六步：下载下来**

点击左上角的 download project，浏览器就会自动下载一个 zip 压缩包，里面包含了所有设计稿的 html 文件和图片。同样的，把它解压后复制粘贴到你的 design 文件夹下面。

![](img/8b1d6edbee8e0cf22380f8560d035e51.png)

第七步：使用 doc-coauthoring 完善最终版 PRD

UI 做完了我们可以来写 PRD 了。还是一样，我们使用 gemini-cli 来完成内容撰写。输入提示词如下：

Plain Text

```
来看一下 stitch_larkbase_club_homepage文件夹里的设计稿，以及 @larkbase-club-mvp-requirements.md ，整理一下交互，用 doc-coauthoring 和我一起把 prd 写出来
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
### 02.构建电商视频策划 Skill

1.项目灵感与设计哲学

1.1 灵感来源

**问题场景**

在电商行业，制作一个高质量的带货视频策划案通常需要：

• **视觉分析师**：分析产品外观、材质、设计

• **市场研究员**：调研竞品、用户痛点、行业趋势

• **卖点策划师**：提炼差异化的营销卖点

• **视频导演**：撰写分镜脚本、设计拍摄方案

这些角色需要密切配合，信息层层传递，才能产出一份可落地的策划案。

**核心洞察**

**Claude Code 的多 Agent 协作能力，恰好可以模拟这种&quot;团队协作&quot;的工作模式**

：Plain Text

```text
一个主控Agent（总监）统筹调度
↓多个子Agent（专家）各司其职
↓输出标准化文档
↓整合成最终成果
```

**设计理念**

这套系统的设计遵循以下原则：

1.  **角色分工明确**：每个 Agent 有清晰的能力边界

1.  **流程标准化**：每个步骤有明确的输入/输出规范

1.  **质量可校验**：每一步都有检查清单

1.  **结果可落地**：最终输出可以直接执行

1.2 系统架构总览

Plain Text

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

**核心概念解释**

| 概念 | 作用 | 类比 |
| --- | --- | --- |
| CLAUDE.md | 项目级主控 Agent | 公司的 CEO/总监 |
| agents/*.md | 子 Agent 定义 | 各部门负责人 |
| skills/*/ SKILL.md | 用户可调用的技能 | 对外服务窗口 |
| references/skills/*.md | 工具型参考文件 | 执行工具手册 |

这个是这个Skill的项目文件：

[

![](img/146fd4fc573a21232d7b02f6d31268dd.png)

电商.zip](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/KEcebvnjcoueSExvy1Acq0lonIf?response-content-disposition=attachment%3B%20filename%3D%22%E7%94%B5%E5%95%86.zip%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260526%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260526T144427Z&x-oss-expires=86400&x-oss-signature=1d2fbb3ff9d544842355b446df81e3a0d60b3a225f079c628d8f7cbe4c9975b2&x-oss-signature-version=OSS4-HMAC-SHA256)

2.为什么这样设计

2.1 为什么要分主控 Agent 和子 Agent？

**设计考量**

如果只用一个 Agent 处理所有事情

：•Prompt 会非常长，容易遗漏细节

• 角色混乱，既要做分析又要做创意

• 质量难以保证，没有专业深度

**分层设计的好处**

：•每个子 Agent 专注一个领域，Prompt 更精准

• 模拟真实团队协作，逻辑更清晰

• 可以单独调试每个环节

**类比理解**

Plain Text

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

2.2 为什么要设计 Skill 工具参考文件？

**设计考量**

子 Agent 需要调用"工具"来执行具体任务，比如：

• 分析图片 → 需要图片分析工具

• 搜索信息 → 需要搜索工具

• 生成脚本 → 需要脚本生成工具

**工具型 Skill 的特点**

在references/skills/下的工具定义有共同特点：

1.  **纯功能执行**：明确声明"无任何自主决策能力"

1.  **标准化输入输出**：严格定义 JSON/Markdown 格式

1.  **单一职责**：每个工具只做一件事

**为什么要这样设计？**

Plain Text

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

2.3 为什么要设计质量校验机制？

**质量校验的设计**

在[CLAUDE.md](http://CLAUDE.md)中，每个步骤都有**质量校验清单**：

Markdown

```
质量校验：
- [ ] 是否识别出产品品类
- [ ] 是否提取了3个以上视觉卖点
- [ ] 是否提供了搜索关键词建议
- [ ] 报告格式是否完整
```

**为什么需要这个？**

1.  **AI 输出不稳定**：同样的输入可能产生不同质量的结果

1.  **保证流程可靠**：不合格的输出会影响后续环节

1.  **模拟真实工作流**：总监需要审核下属的工作

**校验后的处理**

Markdown

```
不合格处理：驳回并要求重新分析，说明具体问题。
```

这模拟了真实工作中"返工"的场景。

2.4 为什么输出要标准化？

**标准化的输出格式**

每个子 Agent 都有明确的输出模板：

Markdown

```
产品视觉特征报告

 基础信息
- 产品品类：[品类]
- 核心材质：[材质列表]

 视觉卖点分析
 卖点1：[卖点名称]
...
```

**为什么需要标准化？**

1.  **便于传递**：下一个 Agent 需要解析上一个 Agent 的输出

1.  **便于整合**：最终策划案需要汇总所有信息

1.  **便于用户理解**：统一的格式更专业

3.从零开始搭建

3.1 环境准备

**创建项目目录**

Bash

```
mkdir ecommerce-video-planner
cd ecommerce-video-planner
mkdir -p .claude/agents
mkdir -p .claude/skills/ecommerce-video-planner/references/skills
mkdir output
```

**目录结构预览**

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

3.2 创建主控 Agent（CLAUDE.md）

**文件位置**

Plain Text

```
.claude/CLAUDE.md
```

**设计思路**

主控 Agent 是整个系统的大脑，需要定义：

1.  **人设定位**：赋予专业身份

1.  **核心目标**：明确任务

1.  **工作流程**：步骤化执行

1.  **校验标准**：质量控制

1.  **异常处理**：容错机制

**核心代码框架**

Markdown

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

**关键设计点**

**（1） 人设定位的重要性**

Markdown

```
人设定位

你是顶级电商代运营公司的视频策划总监，操盘过100+电商爆款单品，精通抖音、淘宝、小红书等全平台电商流量逻辑...
```

**为什么这样写？**

• 赋予 AI 专业身份，引导其用专业视角思考

• "操盘过 100+爆款"暗示丰富的经验

• 明确能力范围（电商视频策划）

**（2） 工作流程的步骤化**

Markdown

```
步骤2：调度产品视觉分析师

下发任务：
```

@visual-analyst-agent请分析以下产品图片，输出《产品视觉特征报告》。

Plain Text

```
接收输出：《产品视觉特征报告》

质量校验：
- [ ] 是否识别出产品品类
- [ ] 是否提取了3个以上视觉卖点
```

**为什么这样写？**

• 明确每个步骤的输入和输出

• 定义质量标准，便于校验

• 便于调试和优化单个环节

**（3） 异常处理机制**

Markdown

```
异常处理

 图片无法识别
 搜索结果不足
 子Agent输出不合格
```

**为什么需要这个？**

• AI 不是万能的，需要容错机制

• 给用户提供明确的下一步建议

• 提升系统的鲁棒性

3.3 创建子 Agent

3.3.1 产品视觉分析师

**文件位置**

：.claude/agents/visual-analyst-agent.md

**设计思路**

：•定义专业背景（8 年经验）

• 明确能力边界（只分析视觉，不做市场调研）

• 定义输出格式

Markdown

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

3.3.2 电商情报研究员

**文件位置**

：.claude/agents/market-researcher-agent.md

**核心职责**

：•接收产品视觉特征报告

• 调用搜索工具调研市场

• 整合竞品信息、用户痛点、行业趋势

**关键设计**

：Markdown

```
专属工具箱
- skill_2_keyword_searcher：电商关键词搜索器
- skill_3_data_integrator：电商数据整合器
```

**为什么需要两个工具？**

• 搜索器：负责获取原始数据

• 整合器：负责提炼关键信息

• 分工明确，输出更可控

3.3.3 卖点策划经理

**文件位置**

：.claude/agents/selling-point-manager-agent.md

**核心职责**

：•结合视觉特征和市场情报

• 提炼分层卖点（核心/差异化/情感化）

**关键设计 - 分层卖点体系**

：Markdown

```
卖点分层设计

 核心卖点（1个）
最强的功能/价值主张

 差异化卖点（2个）
与竞品形成区隔的独特优势

 情感化卖点（1个）
击中用户心理需求，创造情感共鸣
```

**为什么分层？**

• 30 秒视频无法展示所有卖点

• 核心卖点作为主打

• 差异化建立竞争优势

• 情感化触发购买冲动

3.3.4 视频脚本导演

**文件位置**

：.claude/agents/script-director-agent.md

**核心职责**

：•基于卖点清单设计视频类型

• 撰写分镜头脚本

• 输出拍摄执行清单

**关键设计 - 30 秒视频结构**

：Markdown

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

**为什么是 30 秒？**

• 抖音等短视频平台的最佳时长

• 完播率高，算法推荐更友好

• 信息密度适中，不会造成认知负担

3.4 创建 Skill 入口文件

**文件位置**

：.claude/skills/ecom[merce-vi](http://SKILL.md)deo-planner/SKILL.md

**YAML 头部定义**

YAML

```
---name: ecommerce-video-planner
description: 电商视频全案策划系统。用户上传产品图片后，自动完成「产品视觉解析→市场情报调研→核心卖点提炼→短视频脚本全案输出」全流程...
---
```

description 的作用：

• Claude Code 根据这个描述判断何时触发此 Skill

• 需要包含关键词和触发场景

**系统架构展示**

Markdown

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

**为什么展示架构图？**

• 帮助用户理解系统工作原理

• 建立信任感

• 明确预期输出

3.5 创建工具型 Skill 参考文件

**设计原则**

所有工具型 Skill 都有共同结构：

Markdown

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

**为什么声明无自主决策能力？**

Plain Text

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

**工具 1：图片视觉特征提取器**

**文件**

：skill_1_image_[analyzer.md](http://analyzer.md)

**输入**

：产品图片**输出**：JSON 格式的视觉特征

JSON

```
{&quot;category&quot;: &quot;产品品类&quot;,
  &quot;core_materials&quot;: [&quot;材质1&quot;, &quot;材质2&quot;],
  &quot;color_style&quot;: &quot;颜色+风格&quot;,
  &quot;visual_selling_points&quot;: [&quot;卖点1&quot;, &quot;卖点2&quot;, &quot;卖点3&quot;],
  &quot;usage_scenarios&quot;: [&quot;场景1&quot;, &quot;场景2&quot;],
  &quot;suggest_search_keywords&quot;: [&quot;关键词1&quot;, &quot;关键词2&quot;]
}
```

**为什么用 JSON？**

• 结构化数据，便于后续 Agent 解析

• 字段明确，不会遗漏信息

**工具 2：电商关键词搜索器**

**文件**

[：skill_2_ke](http://searcher.md)yword_searcher.md

**核心设计**

：三维搜索

Markdown

```
1. 竞品卖点搜索：搜索&quot;[关键词] + 卖点/特点/优势&quot;
2. 用户痛点搜索：搜索&quot;[关键词] + 痛点/问题/差评&quot;
3. 行业趋势搜索：搜索&quot;[关键词] + 趋势/新品/2024&quot;
```

**为什么要分三个维度？**

• 全面覆盖市场信息

• 不同维度的信息服务于不同目的

• 便于后续整合分析

**工具 3：电商数据整合器**

**文件**

：skill_3_data_[integrator.md](http://integrator.md)

**职责**

：将原始搜索结果提炼为 TOP3 清单

Markdown

```
输出结构

 1. 核心竞品卖点TOP3
| 排名 | 卖点描述 | 信息来源备注 |

 2. 用户高频痛点TOP3
| 排名 | 痛点描述 | 典型用户反馈 |

 3. 行业热门趋势
```

**为什么要提炼 TOP3？**

• 信息过载不利于决策

• 聚焦最重要的信息

• 30 秒视频也容纳不了太多卖点

**工具 4：分层卖点生成器**

**文件**

[：skill_4_sel](http://generator.md)ling_point_generator.md

**核心设计**

：卖点必须有支撑依据

Markdown

```
| 卖点层级 | 卖点内容 | 支撑依据 |
|----------|----------|----------|
| 核心卖点 | [内容] | 图片特征：xxx；市场数据：xxx |
```

**为什么要求支撑依据？**

• 避免编造卖点

• 确保卖点有事实基础

• 便于追溯和验证

**工具 5：分镜头脚本撰写器**

**文件**

[：skill_5_](http://writer.md)script_writer.md

**核心设计**

：平台适配

Markdown

```
平台规则参考

- 抖音：前3秒必须有强钩子，30秒内
- 淘宝：45-60秒，重点展示细节
- 小红书：注重真实感和种草感
```

**为什么要区分平台？**

• 不同平台的流量逻辑不同

• 用户期待不同

• 审核规则不同

• 3.6 搭建流程总结

**步骤回顾**

Plain Text

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

Plain Text

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

4.输出结果示例

4.1 最终输出物

系统运行完成后，会在output/目录生成：

Plain Text

```
output/
└── 电商视频策划案_20240315_1430.md
```

4.2 策划案结构示例

Markdown

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

5.使用手册

**5.1 快速开始**

**安装 Claude Code**

Bash

```
如果尚未安装Claude Code CLI
npm install -g @anthropic/claude-code
```

**进入项目目录**

Bash

```
cd ecommerce-video-planner
```

**启动 Claude Code**

Bash

```
claude
```

**触发 Skill**

在 Claude Code 对话中输入：

Plain Text

```
帮我策划一个电商视频
```

或直接上传产品图片并说：

Plain Text

```
这是我的一款产品，帮我做个抖音带货视频策划
```

5.2 输入要求

**必填项**

| 项目 | 说明 |
| --- | --- |
| 产品图片 | 清晰展示产品的图片，支持 JPG/PNG |

**可选项**

| 项目 | 说明 | 示例 |
| --- | --- | --- |
| 产品品类 | 如果 AI 识别不准，可手动指定 | &quot;这是一个智能保温杯&quot; |
| 目标平台 | 指定视频投放平台 | &quot;目标平台是抖音&quot; |
| 目标人群 | 指定目标用户群体 | &quot;主要面向白领女性&quot; |
| 特殊要求 | 其他定制需求 | &quot;要突出性价比&quot; |

![](img/8578043ca393de1f2b70a5831e09255f.png)

5.3 使用示例

**示例 1：基础使用**

**用户输入**

：Plain Text

```
[上传产品图片]
帮我策划这个保温杯的抖音带货视频
```

**系统响应**

：Plain Text

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

**示例 2：带补充信息**

**用户输入**

：Plain Text

```
[上传产品图片]
这是一款新出的护肤精华，主要成分是玻尿酸
目标平台：小红书
目标人群：25-35岁都市女性
```

**系统响应**

：Plain Text

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

**用户输入**

：Plain Text

```
[上传产品图片]
这个产品要在淘宝和抖音同时推，帮我分别策划视频
```

**系统响应**

：Plain Text

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

5.4 输出文件说明

**文件位置**

Plain Text

```
output/电商视频策划案_YYYYMMDD_HHMM.md
```

![](img/c8ef53720ffba280d37c8de272242c02.png)

**文件内容**

策划案包含以下部分：

| 章节 | 内容 | 用途 |
| --- | --- | --- |
| 产品视觉分析摘要 | 产品外观、材质、风格 | 了解产品基础信息 |
| 市场情报摘要 | 竞品、痛点、趋势 | 了解市场环境 |
| 核心卖点策略 | 4 个分层卖点 | 视频核心信息 |
| 视频执行方案 | 分镜脚本、标题标签 | 直接拍摄使用 |
| 执行建议 | 拍摄要点、避坑提醒 | 执行参考 |

![](img/d84292fdf213e61f381c6929de0aea5f.png)

5.5 常见问题

**Q1：图片识别不准确怎么办？**

**解决方案**

：•上传更清晰的产品图片

• 在输入中补充产品描述

• 指明产品品类

**Q2：搜索结果有限怎么办？**

**可能原因**

：•产品过于小众

• 关键词不够精准

**解决方案**

：•提供更多产品信息

• 指定竞品品牌帮助搜索

• 系统会基于有限信息继续策划

**Q3：如何修改生成的策划案？**

在 Claude Code 中继续对话：

Plain Text

```
把核心卖点改成突出&quot;便携性&quot;
```

Plain Text

```
把视频时长改成60秒
```

Plain Text

```
再给我几个标题备选
```

**Q4：支持哪些平台？**

| 平台 | 支持 | 视频特点 |
| --- | --- | --- |
| 抖音 | ✅ | 30 秒快节奏，强钩子 |
| 淘宝 | ✅ | 45-60 秒详细版 |
| 小红书 | ✅ | 真实种草感 |
| 快手 | 🔄 | 可适配抖音版 |
| 视频号 | 🔄 | 可适配抖音版 |

**Q5：如何调试单个环节？**

如果某个环节输出不理想，可以要求重新执行：

Plain Text

```
重新分析产品图片，我需要更多视觉卖点
```

Plain Text

```
市场调研太少了，帮我补充更多竞品信息
```

5.6 高级用法

**自定义卖点数量**

Plain Text

```
给我提炼5个卖点，视频时长60秒
```

**指定视频风格**

Plain Text

```
这个产品适合走科技感风格，帮我调整脚本
```

**多产品对比**

Plain Text

```
[上传多张产品图片]
帮我对比这三款产品，分别策划视频
```

**结合热点**

Plain Text

```
最近&quot;XX话题&quot;很火，帮我结合这个热点策划视频
```

5.7 最佳实践

**上传图片建议**

1.  **清晰度**：至少 1080P

1.  **角度**：多角度展示产品

1.  **光线**：自然光或专业布光

1.  **背景**：简洁干净的背景

**补充信息建议**

提供的信息越具体，策划案越精准：

Plain Text

```
[上传产品图片]
产品：便携式榨汁机
核心功能：30秒快速榨汁
目标人群：健身爱好者、上班族
核心卖点希望突出：便携+快充
竞品参考：XX品牌
```

**策划案使用建议**

1.  **拍摄前**：仔细阅读拍摄清单，准备道具

1.  **拍摄中**：按分镜脚本执行，注意拍摄要点

1.  **剪辑时**：参考节奏建议和 BGM 风格

1.  **发布时**：使用配套标题和标签

5.8附录：文件清单

**项目文件结构**

Plain Text

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

**文件用途速查**

| 文件 | 类型 | 用途 |
| --- | --- | --- |
| CLAUDE.md | 主控 | 定义整体工作流程 |
| *- agent.md | 子 Agent | 定义专业角色职责 |
| SKILL.md | 入口 | 定义触发条件和使用说明 |
| skill_*.md | 工具 | 定义标准化输入输出 |

**写在最后**

**恭喜你，当你成功安装了Claude code、Skills、 Open Claw，并且完成实战篇的第一个案例时 ，你已经进**入了AI编程的大门，但我相信，航海的结束不是学习结束，你可以继续在业务中运用这些 AI 工具，让你的AI编程之路越走越远

最后，让我们一起用好 AI，跟上 AI时代，一起生财有术！！！

![](img/60723d70ec2997b06a730b18390e0ea2.png)

```

```