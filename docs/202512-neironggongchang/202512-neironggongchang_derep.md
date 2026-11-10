# 内容工厂 Agent 202512：把选题、创作与发布交给 AI 流水线

> 源自：[https://my.feishu.cn/docx/Qzswdht0colCdixZUjacmuSQnUb](https://my.feishu.cn/docx/Qzswdht0colCdixZUjacmuSQnUb)  
> 同步地址：<https://my.feishu.cn/sync/Lj5sd8APisk896bxImEcYvjMnlF>

# 启航第一课：从零开始，搭出内容工厂Agent

## 新手怎么进入这个项目？

### 1.内容工厂Agent是什么

我是钱塘江鲤，欢迎上船。接下来的航程，我会带大家把内容工厂 Agent 完整做出来。技术方面，我们以 Next.js 作为开发框架，SQLite 负责数据存储，写码环节交给 Claude Code 或 Codex 这类 AI 编程工具，目标是打通内容工厂的核心链路。

项目整体拆成三大模块：内容采集与选题分析、内容创作、发布模块。

前半段我们会先理清 AI 编程的基础知识，之后再按章节推进开发。每一章都会配备对应的 Claude/Codex 提示词和完整对话记录，手册中也收录了本次航海用到的全部提示词，方便你理解“借助 AI 工具完整开发一个内容工厂”的全过程。

同时，为了让不同基础和不同行业的圈友都能有所收获，除提示词和视频教程外，我们还会在航海群中放出完整源代码，确保大家可以真正把项目搭起来、用起来。

开始之前，先看看本次航海的目标以及最终效果（视频学习）：

https://scys.com/view/docx/J4ETdEfOpo4P3kxAWQOcZJl7nWf#SeCtdQu49olrjsxNTnpc1vwYnje

我们要做的内容工厂 Agent，本质是一套高适应性的自动化基础框架，可以按需求自由拼接，适配不同内容生产场景。学完这次航海，你将获得：

**智能选题中心**——输入关键词，自动捕捉热点，生成有参考价值的选题分析报告。

**高效创作中心**——一键产出适配小红书、公众号等不同平台风格的内容。

**闭环分发链路**——小红书扫码即发，公众号自动推送草稿箱，完成一键发布。

### 2.项目完整操作思路

#### 2.1 项目完整操作思路

本次航海采用 AI 编程的方式构建内容工厂，核心思路很直接：通过自然语言和 Claude Code 等工具持续对话，把开发任务一步步推进。

工具安装并配置完成后，先与 AI 反复沟通，把需求说透，生成页面原型；接下来按“数据采集—选题分析—内容创作—发布管理”四个模块逐个实现。

每个模块都遵循同一个循环：描述需求 → AI 出方案 → 确认 → AI coding → 测试。出错时，直接把浏览器控制台的报错抛给 AI 修复。靠这种人机协作，产品可以在很短时间内完成从 0 到 1 的开发。

整个协作中，人负责产品方向与关键决策，AI 负责代码落地。

#### 2.2 操作重点

操作重点连成一条线就是：环境搭建与工具配置 → 构建选题采集与分析 agent → 开发 AI 内容二创与多平台适配功能 → 打通公众号与小红书官方发布接口与分发 → 系统集成与工作流优化。

#### 2.3 新手常见问题

+ **完全没有编程基础，学得会吗？**

学得会。这次航海的核心是用自然语言和 AI 对话，不要求传统手写代码。只要能把需求表达清楚，AI 就能理解并帮你实现。

+ **搭建中遇到报错或不懂的地方怎么办？**

报错是很正常的事情，不用太担心。我们会尽量提供稳定的流程；实际操作中遇到问题，可以向 AI 提问解决，也可以找教练求助。

+ **可以用别的 AI 工具吗？比如 Cursor、Trae 等**

AI 工具选择很多，但建议优先挑生产力最强的那一款。好工具能大幅提升效率、节省时间，所以还是推荐用 Claude Code/Codex 来跟进航海任务。

#### 2.4 开船前必备

+ 一台电脑，mac 最佳，Windows 也可以用
+ ChatGPT Plus / Claude 账号
+ 稳定的网络环境

# 必修篇

# 一、快速上手 AI 编程工具

## 01.理解 AI 辅助编程与传统编程的区别

### 0.本章概要

💡

本章概要

恭喜你，终于踏出内容工厂 Agent 的第一步。

这一章从零开始：弄清楚 AI 辅助编程是什么、它和传统编程的根本差异在哪里，再把开发环境装好，并激活 Claude Code 或 Codex 这类 AI 编程工具。

本章内容分成三大块：

**第一块：理解 AI 辅助编程的核心逻辑。**

我们会一起认识 AI 编程的原理，以及「人机协作」这种新模式。你会发现，未来编程的重点不是背语法，而是如何把需求描述清楚、引导 AI 找到更优方案。一旦掌握这种思维，生产力会进入另一个量级。

**第二块：准备开发环境与工具安装。**

这一阶段，我们会完成 VS Code 和 Node.js 的安装与配置，把本地运行环境搭起来。无论你用 Mac 还是 Windows，只要按步骤操作，就能顺畅进入 AI 编程的世界。

**第三块：激活并配置 AI 编程助手。**

学完本部分，你将完成 Claude Code 或 Codex 的安装、登录和配置；我们也会给出 GLM4.6 等国内模型的接入方式，让 AI 编程全流程可以顺利跑通。

完成这一章，你就正式进入了 AI 编程的世界，并拥有让 AI 写代码、调试程序、构建产品的基础能力。更重要的是，你会理解这种能力的核心思维——用语言创造，用想法驱动，用 AI 实现。

⚠️ 课前准备：需要稳定的科学网络环境，并拥有 Claude Code 或 Codex 账号（二选一）。

💡

**本章航线图**

完成本章的学习与实操，就可以通过第一阶段：

第一阶段：快速上手 AI 编程工具（约 3 天）

+ 理解 AI 辅助编程与传统编程的区别（约 0.5 天）
+ 准备开发环境并安装 Claude Code/Codex（约 2 天）
+ 激活并配置你的 Claude Code/Codex 账号（约 1 天）

### 1.AI 辅助编程是什么

Vibe Coding 在最近半年彻底火出了圈。今年 2 月初，OpenAI 联合创始人 Andrej Karpathy 在社交平台上提出这个概念，短短一个多月，就在开发者圈子里引发了不小的讨论。它能火起来并不意外——编程的门槛确实被大幅拉低了。

过去，想把一个想法变成能用的产品，总要有专业程序员去实现需求。但今天的规则已经改变。

即使对代码一窍不通，也能靠 AI 编程工具把想法快速落地。这种变化不是渐进式改良，而是颠覆性的重构。

在生财，我们已经见过太多鲜活的例子：不少圈友从没写过一行代码，却借助 Cursor、Claude Code 等工具做出了真实可用的应用。有人因此做出海外工具站，有人搭起了自动化工作流，还有人做出了能赚钱的小程序。

这已经不单是效率差距。会用与不会用 AI 编程，生产力可能差出十倍甚至百倍。一个懂得与 AI 协作的人，可以在一天内完成过去一个小团队一周的工作量。更关键的是，这种能力正在重塑“谁能创造价值”的定义：技术不再是壁垒，想法和执行才是。

你不必再把 80% 的精力花在写代码上，而能专注创意、产品设计、用户体验这些真正重要的事。代码实现交给 AI，你只需要想清楚“要做什么”和“为什么这么做”，AI 负责“怎么做”，时间精力都会被极大释放。

这次航海，就让我们一起感受 AI 编程的魅力，用 Claude Code/Codex 等工具，打造你自己的内容工厂 Agent。

![](img/601ee5e04792bbc35a4786103510b35c.png)

### 2.AI 辅助编程与传统编程的区别

把传统编程和 AI 辅助编程放在一起，会发现它们是两种完全不同的工作方式。

旧路线的开发者要先啃完厚厚的编程书，消化复杂的专业术语，再摆弄各种框架配置。学习周期以半年起步，时间成本相当高。很多人正是在这个阶段停了下来，不是不够聪明，而是这条路本身就太陡峭。

AI 时代相当于把规则重新写过。现在真正重要的能力，不再是记住编程语法，而是学会和 AI 对话：清晰描述你的要求，用最自然的语言告诉 AI 你想要的产出。AI 会生成代码，还会给出多种实现方向；你从中选出合适的那一个，然后继续对话，比如“这里的逻辑能不能调整一下”“能不能加个导出功能”。就这样一轮轮迭代，项目在人与 AI 的配合中慢慢成形。

两者的差异，可以从下面几个维度来看：

- **驱动方式**：传统开发由人手动写代码、定逻辑、定流程，一切都由开发者决定；AI 辅助编程则通过大语言模型、代码生成/补全工具来产出和优化代码，最终以“人 + AI”协同的方式推进项目。
- **编码工作量**：传统模式下，算法、流程、结构、接口、细节都要从零搭建；AI 模式会把大量重复、模板化或样式化的工作自动处理掉，人主要负责提需求、验证和监督。
- **能力侧重**：传统更看重编程语言熟练度、逻辑思维、数据结构、算法和架构；AI 模式在此基础上，还要求你会协作、会写提示词、会验证 AI 输出、会管理 AI 生成的系统。
- **速度与效率**：传统开发在结构清晰、可预期的项目里效率不低，但碰上重复或模板化任务会比较耗时；AI 辅助则在 boilerplate、重复逻辑和原型阶段能显著提速。
- **质量与可维护性**：传统代码更容易被开发者理解和维护，责任边界清楚；AI 生成速度快，但复杂项目里可能出现可读性差、结构重复、隐藏 bug 或安全风险。
- **学习门槛**：传统模式要先投入时间学语言、算法、工程思维，新手爬坡期较长；AI 模式能让新手更快写出可运行代码，以学代练、边做边学。
- **适用场景**：传统开发适合高复杂度、需求模糊、强调创新和质量的场景；AI 辅助更适合重复性任务、快速原型、标准模块、初稿编写以及追求开发效率的场合。
- **工具生态**：传统生态是 IDE + 手写/模板代码；AI 时代则出现了大量 coding 工具，涵盖代码生成、补全、语义搜索、错误检测、自动测试等能力。

![](img/50e2491a293c386eead7d68ea14bff3a.png)

### 3.AI 辅助编程中涉及的技术

💡

这次航海要做的，是一个 AI 驱动的内容工厂 Agent，它围绕三大核心能力展开：选题洞察、内容二创、快速发布。

从操作路径看，整体流程会经历这些环节：

第一环是拿数据：按关键词抓取公众号文章和小红书笔记；

第二环是分析：让大模型对采集内容做深度洞察，形成选题判断；

第三环是创作：从优质选题中筛选出值得做的方向，完成文章创作；

最后通过官方认可的 API，把笔记或图文自动发布出去。

整个实现路径的本质，就是把可靠的数据源、稳定的大模型服务、各平台的发布能力，以清晰的工程化方式串在一起。

为了降低上手难度，我们特别选了依赖更少、门槛更低的实现方式。

下面介绍项目里会用到的一些技术。出现专业术语时不必有心理负担——我们不需要研究每个技术的底层原理，只需要知道它在项目中解决什么问题、处于流程的哪一环。

#### 3.1 Next.js：我们的开发框架

Next.js 是一个轻量级全栈开发框架，学习曲线比较平滑，能同时覆盖前端界面与后端逻辑，适合快速构建完整应用，新手也能很快上手。这也是我推荐它作为本次航海开发框架的原因。

先解释“全栈开发框架”：传统开发模式下，做一个网站通常要分别学两套技术——前端管用户看到的页面、按钮、表单、布局，后端管用户登录、数据存储等业务逻辑。

很多时候前端用 React/Vue，后端用 Node.js 或 Python，两套知识体系几乎不重叠。

Next.js 的特别之处，就是把它整合成一套：用同一套技术搞定界面展示和后台数据处理，学习成本下降不少，对新手十分友好。

#### 3.2 SQLite：本地化数据库方案

数据库领域有 Supabase（基于 PostgreSQL）、MySQL 等许多选择。但为了降低学习成本、减少外部服务依赖，让大家快速把内容工厂跑起来，我们选择了完全本地化的 SQLite。

可以把它想象成藏在电脑里的 Excel：数据都存于本地文件，轻量、读写快，适合个人或小规模项目使用。它的优势在于配置简单——不需要安装独立数据库服务器，打开就能用；也不用额外学习数据库概念，使用过程几乎无感。

Supabase（Postgres）是另一个方向：它是功能更强的企业级数据库，需要独立运行，支持更复杂的查询、更大的数据量、更高的并发访问，但初始配置和使用都更繁琐一些。

因此，本次航海先用 SQLite 打通链路；等你的内容工厂真正规模化，或需要云端部署时，再升级到 Supabase。这样兼顾了快速起步和未来的扩展性。

#### 3.3 API：连接外部能力的桥梁

API 即“应用程序接口”，可以理解为一扇标准化的服务窗口：你发出清晰的请求，对方按约定返回结果，内部实现无需关心。API 让原本靠手动复制粘贴的流程，变得可编程、可批量、可定时。

这次航海会大量调用外部 API，比如公众号采集 API、小红书采集 API、大模型 API、内容发布 API 等。往大了看，一个在线产品其实就是多个 API 的组合与再包装。

简单概括：API 是不同服务之间沟通的接口，让我们能够直接使用别人已经开发好的能力。

![](img/4890371351c4f01210b2f2a750088acc.png)

#### 3.4 我们可能会用到的 API 平台

**大模型 API：**

AI 能力会贯穿本次项目的内容生产全流程：我们需要 AI 深度分析公众号文章，提炼选题价值与爆款要素；需要 AI 根据选题生成符合平台调性的内容初稿；还需要 AI 制作配套插图与封面，增强视觉表现。做这些事，都离不开大模型 API。

硅基流动（siliconflow.cn）：一个开源模型聚合平台，提供大量免费或低价的模型 API。本次项目中，内容创作的图片生成功能就使用了硅基流动免费的可灵模型。

DeepSeek（platform.deepseek.com）：国内采买成本很有优势的商业大模型服务之一。V3.1 在推理、代码生成、长文本理解上表现不错，价格却只有 GPT-4 的几十分之一，非常适合内容批量生成这种场景。

火山方舟（volcengine.com）：字节跳动旗下的企业级 AI 服务平台，提供豆包等模型的 API。它的稳定性、响应速度和性价比都可圈可点，而且豆包家族覆盖面广，文本模型、图像模型、视频模型都有。

OpenRouter（openrouter.ai）：手册主推的平台。它是一个大模型聚合服务，把 GPT 系列、Claude、Gemini 等几十个主流模型收进同一接入点；只需一个 OpenRouter API，就能调用这些模型。

本次手册以 OpenRouter 为主，实际使用时，你也可以按自己的情况调整。

**数据采集 API**

数据采集 API 是内容工厂自动化链条的第一步。可以把它看作一个不知疲倦的搬运工，帮你批量拉取各个平台的内容。

以公众号采集 API 为例：只要输入一个关键词或公众号名称，就能自动取回该号的历史文章，标题、正文、发布时间、阅读数、点赞数等字段一应俱全。过去需要手动复制粘贴的活儿，几秒内就能批量完成。

本次航海会使用 https://dajiala.com/ 的公众号采集 API，支持按关键词搜索文章。

市面上还有很多同类平台。比如 apify.com 是功能强大的通用采集平台，支持 Twitter、Instagram、YouTube 等几十个海外站点；未来如果要做跨平台分析或出海业务，它会是个值得关注的选项。

**内容发布 API**

如果说采集 API 是内容的入口，发布 API 就是产品的出口。它能把写好的文章、图片、视频自动投递到目标平台，省去手动登录、复制粘贴、排版这些重复劳动。

拿微信公众号来说：调用发布接口，程序就能自动把文章发布出去。

在本次项目中，公众号自动发布使用 wx.mgxingyuan.com。这个平台把公众号原本复杂的接口封装得很好，只需要传标题、正文、封面图等参数，就能完成发布。

小红书侧使用 note.limyai.com，它采用生成发布链接的方式来发布笔记。

理解了这个逻辑，你会看到：整个项目其实就是对各式 API 做串联与包装，最终聚合成一套完整的自动化内容生产系统。

### 4.Claude Code 和 Codex 的区别

这两款是当下讨论度最高的 AI coding 工具，特点也比较互补。Codex 速度偏慢，但代码质量稳定，定位问题、修改 bug 的能力很强；Claude Code 响应更快，前端审美和从 0 到 1 的搭建能力更突出，但最近幻觉率偏高，也一直面临“降智”的争议。

# Claude Code 和 Codex 怎么选？开发环境安装指南

Codex 可直接供 ChatGPT 会员使用，额度相对宽裕；每月 20 美元的 Plus 套餐基本能满足日常需求，并且 gpt-5-hign 在定位和修复缺陷方面非常强。它主要的问题是响应偏慢：单个任务常常要等半小时以上，工具链的成熟度也比 Claude Code 略低。

从整体来看，Claude Code 依旧是当前最出色的 AI 命令行编程工具。它的工具链最成熟，交互顺畅，subagent、自定义 slash、hook 以及各类细节能力都比眼下的 Codex 更完善。但最近 Claude Code 频繁出现能力下降，流量高峰时会切换到低成本模型；官方也多次承认过模型方面的问题，不过社区反馈和实际使用感受显示，它和早期版本相比仍有差距。

**选择建议**：如果预算允许，两款都装；重视产出质量就选 Codex，重视速度和综合平衡则选 Claude Code。可以先用 Claude Code 完成从 0 到 1 的编码，再让 Codex 负责审查和修 bug，用互补的方式把两者优势发挥到最大。

## 02. 准备开发环境并安装 Claude Code/Codex

在正式写代码前，需要先准备好开发工具、Node.js 基础环境，以及 Claude Code（或 OpenAI Codex）的相关配置。

### 1. 开发环境介绍

#### 1.1 VS Code 是什么

微软于 2015 年推出的 VS Code，是一款现代代码编辑器，跨平台、开源且免费。Windows 和 macOS 都能运行，无论使用哪种系统，都能获得一致的开发体验。

它的显著优势是体积轻、能力全。主流编程语言几乎都覆盖，包括 TypeScript、Python、Java 等数十种；安装包往往只有几十兆，启动迅速，功能却不亚于专业 IDE。扩展生态尤其丰富，可按需安装各类插件。本次要用的 Claude Code 和 Codex 也都有 VS Code 插件，能帮助快速上手。

VS Code 是目前最流行的开发工具之一。大家熟悉的 Cursor、Trae 等 AI IDE，也是基于 VS Code 深度定制而成。

#### 1.2 Node.js 是什么

先交代一个背景：JavaScript 最初只面向浏览器，代码只能在网页中执行。Node.js 的出现改变了这一局面，使 JavaScript 可以脱离浏览器，直接在服务器端运行。

Node.js 是建立在 Chrome V8 引擎之上的 JavaScript 运行时环境。通俗地说，它让 JavaScript 代码可以在本机执行。

为什么需要 Node.js？

在这次学习过程中，Node.js 承担着几项关键职责。

第一，它是运行 Next.js 项目的必备环境。Next.js 本身就是基于 Node.js 构建的 React 框架，缺少 Node.js，项目就无法启动。

第二，Node.js 自带的包管理工具（npm 或 yarn）是安装、管理项目依赖的核心。第三方库、框架和开发工具几乎都靠它来安装与更新，本次使用的 Claude Code 和 Codex 也不例外。可以说，Node.js 是整个前端工具链的根基。

**Node.js 的核心优势**

Node.js 使用事件驱动、非阻塞 I/O 模型，因此特别适合高并发场景。学习阶段可能体会不深，但在真实生产环境中，这种特性让它能高效应对大量用户请求。另一个优势是生态繁荣。npm 是全球最大的软件注册表，开源包数量超过两百万。几乎任何功能需求都能找到现成方案，开发效率因此大幅提升。

VS Code 与 Node.js 共同构成开发环境的两大支柱。VS Code 负责写代码，提供舒适高效的编辑体验；Node.js 负责运行代码，提供执行环境和工具支持。掌握这两个工具，后续学习就有了坚实基础。下一节将具体介绍安装与配置方法，让开发环境真正跑起来。

![](img/fc38a9410fd600d7999b11fbb25641aa.png)

### 2. 如何安装开发环境

#### 2.0 视频版教程

如果希望更直观地了解基础环境安装，视频分别用 Mac 和 Windows 演示了 VS Code、Node.js 的安装过程，并讲解如何通过 cc-switch 切换智谱或其他国内模型来驱动 Claude Code，帮助大家快速上手，实操大约需要 1-2 小时。

**Mac 视频版**

点击下方链接学习（建议先看完视频，再阅读文字部分）：

https://scys.com/view/docx/J4ETdEfOpo4P3kxAWQOcZJl7nWf#Rw5cdvwD5oS7f5xF3GEcQIcin1g

**Windows 视频版**

点击下方链接学习（建议先看完视频，再阅读文字部分）：

https://scys.com/view/docx/J4ETdEfOpo4P3kxAWQOcZJl7nWf#MbdwdHqCqoJdI4xutWGcTElinld

#### 2.1 安装 VS Code 环境

#### 2.1.1 Mac 版本

**VS Code 官网地址：https://code.visualstudio.com/**

![](img/22d8b36d2f1c1c76ab5ef1578ff137c0.png)

打开上面的网址，进入 VS Code 官方网站。

页面中间会出现 Download for macOS；若使用 Windows 电脑，则显示 Download for Windows。根据当前系统点击下载即可。

点击后会出现提示：

![](img/9b64c7852ff3b72c78d0c2818752115c.png)

这说明下载已经开始。打开电脑的下载目录，找到 VSCode-darwin-universal.zip，双击解压，随后会出现下方蓝色图标。

这个蓝色图标就是 VS Code，双击即可运行。

![](img/bbbc1d30213515a7c9709cdf193c6319.png)

在文件夹里点击 visual studio code，就能进入 VS Code 主界面。为方便以后使用，可以按住 Visual Studio Code 并拖入“应用程序”文件夹，之后直接打开即可。

![](img/153dddb2bb9f87754d05196007c63f51.png)

接下来打开 VS Code：

![](img/a3f6d8e2aa72dcade55365d167b78b00.png)

简单认识一下首页：左侧从上到下依次是项目目录、搜索、版本管理、调试、扩展安装。

![](img/a5c754fb333e72857a37776d7ca771b9.png)

点击项目文件，通过 “Open Folder” 可以打开指定文件夹。后续实操会用到这些功能，这里先了解即可。

![](img/80ded16154fd39ff6d3a48bbeba29696.png)

![](img/3cc273c5ba142b4ca61c5e82db49a3f4.png)

#### 2.1.2 Windows 版本

Windows 的安装思路与 Mac 类似，可参考上面的 Windows 安装视频。

先访问 VS Code 官网：https://code.visualstudio.com/

点击页面中间的 Download for Windows。

![](img/52f1f473e7c010ca4c415b157929d62e.png)

进入网站后，中间会看到 Download for Windows，点击下载对应系统的安装包。

点击之后会出现提示：

![](img/4e07efe06c31aa6672a536473fc4000c.png)

说明下载已开始。打开下载目录，找到 VS Code 安装文件，双击运行：

![](img/9b21b78ebd7ca6b1a76ddb214a0a7984.png)

按提示依次确认，点击安装，等待进度完成：

![](img/410186f6797d8bc4e9c890018044a8cc.png)

![](img/5c921bd624eefa6d67fa32be99485534.png)

安装结束后会自动弹出 VS Code 初始化界面，表示安装成功：

![](img/fbf8a9b5bbfff0194ea8f4816e9a07cf.png)

点击项目文件，通过 “Open Folder” 即可打开指定文件夹：

![](img/3ed8ae0ec1b3e9ef4154091c964ee703.png)

![](img/d8ec7d2f0a1cf512f24143ccfc5b6b88.png)

#### 2.2 安装 Node.js 环境

#### 2.2.1 Mac 版

Next.js 和 Claude Code 都依赖 Node.js 运行，因此要先确认本机已安装 Node.js 与包管理器 npm。

打开 Node.js 官网 https://nodejs.org/zh-cn/download ，页面如下：

![](img/45e582f2939fc3b28354ce7c386c1a00.png)

**Mac 电脑**

无需额外操作，向下滚动找到绿色的【Mac 安装程序】，下载对应系统的安装包（LTS 版本即可）。

下载完成后，会看到一个打开纸箱图标的 node-xxxx.pkg 文件，这就是 Node.js 安装包，双击运行。

![](img/94058b73ce193f68f63d54e5e148a6ea.png)

进入下一步页面，点击继续：

![](img/46cce2d3c63246681acde496d3e32eba.png)

继续点击继续：

![](img/2129426a926e605a95b98e1033bbf971.png)

点击同意：

![](img/5ea0913a600f23fbd58f6adc93b5b403.png)

点击安装，然后输入电脑开机密码：

![](img/9fc720df9e7733f612a4b9a197387d26.png)

最后出现安装成功页面，点击关闭：

![](img/ca0b04c1338c0c439102926ec4ca89ed.png)

此时可打开终端，执行 node -v 和 npm -v 查看版本号。

```bash
node -v
npm -v
```

```
`node -v
npm -v`
```

按 Command（⌘）+ 空格键，屏幕中央会出现搜索框。

输入“终端”（或英文 Terminal）。

搜索结果中第一个通常就是“终端”，按 Enter 回车即可打开。

打开终端后，把 node -v 粘贴进去，按回车执行。

如果终端执行 node -v 后出现如下提示，说明 Node.js 已安装成功。

**注意**：v22.19.0 是版本号，不同电脑版本可能不同；只要执行 node -v 能看到版本号，就表示安装完成。

![](img/f15e2dcb4529750d1b8489f94b976627.png)

![](img/00d44bc6c6e31556cbb5bd5c1cfe6ed6.png)

#### 2.2.2 Windows 版

详细安装过程可参考上面的 Windows 安装视频：

https://scys.com/view/docx/J4ETdEfOpo4P3kxAWQOcZJl7nWf#MbdwdHqCqoJdI4xutWGcTElinld

先打开 Node.js 官网 https://nodejs.org/zh-cn/download ，进入后点击 Windows 安装程序下载：

![](img/a4e15a164b305d61836c4ad1ba5077f2.png)

**双击 node.js 安装包**

![](img/b99d3eeee6c01c7c71a898ac4b256f57.png)

按提示进入下一步，选择继续；再下一步选择同意：

![](img/899e042253d1a58e354cebc315eaaf99.png)

![](img/dd047b2d461fd4684ce5549562c7a699.png)

稍等片刻，会提示安装完成：

![](img/e7b5eec9829831fe75c913a57952044d.png)

在开始菜单搜索 cmd，打开命令提示符：

![](img/9c9a61e463c403349feb275c43541b04.png)

在终端中执行 node -v 和 npm -v 检查版本号。

```bash
node -v
npm -v
```

```
`node -v
npm -v`
```

如果执行 node -v 后出现如下提示，说明 Node.js 安装成功。

**注意**：v24.11.0 是版本号，不同电脑版本可能不同；只要执行 node -v 能看到版本号，就表示安装完成。

![](img/bd211188977fbf05d0fa907f58c8dbcc.png)

![](img/64244ecd233d3ec12daea28f606db658.png)

### 3. 安装 Claude Code

Claude Code 与 Codex 二选一即可，两者的具体差异见第一章 01 节第 4 小节。

#### 3.1 Mac 版本

打开电脑终端，执行：

```bash
npm install -g @anthropic-ai/claude-code
```

```
`sudo npm install -g @anthropic-ai/claude-code`
```

等待一段时间后，如果 Claude 提示安装成功：

![](img/42e8a4ead851548f6c97f089b0ada6dc.png)

💡⚠️注意：如果安装时报下面的错误（图片见下），说明需要管理员权限，在命令前加上 sudo 再执行。

将下面这条命令复制到终端：

```bash
sudo npm install -g @anthropic-ai/claude-code
```

然后在终端输入电脑开机密码。注意，终端不会显示输入的密码，直接输入即可；例如开机密码是 1234，就在钥匙🔑标志后输入 1234，再按回车。

图片如下：

![](img/39fac07ee2b030138d3b6dedc2448fc0.png)

![](img/4a2dd0e04699c69944af0e6a45b4445a.png)

完成以上配置后，Claude Code 环境就准备好了。在终端执行 claude -v，如果出现 Claude Code 版本号，说明安装成功。接下来可以用 cc-switch 配置 API。

![](img/fc474dea20c7b4c4fcf5013dd5113205.png)

![](img/d596de9c07dc74141c715bac14a3ded6.png)

#### 3.2 Windows 版本

Windows 安装 Claude Code 前，需要先装 git，否则会报错：

![](img/e44ce66ac1b8513f0659046180c48324.png)

打开 git 官网：https://git-scm.com/install/windows

可以点击 Click here to download，或选择对应系统版本。为方便起见，直接选第一个，即 Git for Windows/x64 setup：

![](img/75ea57b66ce1360d73d713855d5d2d75.png)

下载完成后打开安装包，点击安装：

![](img/ec37d68d29f2285243a150c0183647d0.png)

一路按下一步完成安装，最后点击 Finish 关闭：

![](img/7cae043faa2554c1fe9c72af24baa2e9.png)

然后继续安装 Claude Code。

在开始菜单搜索 cmd 打开终端：

![](img/0aeec711ed5391fe4f583ad7047c6fd2.png)

在终端执行下面的安装命令：

```bash
npm install -g @anthropic-ai/claude-code
```

```
`npm install -g @anthropic-ai/claude-code`
```

出现下面提示表示安装成功：

![](img/60d65f84f7b2b32ab3f9906ce5ed8ddd.png)

在终端输入 claude 进行验证，如果进入主题模式选择界面，说明 Claude 已安装成功。后续按登录方式验证后即可使用：

![](img/95e1609d79d8dac054a1c26910874079.png)

![](img/cc97f77965fb4807ede554e114857e44.png)

### 4. 安装 Codex

💡 若已装好 Claude Code，Codex 可以跳过；若觉得 Claude Code 上手偏难，也可以改用 Codex。二者装一个即可。

如果你是 ChatGPT Plus 或 ChatGPT Pro 的订阅用户，建议把 Codex 也一起装上。它在查找和修复 bug 上会比 Claude Code 略胜一筹；但如果是做从 0 到 1 的项目起步，或是前端视觉要求高，Claude Code 的表现会更好。

#### 4.1 用终端安装 OpenAI Codex

因为后面要操作本地环境和数据库，所以建议直接用终端来安装 Codex，不要从 ChatGPT 界面进入。

4.1.1 Mac 版本安装 Codex

在 Mac 的终端里，用 Command（⌘）+ V 粘贴下面这行命令，然后回车：

```
npm i -g @openai/codex
```

Plain Text

```
`npm i -g @openai/codex`
```

![](img/5b934b61a1333d7a6735db3f2452cb9a.png)

如果出现和之前安装 Claude Code 时一样的权限不足提示，那就需要加上 sudo 再来一次。

![](img/fb63e8af32d5018c7339d2813874c165.png)

复制下面这行到终端并回车（操作步骤与 3.1 相同）：

```
sudo npm i -g @openai/codex
```

Plain Text

```
`sudo npm i -g @openai/codex`
```

接着输入开机密码。注意终端不会显示密码字符，直接键入即可。比如密码是 1234，就在钥匙🔑标志后敲 1234，然后回车。

![](img/6b8e61324c00fe95b5c97cc194152184.png)

以上步骤完成后，Codex 的运行环境就准备好了。在终端输入 codex 会进入交互式对话界面，看到这个就说明安装成功。接下来参考下一节登录。

![](img/2fd5b10ed1c27bacfcb9a3001171294c.png)

![](img/f81c415c26a9e413e32b0d15313511df.png)

4.1.2 Windows 安装 Codex

同样，把下面的命令复制到终端，回车运行：

```
npm i -g @openai/codex
```

Plain Text

```
`npm i -g @openai/codex`
```

稍等片刻，如果出现类似下面的提示，就表示 Codex 已装好，环境准备就绪。

![](img/0ff1f4792ebce9de6cd169c761e67b33.png)

在终端里输入 codex，进入交互式对话模式，即可认定安装成功。推荐使用 WSL2 来操作；不过为了省事，也可以直接选 2 继续。登录方法参考下一节。

![](img/28d94c1f57f676a42a6e36a63a56a015.png)

#### 4.2 用 ChatGPT Pro/Plus 打开 Codex

Codex 也支持云端访问：打开 chatgpt.com，只要订阅了 ChatGPT，左侧就有 Codex 入口，点击即可。但考虑到我们这次需要操作本地环境和数据库，不建议用云端版，了解即可。

![](img/1dcb3a1a8474b49fbf1a0ae81ce5fa86.png)

## 03. 激活并配置你的 Claude Code/Codex 账号

下面是 Claude Code 和 Codex 的激活配置说明，任选其一即可。

### 1. Claude Code 登录与使用

Claude Code 有两条使用路径：一是官方原版，二是用国内模型（比如 GLM4.6）来驱动。

官方原版需要先在 Claude.ai 上完成订阅。现在 Claude 提供 Pro、5x MAX、20x MAX 三档套餐，价格分别为每月 20 美元、100 美元、200 美元。同时，Claude 一直限制国内访问，用官方版还得想办法解决网络和海外信用卡支付，门槛不低。如果是新手，建议直接用国内模型来驱动 Claude Code。

下面以 GLM4.6 为例，讲讲这两种方式。

**第一种方式：使用国产模型驱动 cc**

这里借助一个 GitHub 开源小工具 cc-switch，它可以让你在不同模型之间快速切换，从而驱动 Claude Code。项目地址是：https://github.com/farion1231/cc-switch

Windows 和 Mac 版本都提供了，开箱即用：

Windows 版本：[ ![](img/926059c88a0af05a7cef1a4ab97cb185.png) CC-Switch-v3.5.1-Windows-Portable.zip ](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/VfcdbCf4hoqTtJxYH47cXVWtnRk?response-content-disposition=attachment%3B%20filename%3D%22CC-Switch-v3.5.1-Windows-Portable.zip%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260109%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260109T022502Z&x-oss-expires=86400&x-oss-signature=89e5153ad59231d22e5dc4107b6c5ff2f991b40bd7b3cbb9773ee16323908c6c&x-oss-signature-version=OSS4-HMAC-SHA256)

Mac 版本：[ ![](img/89bf74e1ede2779666a283fe9fdf85a6.png) CC-Switch-v3.5.1-macOS.zip ](https://sphere-sh.oss-cn-shanghai.aliyuncs.com/private/docx/drive/media/CuJUbp3oxoAhTXxtM83caIS3nxc?response-content-disposition=attachment%3B%20filename%3D%22CC-Switch-v3.5.1-macOS.zip%22&x-oss-credential=LTAI5tDANFnEjK2qWnHwZKzr%2F20260109%2Fcn-shanghai%2Foss%2Faliyun_v4_request&x-oss-date=20260109T022502Z&x-oss-expires=86400&x-oss-signature=008757ac75d0e5e86395925cb0f13a2f214a820f8fb1a1051807ed3698efcfbb&x-oss-signature-version=OSS4-HMAC-SHA256)

当然，也可以直接去这里下载：https://github.com/farion1231/cc-switch/releases

安装好后打开 cc-switch，界面如下图所示。

![](img/d1760af2ba13e680cfb5d705e7930494.png)

点击“添加供应商”，在弹出的窗口里可以选择任意供应商，只需配好对应的 API Key 即可。这样一来，用不同模型驱动 cc 的成本就大大降低了。

![](img/342464ac942a676f58f860157dc33133.png)

比如想用 glm-4.6 来驱动 cc，先去智谱开发者平台（https://www.bigmodel.cn/usercenter/proj-mgmt/apikeys）复制 API Key，再填入 cc-switch 并点击启用。搞定之后，就可以用 glm-4.6 驱动 Claude Code 了。

![](img/e0f7921dfb428fd83d8c613865e7ec6e.png)

另外，glm-4.6 也有官方的 coding 套餐，有需要可以直接购买：https://bigmodel.cn/glm-coding

![](img/726c6364e405366a7bbc71693b7f3486.png)

**第二种方式：官方原版 Claude Code**

⚠️ 这里有个高频报错需要提醒：如果本地没有配置全局代理，可能会看到类似 “Unable to connect to Anthropic services, please check your internet connection and network settings” 的提示。如果接下来要用智谱等国内模型驱动 cc，这个报错可以先忽略；如果要跑官方原版，请继续看下面的解决方案。

![](img/55d16593efdd2eea3d7122e6c20a0b30.png)

**网络错误解决方案**

处理上述网络错误，需要修改 Claude Code 的配置文件。路径如下：

- Mac：/Users/[电脑用户名]/.claude/settings.json
- Windows：C:\Users[电脑用户名]\.claude\settings.json

比如我的 Mac 用户名是 limo，那配置路径就是 /Users/limo/.claude/settings.json。如果该文件不存在，就新建一个。

![](img/262754587b2094eb89160a61a54e3abb.png)

用文本编辑器打开 settings.json，把下面的代理配置加进去。注意！端口必须与自己的代理软件一致：比如 HTTP 端口是 7890，就写 7890；如果是 7897，也要改成 7897。

JSON

```
`{
  &quot;env&quot;: {
    &quot;HTTP_PROXY&quot;: &quot;http://127.0.0.1:7890&quot;,
    &quot;HTTPS_PROXY&quot;: &quot;http://127.0.0.1:7890&quot;
  }
}`
```

配置完成后，重启终端并输入 claude，即可进入官方版 Claude Code 的初始界面。

官方原版需要突破两关：一是干净的网络环境（指纹浏览器+静态住宅 IP 会更稳，否则封号率很高）；二是可用的海外信用卡，用 Google Pay 或 App Store 内购也行。目前官网三档套餐分别为 Pro（20 美元/月）、MAX 5X（100 美元/月）、MAX 20X（200 美元/月），核心差异是限额大小，以及能否使用 Opus 4.1 等更高阶模型。

如果网络和海外支付中任意一点搞不定，官方版 cc 可以直接跳过，用前面说的国内模型驱动方案就好。

下面是官方 Claude Code 的登录流程。

**Mac 版：**

在终端输入 claude 进入对话界面，然后输入 /login：

```
`/login`
```

![](img/aef3fe8c46566e294c9209b62bd22dc4.png)

选择 “Claude account with subscription”，回车。

![](img/0828d877e9930b1a8413c83bbd640dbd.png)

系统会自动唤起浏览器；如果没有自动跳转，可以手动复制链接到浏览器里授权。

![](img/3a68517a911770fd60bf7f2b0d928304.png)

![](img/ff12fb35143e6daa12dfa42e6f84eae8.png)

**Windows 版：**

Windows 的授权方式和 Mac 大同小异。先在终端输入 claude，进入下图所示的界面，再输入 /login：

![](img/c4658670b25ecf1b931cedf0d62c0195.png)

这时会询问是通过账号订阅授权还是 API 授权，直接默认回车即可。

![](img/a6290d9239143dc29a04b1eeaa7ebed4.png)

回车确认后，浏览器会自动打开 claude.ai 的登录页面。如果订阅了 Claude Pro 或 Max，登录账号并确认即可完成授权。

![](img/ed278a259931e1bdc806676b3d1e4912.png)

如果浏览器没有自动打开，也可以把控制台里的链接复制出来，手动粘贴到浏览器访问 claude.ai 完成登录，同样会自动授权。

![](img/0c2188f8bd1f87342a1fb189a6630796.png)

**Claude Code yolo 模式（自动挡模式）**

用 Claude Code 时，经常会遇到需要手动确认文件修改的情况，频繁确认很容易打断思路。这时候可以切换为 yolo 模式，让 Claude Code 自动工作，解放双手。

一行命令即可开启：

```
claude --dangerously-skip-permissions
```

当左下角出现 “bypass permissions on” 的提示，就说明 yolo 模式已生效。

![](img/24c4497b6a2cf9b8ab412bd04a1ab630.png)

yolo 模式很适用于从 0 到 1 新建项目，无需反复接受变动，写代码的过程会顺滑许多。

不过每次都敲这一大串命令确实麻烦，能不能让 claude 默认就是 yolo 模式？方法很简单——配置终端别名。不需要自己写，直接给 Claude Code 发下面这个指令：

Plain Text

```
`请帮我在终端配置一个别名，使得输入claude时自动执行claude --dangerously-skip-permissions命令`
```

这样以后执行 claude 时，终端左下角也会出现 yolo 模式的提醒。

至此，开发环境就配置完毕了。接下来正式开始项目开发。

### 2. Codex 的登录与使用

前面已经完成了 Codex 的安装，并且在终端输入 codex 成功进入了对话框。现在来登录它。

⚠️ 注意：Codex 需要 ChatGPT Plus、ChatGPT Team 或 ChatGPT Pro 的会员才能使用，没有会员是用不了的。

![](img/383df7edeb8871615a8e7fe7323b73ee.png)

在对话框中选择第一项 “Sign in with ChatGPT”。之后浏览器会自动打开，终端里也会出现一个授权链接。终端里的链接可以忽略，直接在浏览器页面登录 ChatGPT 账号即可。

![](img/1d98b554f948bd37265e74c9f628a7a9.png)

在自动弹出的页面中，输入 ChatGPT 的账号密码并登录。

![](img/ff7cc9101a42894f8038eabacc0edff3.png)

登录后会出现一个“是否允许 ChatGPT 登录到 Codex”的提示，点击“继续”。

![](img/8d7360739a55c82593a3341da8d321d8.png)

点“继续”后再等大约一分钟，就能看到登录成功的提示。

![](img/b051e8bc31d3e874e801e0462edf809c.png)

回到终端，同样会看到登录成功的提醒。到这儿，Codex 就可以正常使用了。

![](img/777e497ca01ceeed5ebf4a4b6e064253.png)

环境准备阶段到此全部完成，下面我们进入正式的开发阶段。

# 二、搭建内容采集与数据分析 Agent

## 01. 页面原型设计

### 0. 本章概要

💡 **本章概要**

前期的环境搭建和背景介绍花了不少篇幅，相信你已经装好了 Claude Code 和 Codex。现在开始进入真正的项目开发环节。

整个体系可以拆成四个模块：数据采集、选题分析、AI 改写、一键发布。它们彼此独立，又相互关联。接下来的章节会逐个实现，先从最基础的数据采集开始，逐步搭起一个完整的 AI 内容工厂。这一章先从页面原型做起。

⚠️ 注意：之后的实操演示会以 Claude Code（cc）为主。如果你用的是 Codex，开发方式和 cc 完全一样，直接在 Codex 中正常对话即可，提示词等都不需要改动。

💡 **本章航线图**

完成本章的学习与实践，就能走完航线图的第二阶段：搭建内容采集与分析 Agent，总耗时约 7 天。

- 用 AI 工具进行页面原型设计：约 2 天
- 用 AI 工具获取公众号数据：约 2 天
- 用 AI 工具开发数据分析功能：约 1 天

和 AI 协作，最重要的一件事是什么？把需求对齐。如果自己都不知道要做什么，AI 能力再强也无法给出满意的结果。所以必须准备一份清晰的需求文档，它可以是你和 AI 反复对话后逐步明确的。

这里还有一个认知上的转变：现阶段 AI 的能力已经超过大多数人了。因此不必害怕提出想法，大胆去和 AI 讨论细节。AI 编程和传统人工编程的底层逻辑没什么不同——都需要精准定义需求。需求对不齐，就别指望结果符合预期。

# 先聊透需求，再动手做原型（视频+指令）

别一上来就编码。更稳的做法是先把想法讲给 CC，把执行方案定下来。下面把过程录了下来，配套输入内容也一并给出。

### 1. 视频演示

这段录像展示的是：用对话形式把想法、要求、实施思路同 CC 过一遍，再根据反馈增补、调整，最后得到一版原型草图。动手时间约 1～2 小时。若你使用 Codex，照着 CC 的流程操作即可，两边可用的输入内容没有差别。

建议先刷完视频，再对照下面的文字步骤；链接在这里：

https://scys.com/view/docx/J4ETdEfOpo4P3kxAWQOcZJl7nWf#Fz6udIpdhoJ0RLxvxglcpYWcnte

文字流程附后，动手耗时同样约 1～2 小时：

### 2. 先做出首版原型

2.1 建一个空目录当项目根目录

先挑一个目录，在里面建空目录作为项目根目录。比如我在示例里用了“mini 航海”这个名字：

![](img/089eba77a4658cf83491a4bbd3570c32.png)

2.1 从 VS Code 启动 Claude Code

启动 VS Code 后，会先看到初始界面。在窗口左上区域找到文档形状按钮，点开后选择 Open Folder：

![](img/d6eb3825db1a7c80ef7d0515c72e5b2d.png)

选中刚才创建的那个目录：

![](img/26f1cd0037834203d30e7c6946072a62.png)

随后界面会变成一片空白：

![](img/ff4c1aa0628b73d70ae8c313c33c2281.png)

在顶部菜单条里定位 Terminal，展开后选 New Terminal：

![](img/928e82b646db68c9567db6121360b4db.png)

这时下方会新增一个 Terminal 面板：

![](img/7720c63bc2fc5eab5b371ac5b0df2681.png)

在下面的 Terminal 面板里敲入 claude 并回车，就会进入 Claude Code；此时输入框已经可以接收指令。若你用的是 Codex，则敲 codex 后回车，之后步骤与 Claude Code 一致，把同一份输入内容粘贴过去即可。

![](img/588bbb97ef0e766208c93b1f555c5050.png)

2.3 把整段内容交给 Claude Code（Codex 同样适用）

将下面这段内容整体拷贝，放进 Claude Code 中；用 Codex 的话，照同样方式处理即可。

Plain Text

```
`请和我一起讨论一个需求，我希望做一个内容工厂agent，主要由三个部分组成，第一部分是选题分析，需要支持根据关键词获取公众号文章（有第三方API，且可以获取到标题正文，阅读数，点赞数，在看数，然后使用openai兼容的AI接口对每篇文章首先进行概要分析，然后再整体结合这些概要进行选题洞察，使用ai  api生成洞察报告。注意洞察报告需要包括点赞量最高的五篇文章，互动率最高的五篇文章，高频词云，五个选题洞察。

第二部分是内容创作，需要支持针对生成的选题进行一键AI创作，生成新的文章，生成新的文章中第一步使用upsplash获取一些相关图片插入其中，注意为了方便管理需要新建一个发布管理的页面，所有AI生成的文章都要放到发布管理页面的列表中，并且文章还需要有一些状态方便管理。
第三部分就是发布。针对生成的文章在列表操作栏需要有发布到小红书和发布到公众号两个选项，这一部分也有第三方API。为了方便和快速上手我希望你使用next.js框架和sqlite数据库。针对我以上的想法，请你首先帮我讨论需求，并帮我设计页面结构和主要元素布局，可以用简要的线框图形式描述方便我们对齐确认。`
```

2.4 和 Claude Code 核对需求

这一步里，AI 会先发来一版它理解的需求清单。把 CC 给出的需求梳理与方案通读一遍：若与你的设想一致，就让它照此推进开发；若有出入，继续多轮讨论，直至满意。

我的经验是：首版原型值得反复打磨。初次和 AI 谈需求时，若线框图或页面设计没达到你的标准，就继续迭代，先别催它进入编码。

![](img/3a5e424209050a3f86c1d0f9a667b660.png)

![](img/465c63653e9f3e35c55c362c01fd1921.png)

CC 的完整回复放在下面，供你对照参考：

SQL

```
`需求分析与细化
基于您的描述，我理解这个内容工厂Agent的核心价值是：自动化内容创作流程，从选题分析到发布的全链路解决方案。让我帮您细化需求：
1. 选题分析模块
核心功能：
根据关键词抓取公众号文章（通过第三方API）
AI分析每篇文章的概要
生成综合洞察报告
需要明确的问题：
一次分析多少篇文章比较合适？（建议20-50篇）
互动率的计算公式：(点赞数+在看数)/阅读数？
高频词云是否需要过滤停用词？
洞察报告是否需要保存历史记录？
2. 内容创作模块
核心功能：
基于选题一键生成文章
自动插入Unsplash相关图片
文章状态管理（草稿、待审核、已发布等）
需要明确的问题：
文章状态流转：草稿 → 待审核 → 已发布？还是需要其他状态？
图片插入策略：自动插入几张？位置如何确定？
是否需要支持手动编辑生成的文章？
是否需要文章版本管理？
3. 发布模块
核心功能：
发布到小红书
发布到公众号
发布记录追踪
需要明确的问题：
不同平台的内容格式差异如何处理？
是否需要定时发布功能？
发布失败如何处理和重试？
页面结构设计
基于需求，我建议采用以下页面结构：
内容工厂Agent
├── 首页/仪表盘
│   ├── 快速入口
│   └── 数据统计概览
│
├── 选题分析
│   ├── 关键词输入区
│   ├── 分析进度显示
│   └── 洞察报告展示
│
├── 内容创作
│   ├── 选题列表
│   ├── 创作按钮
│   └── AI配置参数
│
├── 发布管理
│   ├── 文章列表（表格）
│   ├── 状态筛选
│   ├── 批量操作
│   └── 发布操作
│
└── 设置
    ├── API配置
    └── AI模型配置
主要页面线框图
1. 选题分析页面
┌─────────────────────────────────────────┐
│  🔍 选题分析                              │
├─────────────────────────────────────────┤
│                                          │
│  关键词输入：[___________] [开始分析]      │
│                                          │
│  ┌──────────────────────────────────┐   │
│  │ 分析进度                          │   │
│  │ ▓▓▓▓▓▓▓▓▓▓░░░░░ 60%             │   │
│  │ 已分析：12/20篇                    │   │
│  └──────────────────────────────────┘   │
│                                          │
│  ┌──────────────────────────────────┐   │
│  │ 洞察报告                          │   │
│  │                                   │   │
│  │ 📊 点赞TOP5    📈 互动率TOP5      │   │
│  │ 1. 文章A       1. 文章X           │   │
│  │ 2. 文章B       2. 文章Y           │   │
│  │ ...           ...                 │   │
│  │                                   │   │
│  │ ☁️ 高频词云                       │   │
│  │ [词云可视化图]                    │   │
│  │                                   │   │
│  │ 💡 选题洞察                       │   │
│  │ • 洞察1：xxxxx                    │   │
│  │ • 洞察2：xxxxx                    │   │
│  │ ...                              │   │
│  │                                   │   │
│  │ [保存报告] [基于洞察创作]          │   │
│  └──────────────────────────────────┘   │
└─────────────────────────────────────────┘
2. 发布管理页面（核心页面）
┌─────────────────────────────────────────┐
│  📝 发布管理                              │
├─────────────────────────────────────────┤
│                                          │
│  [新建文章] [批量操作▼]                    │
│                                          │
│  筛选：[全部状态▼] [全部来源▼] 🔍[搜索]    │
│                                          │
│  ┌──────────────────────────────────┐   │
│  │ 标题      状态    创建时间   操作   │   │
│  ├──────────────────────────────────┤   │
│  │ 文章1    草稿    2024/1/1   [编辑] │   │
│  │                            [预览] │   │
│  │                            [发布▼]│   │
│  │                             └小红书│   │
│  │                             └公众号│   │
│  ├──────────────────────────────────┤   │
│  │ 文章2    待审核  2024/1/2   [编辑] │   │
│  │                            [预览] │   │
│  │                            [发布▼]│   │
│  ├──────────────────────────────────┤   │
│  │ 文章3    已发布  2024/1/3   [查看] │   │
│  │         (小红书)            [复制] │   │
│  └──────────────────────────────────┘   │
│                                          │
│  [上一页] 1 2 3 ... 10 [下一页]          │
└─────────────────────────────────────────┘
3. 内容创作页面
┌─────────────────────────────────────────┐
│  ✍️ 内容创作                              │
├─────────────────────────────────────────┤
│                                          │
│  选题来源：                               │
│  ○ 从洞察报告选择  ○ 自定义输入           │
│                                          │
│  ┌──────────────────────────────────┐   │
│  │ 可用选题                          │   │
│  │ □ 选题1：xxxxx                    │   │
│  │ □ 选题2：xxxxx                    │   │
│  │ □ 选题3：xxxxx                    │   │
│  └──────────────────────────────────┘   │
│                                          │
│  创作参数：                               │
│  文章长度：[800-1200字▼]                  │
│  写作风格：[专业严谨▼]                     │
│  图片数量：[3张▼]                         │
│                                          │
│  [开始创作]                               │
│                                          │
│  ┌──────────────────────────────────┐   │
│  │ 预览区                            │   │
│  │                                   │   │
│  │ 生成中...                         │   │
│  │                                   │   │
│  └──────────────────────────────────┘   │
└─────────────────────────────────────────┘
Update Todos
需求分析与细化
设计数据库结构
设计页面结构和布局
绘制线框图
Thinking

数据库结构设计（SQLite）
-- 1. 分析任务表
CREATE TABLE analysis_tasks (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    keyword VARCHAR(100) NOT NULL,
    status VARCHAR(20) DEFAULT &#x27;pending&#x27;, -- pending/processing/completed
    total_articles INTEGER,
    analyzed_at DATETIME,
    created_at DATETIME DEFAULT CURRENT_TIMESTAMP
);

-- 2. 洞察报告表
CREATE TABLE insight_reports (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    task_id INTEGER,
    top_likes_articles TEXT, -- JSON格式
    top_engagement_articles TEXT, -- JSON格式
    word_cloud TEXT, -- JSON格式
    insights TEXT, -- JSON格式
    created_at DATETIME DEFAULT CURRENT_TIMESTAMP,
    FOREIGN KEY (task_id) REFERENCES analysis_tasks(id)
);

-- 3. 文章表
CREATE TABLE articles (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    title VARCHAR(200) NOT NULL,
    content TEXT NOT NULL,
    summary TEXT,
    source VARCHAR(50), -- &#x27;ai_generated&#x27; or &#x27;imported&#x27;
    status VARCHAR(20) DEFAULT &#x27;draft&#x27;, -- draft/pending_review/published
    images TEXT, -- JSON格式存储图片URLs
    report_id INTEGER,
    created_at DATETIME DEFAULT CURRENT_TIMESTAMP,
    updated_at DATETIME DEFAULT CURRENT_TIMESTAMP,
    FOREIGN KEY (report_id) REFERENCES insight_reports(id)
);

-- 4. 发布记录表
CREATE TABLE publish_records (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    article_id INTEGER NOT NULL,
    platform VARCHAR(20) NOT NULL, -- &#x27;xiaohongshu&#x27; or &#x27;wechat&#x27;
    platform_id VARCHAR(100), -- 平台返回的文章ID
    status VARCHAR(20) DEFAULT &#x27;pending&#x27;, -- pending/success/failed
    error_message TEXT,
    published_at DATETIME,
    created_at DATETIME DEFAULT CURRENT_TIMESTAMP,
    FOREIGN KEY (article_id) REFERENCES articles(id)
);

-- 5. 系统配置表
CREATE TABLE settings (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    key VARCHAR(50) UNIQUE NOT NULL,
    value TEXT,
    updated_at DATETIME DEFAULT CURRENT_TIMESTAMP
);
Update Todos
需求分析与细化
设计数据库结构
设计页面结构和布局
绘制线框图
Thinking

技术实现建议
API路由结构（Next.js App Router）
/app
├── api/
│   ├── analysis/
│   │   ├── start/route.ts      # 开始分析
│   │   └── status/route.ts     # 查询状态
│   ├── articles/
│   │   ├── route.ts            # CRUD操作
│   │   └── generate/route.ts   # AI生成
│   ├── publish/
│   │   ├── xiaohongshu/route.ts
│   │   └── wechat/route.ts
│   └── settings/route.ts
关键技术点
并发控制：分析多篇文章时使用Promise.all配合并发限制
流式响应：AI生成内容时使用SSE推送进度
图片处理：Unsplash API调用时注意速率限制
状态管理：使用Zustand或React Query管理客户端状态
样式方案：推荐使用Tailwind CSS + shadcn/ui快速搭建UI
工作流程图
选题分析 → 洞察报告 → 选题确认 → AI创作 
                              ↓
发布管理 ← 文章编辑 ← 图片插入 ← 内容生成
    ↓
平台发布 → 小红书/公众号
下一步行动建议
先验证核心功能：建议先实现选题分析和AI创作的最小可行版本
API接入准备：
OpenAI兼容接口（如通义千问、智谱等）
公众号文章抓取API
Unsplash API
发布平台API
渐进式开发：选题分析 → 内容创作 → 发布管理
您觉得这个方案如何？有哪些地方需要调整或深入讨论的吗？我们可以先确定哪个模块优先开发，然后我可以帮您搭建项目框架和实现核心功能。`
```

## 原型先行，后端暂缓

读完那份需求报告后，我发现 cc 给出的理解与我的预想基本吻合。所以第一步，我只让它依据需求文档搭出原型，后端逻辑暂时不用碰。

提示词如下：

Plain Text
```
`很好,请你首先帮我实现所有页面的原型,暂时无需实现后端逻辑`
```
![](img/5bbbebb7c2e545dbd3ba49dd7597988d.png)
![](img/9e6f6e4f1dae3b507bb7c1fc4f5fa9d5.png)

大约过了三十分钟，cc 顺利把原型做了出来。

![](img/25ebe39cf2ca360282a95223fd797955.png)

### 3.报错先别慌

原型生成成功后，接着就可以让 cc 把项目跑起来，做第一轮验证。不过这次任务链路较长，首次启动难免碰到报错——截图里那些红色文字就是错误提示。

![](img/b4ee6aa4c615368f3856ba1ea32f9a25.png)

遇到这种情况不用着急，把错误提示原封不动发给 cc 就行。比如第一次启动时出现了下面的提示：

Plain Text
```
`报错，请解决下：【复制报错的日志信息】`
```

这时，可以把 Claude Code 生成的站点链接放到浏览器中访问。

![](img/c73dbb9fe518561238f5ba8253a6ec02.png)

提醒一句：链接粘进浏览器后如果打不开，很可能是项目尚未启动。处理方法很简单，直接对 Claude Code 说：“localhost:3000 打不开，请你帮我启动项目。”

### 4.第一版原型调通

当 cc 完成修改并成功启动项目后，我们眼前出现了第一版原型：

![](img/87c9d6aaf64c1b271e86e4ddf17b10e8.png)

表面上看，该有的组件似乎都齐了，但版式排得很散，大概率是部分样式信息没有加载上。遇到这种情况，直接把截图发给 cc 就行。

![](img/18ebb6ca41b0d56b4c2b75e758895d02.png)

![](img/5e18f41978d5b90d5e969964a313d4e7.png)

描述时不用复杂，把眼前的现象如实说清楚即可：

Plain Text

```
`样式全都乱了：【附加你的截图】`
```

![](img/e44da69bedfd5817c361b17c4d0973c2.png)

没过几分钟，cc 就完成了修正。我们重新打开本地页面，样式已经恢复正常；再切到其他页面检查，结果也基本符合预期。个别小细节暂时不用急着让 cc 处理。

注意：第一版原型阶段，我们只要确认页面能正常跳转、核心元素大致齐全就够了。等后面逐个页面补逻辑时，再慢慢调整也不迟。

## 02.抓取公众号文章数据

💡 在 01 节里，cc 已经帮我们把原型搭好了。接下来要落地第一个核心功能：按关键词抓取数据，并据此做选题分析。这里先拿公众号举例，采集文章后再进行分析。

### 1.视频讲解

这段视频主要讲两件事：怎样接入公众号 API，以及如何按关键词拿到公众号文章，并做一轮简单的数据分析。动手实操大约需要 2—3 小时。

建议先看视频，再读下面的文字版。视频入口：

https://scys.com/view/docx/J4ETdEfOpo4P3kxAWQOcZJl7nWf#LgYydT1zhoRDaOxVRtncON6VnRd

文字版内容如下（实操预计 2—3 小时）：

### 2.对接公众号数据接口

公众号采集 API 我们选用第三方服务，例如极致了数据。通过这个平台，视频号和公众号的主要接口基本都能拿到，按需付费即可，日常需求大多能覆盖。

先打开极致了官网： https://dajiala.com/

登录方式：点右上角，用微信扫码即可。首次登录需要绑定手机号并设置密码。

![](img/46194368f21e620e3def36e33a4b2798.png)

充值路径：右上角头像——API 充值续费——进入文档页面。

⚠️注意：首次使用需要付费，按自己的用量购买即可。开发阶段可以采取“多次少量”的充值方式，先保证流程能跑通。

另外，极致了 API 每次调用约 4 毛钱（可获取 20 篇文章）。第一次充值可以适当多充一些，因为第二次充值最低要 200 元！！！

![](img/6c223c6d3cd6c8afd7836edb07ec6d40.png)

进入平台后，视频号/公众号的 API 信息一目了然。借助这些接口，我们可以按关键词抓取视频号信息或公众号文章，也能获取指定博主的数据。这里先以“按关键词搜索微信文章”作为示例，其他接口可以结合自己的业务场景接入。

![](img/7fe700fb21f4d74a30fe90208f3a0be9.png)

找到这个 API 后，点击“在线调试”进入文档页。如果想让 cc 帮忙接入任意 API，只需把接口文档交给它即可。

需要重点提供三块内容：API 请求参数、密钥信息、返回值信息。只要这三样齐全，任何外部 API 都可以让 cc 嵌进我们的系统。

下面就以接入公众号数据为例，让 cc 把完整的公众号获取逻辑实现出来。提示词太长的话可以跳过不读，直接复制组装好的版本发给 cc。

先复制请求信息：在“请求示例代码”处点击复制：

![](img/cd34f7245dd4361a71ce7f2d723eb0a1.png)

然后回到响应部分，点击“生成代码”，复制返回信息。

![](img/982899b5179697316554eb2cb77185a3.png)

![](img/c4a920bf0afce9e59d2249a7afdb7d76.png)

接着复制密钥信息。地址是 https://dajiala.com/main/interface?actnav=0 ，在页面中复制密钥即可。

![](img/82e9c6c84a9fce016d08ab51179fa345.png)

最后，把这三部分拼成提示词，发给 cc：

![](img/4348bf9b3ed7c70e1167eb75b5b80009.png)

![](img/dd6ca9b8a603ce8a1032bcd8b4f9a98b.png)

组装后的完整提示词如下。复制时记得把提示词里的 KEY 替换成自己的密钥：

ProtoBuf

```
`请你帮我完成选题分析这个页面中获取公众号文章的逻辑，根据关键词获取公众号文章的API接口如下，key为：{重点，这里填写你自己的key!!：XXXXXXX，就是刚刚在极致了复制的密钥}：curl --location --request POST &#x27;https://www.dajiala.com/fbmain/monitor/v3/kw_search&#x27; \
--header &#x27;Content-Type: application/json&#x27; \
--data-raw &#x27;{
    &quot;kw&quot;: &quot;人民日报&quot;,
    &quot;sort_type&quot;: 1,
    &quot;mode&quot;: 1,
    &quot;period&quot;: 7,
    &quot;page&quot;: 1,
    &quot;key&quot;: &quot;{{key}}&quot;,
    &quot;any_kw&quot;: &quot;&quot;,
    &quot;ex_kw&quot;: &quot;&quot;,
    &quot;verifycode&quot;: &quot;&quot;,
    &quot;type&quot;: 1
}&#x27;
返回消息是：export interface ApifoxModel {
    code: number;
    cost_money: number;
    cut_words: string;
    data: Datum[];
    data_number: number;
    msg: string;
    page: number;
    remain_money: number;
    total: number;
    total_page: number;
    [property: string]: any;
}

export interface Datum {
    /**
     * 封面
     */
    avatar: string;
    /**
     * 分类
     */
    classify: string;
    /**
     * 正文
     */
    content: string;
    /**
     * 原始id
     */
    ghid: string;
    /**
     * 发布地址
     */
    ip_wording: string;
    /**
     * 是否原创
     */
    is_original: number;
    /**
     * 再看数
     */
    looking: number;
    /**
     * 点赞数
     */
    praise: number;
    /**
     * 发布时间
     */
    publish_time: number;
    publish_time_str: string;
    /**
     * 阅读数
     */
    read: number;
    /**
     * 文章原始短链接
     */
    short_link: string;
    /**
     * 文章标题
     */
    title: string;
    /**
     * 更新时间
     */
    update_time: number;
    update_time_str: string;
    /**
     * 文章长连接
     */
    url: string;
    /**
     * wxid
     */
    wx_id: string;
    /**
     * 公众号名字
     */
    wx_name: string;
    [property: string]: any;
}`
```

约十分钟后，cc 提示公众号搜索已经接入成功。我们来验证一下：

![](img/80cb79d66d4573357449e924c9ecf459.png)

![](img/0ed7fcd182a6fd4dbf35d3aaf1f1d004.png)

### 3.应对项目报错

【项目报错怎么处理？】如果发现功能失败，先别慌。直接在页面上右键，选择“检查”：

![](img/9c0c7538d26cb7aa944ff621bc622467.png)

然后切到控制台：

![](img/686880a25e9f1cad72895dc470f747b4.png)

控制台里确实出现了红色报错日志。把这些报错信息复制出来，原样交给 cc 即可：

Plain Text

```
`报错了，请修改：【详细的报错信息】`
```

如果一次没解决，就按同样的方式多试几轮，直到问题消失。以刚才的报错为例，我们把信息发给 cc 后，它一次就修好了，关键词下的文章也能正常显示：

![](img/dd9b0aeabac593f540164e59f2e31831.png)

💡 AI coding 的排错流程可以这样理解：

比如刚才右键“检查”弹出的窗口到底是什么？又该去哪里找错误日志？

第一，点击“检查”打开的是浏览器开发者工具，它会实时展示网页运行过程中的信息。

第二，Console（控制台）标签页会显示运行时的错误信息，比如哪一行代码出错、哪个资源加载失败。红色文字通常代表错误，点开就能看到详细说明和出错位置。Network 标签页则能查看页面加载了哪些文件、哪个请求失败了。

排查时优先看 Console 里的红色提示，它往往能直接指出问题所在。这是前端开发中最基础也最重要的调试手段。

第三，看到红色异常信息后，直接复制给 AI 工具，让它协助排查。大多数情况下，90% 以上的基础 bug 都能被解决。

### 4.优化现有内容

背景：刚才已经按关键词抓到了全部数据，但这些数据有没有存进数据库？以后想回看历史记录该怎么办？拿不准的时候，可以让 cc 帮忙确认。

提示词：

Plain Text

```
`现在数据是否有保存?我希望保存到sqlite中.另外我希望每次查询的关键词都可以保存到一个列表中,我可以查看历史的关键词以及选题信息.请帮我确认以上问题并设计我的新需求的线框图并和我确认,先不要着急修改代码,设计完成后和我确认后再开工`
```

大约十分钟后，cc 给出了一套完整方案：

![](img/6f9acf29f5c2d287bc0b96a1a657d829.png)

![](img/222f73005bb51b7420a307cfe4c813cb.png)

cc 也按照我们的要求，对需求做了确认。

![](img/bf11c97c7339e053899ff0ffb1156bde.png)

我们结合实际情况回复即可：

Plain Text

```
`1.当前方案即可 2.选项A 3.每次分析自动保存 4.保存完整的文章原始数据 5.暂时不需要 6.`
```

经过一段较长的等待，cc 通知修改完成。我们直接验证：

![](img/fc465dc29f1986d408019f20f4b60a30.png)

可以看到，所有历史搜索记录都已成功保存。完整过程在视频里也能看到。

💡 页面内容如何迭代优化

遇到不满意的地方或有新需求，比如“我发现抓取到的 top 文章点不开原文”，可以直接把需求告诉 Claude code：【现在有个问题，获取到的 top 文章没有办法点击查看原文，你帮我修改下】

流程就是：发现需求——告诉 AI 工具——再确认功能是否实现。

## 03.增加选题分析能力

公众号数据抓取已经跑通，基础数据分析也有了：话题下的高赞文章、高互动文章、高频词云等信息都能呈现（如下图）。接下来，我们希望让 AI 对已收集的文章做选题分析。

![](img/0ec47d43b73494f9d303a7467a833a34.png)

### 1.视频教程

上一节我们按关键词拿到了公众号文章，也完成了初步的选题分析，但分析维度还比较单一。这段视频会讲如何接入 AI 大模型，对文章做更深入的分析，并生成选题洞察。实操时间约 2—3 小时。

同样建议先看视频，再读文字版。视频入口：

https://scys.com/view/docx/J4ETdEfOpo4P3kxAWQOcZJl7nWf#OpTHd9Y0ZokHZ1xtqwUc5bXhn0b

文字版内容如下（实操预计 2—3 小时）：

### 2.提出新的开发需求

💡 背景：公众号关键词采集和选题报告的基础功能完成后，会发现当前的选题洞察主要依赖数值指标（阅读量、点赞量等），没有真正挖掘文章内容本身的价值。这样一来，洞察结果对选题方向、内容痛点、受众需求的解读不够深，后续做选题策划时参考价值有限。

因此，我们需要让 AI 阅读所有 top 文章：逐篇读取高赞、高互动内容，提取核心观点、受众需求等信息，再做聚合分析，形成更深入的选题结论。顺着这个思路，我们继续让 cc 修改。

先把想法告诉 cc，让它先出一版方案供确认。

![](img/451efebbb69f9b904b6b60047eea0f64.png)

![](img/da15a93ab99a9a3c0a3b1a5b50d9c577.png)

提示词

Plain Text

```
`请你帮我修改一下选题洞察部分的逻辑，目前的状态是一个简单的数值分析，我希望是可以使用 Openai 兼容的 AI 大模型首先对所有的 top 的文章去进行一个摘录，简要的分析，然后要把原文中的一些关键信息，一些关键词，还有文章的亮点进行结构化，然后再次使用 AI 大模型对这些摘要之后的文章细节去进行选题洞察的分析。
我希望是能够输出至少 5 条结构化的选题的洞察，而这样的话方便我去后续的分析和对这一个话题更深的了解，
请你根据我的这一个需求去帮我进行设计，并且标记可能修改的所有的地方。不要着急修改代码，只需要调研后首先和我确认一下需求和变动范围`
```

这里有个小插曲：我们忽略了上下文已满，cc 压缩上下文后直接输出了英文。大意是它在向我们确认几个问题，并针对这些问题给出了建议：

Markdown

```
`为你准备的问题
在我开始实施之前，请确认：
1. **API 提供商**：你是想直接使用 OpenAI，还是 Azure OpenAI，或者其他提供商？
2. **模型选择**：
    - gpt-4o-mini（便宜、快速、足够好）——我的推荐
    - gpt-4o（更贵、质量更高）
    - 其他？
3. **降级行为**：如果 AI 失败，我们应该：
    - 选项 A：显示基于规则的洞察（用户可能不会注意到差异）
    - 选项 B：显示错误消息且不显示洞察
    - 选项 C：显示基于规则的内容 + 警告横幅 “AI不可用，显示基础分析”
4. **数据库**：你是否希望在数据库中跟踪哪些洞察是 AI 生成的，哪些是基于规则的？
    - 是：添加 `aiGenerated` 字段
    - 否：保持架构不变
5. **缓存**：我们是否应该为相同的关键词缓存 AI 洞察？
    - 是：节省 API 成本，但洞察可能过时
    - 否：始终保持最新，但成本更高

### 我的建议
基于我的分析：
1. 使用 gpt-4o-mini —— 最佳成本/性能平衡
2. 静默降级为基于规则的方案 —— 更好的用户体验（UX）
3. 最初不修改数据库架构 —— 保持简单
4. 目前不使用缓存 —— 始终保持洞察最新
5. 显示详细的进度指示器 —— 用户喜欢看到 AI 的工作过程`
```

针对 cc 的补充问题，我们逐一回复：

Plain Text

```
`1. 可以首先配置openai 的url在环境变量中我可以随时改动
 2.gpt-4o 
3.option C 
4. yes 
5. no ,不要缓存`
```

![](img/c237615f1a8aae04d17851099d67ff4c.png)

![](img/0ba7e00dfe30372f802b59be15bc6342.png)

大约十分钟后，这部分功能开发完成，cc 还给出了后续操作安排。

它安排的后续行动计划是：1. 确保项目能启动；2. 设置 OpenAI 的 base URL 和 key；3. 进行分析验证。

![](img/b66910bc500421f3f0a9bed1c4b73310.png)

### 3.补全数据分析功能

按照前面 Claude code 的建议，我们照做：启动项目，然后配置模型信息。这里用 openrouter 做演示，大家也可以换成自己熟悉的中转站，没有强制限制。因为一开始在提示词里就提了要求：只要接口兼容 OpenAI 即可。

# 接通 OpenRouter：让 AI 帮我做选题分析

先访问 OpenRouter 官网：https://openrouter.ai/。页面右上方的“Sign Up”就是入口，点进去创建账户；用 Google 授权或邮箱注册都行。

![](img/94ae914e58f4bcd203153b3cf6ae5487.png)

完成注册、进入登录状态后，从右上角头像点进控制台。第一次用可以先加一点余额，比如 5 美元，选择“Add Credits”。

![](img/b82be9772287986b815d1078483bbec5.png)

![](img/7641e686c857e6521c673ccd3e10b0ba.png)

在弹窗底部展开“Use one-time payment methods”，用支付宝或微信付款即可。

![](img/721d818f525079b089ce3200bcf9c283.png)

余额到账后，切到“Keys”，按下“Create API Key”。

![](img/9b3e99bbb180357b11c6a148ce5d5f52.png)

“Name”一栏随意起个名字。

![](img/7b5be2d99f745f9e87741019b5a97d5a.png)

![](img/cb2c4d789c5b1f27aa7f3ddded643f7c.png)

按下“Create”后会出现一条新 key，复制它，粘贴进项目里的 .env.local（此前 cc 已提醒要填在这个环境变量文件）。

![](img/7223f942dd5484b98ec45be9dfa41112.png)

打开 .env.local，把这条 key 放到 OPEN_API_KEY 等号右边。

![](img/074f90638e419b3cc3d779b00b9594d1.png)

再翻到 OpenRouter 的快速开始文档：https://openrouter.ai/docs/quickstart，把 base url 粘到 OPENAI_API_BASE 这一项。

![](img/4612528be1c57b90ad0af13e8d2f6060.png)

还剩一步：告诉程序用哪款模型来做选题分析。进入模型广场：https://openrouter.ai/models

![](img/c1cad93ac3e9cdcd42db11df0e52bb7e.png)

挑中模型后复制其名称，再写进 .env.local；最后几项变量看起来像下面这样。

![](img/d706897b37719d6c4ae04a0c7081025e.png)

到这儿，大模型接口信息就填齐了。返回前端试跑，用“副业”作为检索词跑一次分析。

![](img/b477e1e70619e0245c3b0c870241fb52.png)

![](img/958fee4bad25a61050a25c3ce23d50ff.png)

![](img/44c0caf88f72200de78e0f758cfad8c5.png)

![](img/fd4f9436f8fb2d4bc88e5092beacfa9d.png)

结果页的洞察区域已经换成 gpt-4o 在出分析结论。

![](img/19ff4879e603cdbfc7297577d4827a86.png)

### 4. 把页面上的毛刺逐个修掉

前面已经把“抓取微信文章 + 调大模型做选题分析”这条链路跑通。接下来只做针对性修补：搜索框与按钮不在一条线上、文章没有全部露出、标题太长把版式撑乱等。动手约半小时。

视频入口如下（建议先看视频，再读文字）：

https://scys.com/view/docx/J4ETdEfOpo4P3kxAWQOcZJl7nWf#Vntbdl9OUo5aX7xzK9qcK065n8d

这部分没有统一答案，AI 生成结果带随机性，你的页面和我的版本可能差得不少。原型阶段我常处理的点有：

+ 样式：AI 爱用的渐变配色容易让系统显得毛糙。若你已有品牌主色，可以直接让 AI 替换；也可以指定 shadcn、21st.dev、diasyui 这类三方 UI 库来重做界面。因项目周期短，且与内容工厂主题关联不深，这里没展开；若你要求样式统一，可以让 AI 采用特定库。
+ 样式细节：元素对齐、字体呈现、布局排版、loading 页等，都可按偏好微调。比如视频里我把“开始分析”按钮与输入框拉齐，并对过长的标题做了截取。

![](img/5f4b70700d97bfd46f3cb88286b950bc.png)

### 5. vibe coding 的指令写法小结

这一节收个尾：从零开始拿到微信文章数据，再让大模型产出选题分析，前后只写了约五条指令；代码一眼没看，cc 自己把项目搭完。

下面是我写指令的一些体会：

启动新项目时，开头发出的那条指令最值钱，它要帮我们划定功能范围，先把原型跑出来。我的做法是：先到 Claude 或 ChatGPT 里来回聊，把产品要做什么、不做什么盘清楚，最好落成一份需求文档；再带着文档去 Claude Code 里对齐。需求本来就要边做边改，别指望一次把细节全交代完。

这套路数和传统软件研发没有本质差别，变的是角色：以前要抹平产品经理与开发之间的理解差，现在要抹平我们与 AI 之间的理解差。双方认知对齐，结果才稳，这是可控性的底座。

后续指令大致可归为三类：

一、纠偏：发现 AI 跑偏就立刻拉回。再强的模型也可能误读需求，越早指出越省返工。

二、确认：它理解对了，就点头让它往下走，别额外加戏，信任其执行。

三、补料：AI 再能干也缺真实业务背景。看它回复时，把关键上下文补进去，比让它自行脑补稳得多；这些补充常常决定成品是否合用。

另外，做 vibe coding 不必把指令雕成花。那些动辄数百字的“提示词工程”不必再迷信。抓住两点：圈定功能范围，点明技术栈；表达尽量短，常识部分 AI 会自己补。需要时按业务顺序列步骤，比如先做什么、再做什么。

短和细并不打架，反而互相补位。短，是去掉废话，把冗长铺陈砍掉；细，是在要紧处舍得写，比如补一份必要文档、把输出格式钉死、把不能碰的操作范围划清。该讲透的讲透，不该展开的别展开。

上面这些，是我和 AI 一起写代码时攒下的指令用法。说到底，就是把自己放在产品经理的位置，把 AI 当成一支开发小队：用尽量少的沟通成本对齐目标、消掉歧义、一轮轮改。别神化复杂技巧，摸清 AI 的脾气，用大白话把需求讲明白，往往就是最管用的 prompt。希望这些体会能帮到你。

# 三、内容再加工与多平台分发功能开发

## 01. 写作模块：成稿与智能配图

上一环里，我们已经按关键词抓到微信平台的相关文章，并让大模型给出洞察和分析结论。接下来就借这些结果，进入写作模块。

### 0. 这一节先看什么

前面几节走完了微信关键词数据采集、接大模型分析文章、产出选题结论这条线。

现在要进入二次加工：围绕上一步的选题洞察做定向写作，同时接入 AI 配图，让成稿图文齐全。

本节还会说清楚：已经写好的稿子怎么送进公众号草稿区，以及怎样通过扫码发到小红书。

学完并动手做完，航线图第三阶段就算完成——内容再加工与多平台分发开发（约 8 天）：

+ 写作模块：成稿与智能配图（约 4 天）
+ 分发模块：一键发到小红书和公众号（约 4 天）

### 1. 对已有内容做再加工

#### 1.1 视频讲解

视频里演示的是：拿第一部分的选题结论去生成正文，并顺手配几张随机图；全程用三条指令，动手时间约一到两小时。

视频链接（建议先看完视频，再读文字）：

https://scys.com/view/docx/J4ETdEfOpo4P3kxAWQOcZJl7nWf#X0d2dunGMokZrZxRFJUcPUzsncc

下面给文字步骤（预计同样一到两小时）：

#### 1.2 把改动交给 ClaudeCode

背景：现在的写作页分三块——选题来源、当前能选的选题、写作参数。大框架符合预期；若你有别的想法，直接找 cc 改就行。

这次仍按原型思路把数据串起来。眼下的“可用选题”还是假数据，跟上一阶段产出的选题没有真正打通，所以先处理它。

![](img/c92c8c44028480be191cd4c982285922.png)

给 cc 的修改指令：

Plain Text

```
`你帮我修改一下内容创作者这个页面，我希望从洞察报告中选择的时候，可以实时的获取到选题分析中不同的关键词生成的选题洞察报告，这部分数据要能够联动起来
另外可用选题部分按照时间的顺序去进行倒叙排序。
同时我还希望在进行开始创作的时候，你可以参考我目前本地环境变量中配置的与OpenAI 兼容的大模型的 API 的一些基本信息调用 AI 去给我生成文章。
请结合现在的页面的现状，以及选题分析中关于选题洞察生成的相关的逻辑首先设计技术方案，对于设计可能变动的地方罗列出来，然后再和我进行需求上的确认。在我获得我的许可之后再去进行代码的修改。`
```

![](img/4d9025a62e43a09875a61ae80732041e.png)

![](img/33cfa13ef2e0c47db19467dd2216066d.png)

把上面这段丢给 cc，等它忙活一阵，方案就出来了：

TypeScript

```
`完美！基于你的选择，我来完善技术方案：

🎯 最终技术方案确认
根据你的选择，我将实现以下功能：

核心功能点
✅ 下拉框选择关键词：在选题来源区域添加关键词下拉框，切换后显示对应的洞察列表
✅ AI参考洞察生成：将选题标题+洞察描述一起传递给AI，生成更符合洞察建议的文章
✅ 自动保存草稿：生成后自动保存到数据库（需要新建Draft表）
✅ 智能推荐图片：基于文章关键词，生成Unsplash图片链接

需要变动的文件（最终清单）
数据库变更（1个文件）
prisma/schema.prisma
- 新增Draft表
model Draft {
  id          Int      @id @default(autoincrement())
  title       String
  content     String   // Markdown格式
  wordCount   Int
  readingTime Int
  keywords    String?  // JSON数组
  images      String?  // JSON数组
  topic       String   // 选题
  createdAt   DateTime @default(now())
  updatedAt   DateTime @updatedAt
}

新增文件（3个）
app/api/insights/list/route.ts
- 获取所有关键词及洞察
app/api/content/generate/route.ts
- AI生成文章
utils/content-prompts.ts
- 文章生成Prompt模板

修改文件（1个）
app/create/page.tsx
- 内容创作页面大改造

📦 具体实现细节
1️⃣ Draft表设计
model Draft {
  id           Int      @id @default(autoincrement())
  title        String   // 文章标题
  content      String   // 文章正文（Markdown）
  wordCount    Int      // 字数
  readingTime  Int      // 阅读时间（分钟）
  keywords     String?  // 关键词（JSON数组）
  images       String?  // 图片链接（JSON数组）
  topic        String   // 原始选题
  insightId    Int?     // 关联的洞察ID（可选）
  metadata     String?  // 其他元数据（JSON）
  createdAt    DateTime @default(now())
  updatedAt    DateTime @updatedAt
}

2️⃣ 图片智能推荐逻辑
// 基于文章关键词生成Unsplash搜索URL
function generateImageUrls(keywords: string[], count: number): string[] {
  const images = []
  for (let i = 0; i &lt; count; i++) {
    const keyword = keywords[i % keywords.length] || &#x27;creative&#x27;
    images.push(`https://source.unsplash.com/800x600/?${encodeURIComponent(keyword)}`)
  }
  return images
}

3️⃣ 页面交互流程
用户访问创作页面
  ↓
加载所有分析历史（关键词列表）
  ↓
[选择关键词] → 显示该关键词的洞察列表（按时间倒序）
  ↓
[勾选洞察] + [设置参数] → 点击&quot;开始创作&quot;
  ↓
调用 /api/content/generate
  ↓
AI生成文章（参考洞察描述）
  ↓
生成Unsplash图片链接
  ↓
自动保存到Draft表
  ↓
展示文章预览

4️⃣ AI Prompt示例
你是一位专业的公众号内容创作者。

请基于以下选题和洞察建议，创作一篇高质量文章：

【选题】
${topic}

【选题洞察】
${insightDescription}

【创作要求】
- 文章长度：${contentLength}字
- 写作风格：${writingStyle}
- 内容要求：结合洞察建议，写出有价值、可读性强的文章

请返回JSON格式：
{
  &quot;title&quot;: &quot;文章标题&quot;,
  &quot;content&quot;: &quot;文章正文（Markdown格式）&quot;,
  &quot;keywords&quot;: [&quot;关键词1&quot;, &quot;关键词2&quot;, &quot;关键词3&quot;]
}

🚀 开始实施？
现在我将按照以下顺序开始编码：
✅ 修改prisma/schema.prisma，添加Draft表
✅ 运行数据库迁移
✅ 创建/api/insights/list API
✅ 创建utils/content-prompts.ts
✅ 创建/api/content/generate API
✅ 改造app/create/page.tsx
✅ 测试完整流程

确认无误后，我将开始编码！ 准备好了吗？ 🎉`
```

先粗看方案有没有大偏差；若没有，就照它执行。

![](img/86f3b2af60d8a1d6f7bb6ec76d97a212.png)

Plain Text

```
`没问题,请你帮我实现`
```

功能一复杂，cc 也会有翻车的时候，难免冒出意料之外的问题。不用紧张，把报错原样贴给它就行。比如写作这块，中途就出过两次状况：

![](img/6b68d329a3863260a30043fddcdd24ea.png)

第一轮跑出来就报错，功能没达到预期。新手未必看得懂报错细节，也不必死磕原理；把错误日志复制给 cc，或者干脆截张图发过去：

Plain Text

```
`点击开始创作之后报错:【错误日志/错误截图】`
```

报错信息通常指向更明确，多数情况下一次就能把同类问题处理掉。

到这里，写作部分的主功能就通了：正文能正常产出，也能落进草稿区：

![](img/6c53444a9e84ab96b20f96f9df269852.png)

![](img/38d5fa23e94496f546a43ad1071238dc.png)

### 2. 让 AI 自动配图

到这一步，写作主链路已基本跑顺。但落到实际使用，还有不少可打磨的地方。

比如，现在正文所配图片是从 upsplash 随机取的，和文章主题关系不大。对一篇完整且质量在线的稿子来说，图文脱节会直接拉低阅读体验，所以要把这个问题修掉，让图片跟正文对得上。

可选路径不少，比如即梦 4API、qwen-image、flux、midjourney 等。为降低上手门槛，可以先用“硅基流动”提供的免费可灵生图模型；正式环境再按需换成即梦 4。

#### 2.1 视频讲解

# 配图懂语义，发布走捷径

先说明这期内容要处理什么：文章需要贴合语义的插图，而硅基流动可免费调用可灵来按文章意思出图。整套流程动手约 60 分钟。

下方是视频入口，建议完整看过再对照文字操作：

https://scys.com/view/docx/J4ETdEfOpo4P3kxAWQOcZJl7nWf#ErqSdwWUwoGFp2xVNABccIwmnbJ

文字流程附在后面，实际操练预留 60 分钟左右：

#### 2.2 让 Claude code 完成实现

先打开硅基流动的模型页：https://cloud.siliconflow.cn/me/models

在分类筛选里选“生图”，再挑那款免费可灵：

![](img/d2ecbe8f93992828e1f49a2db0a38094.png)

接着进入接口说明页：

![](img/3cffb371bbc912744d5da20b985f4bd4.png)

把请求参数与返回示例整理出来，拼成提示词，再发送给 cc：

![](img/c9b959ffb00c1bad53d894d02884532a.png)

JSON

```
`现在就是有一个问题，在内容创作这一个页面，目前生成文章的时候，生成图片的逻辑其实是去随机获取图片的，但是这种和文章的关联性很差，就我希望你去调用硅基流动的官方的生图 API，然后使用可灵模型去帮助我生成文章的配图。
整体流程就是你可以首先根据生成的文章内容去调用 AI 接口去生成指定张数的这个图片的提示词，然后根据这些图片提示词再去调用图像生成接口，再去生成文章内的插图。
所以你根据我刚刚的需求去深入分析相关的代码，然后给出我技术方案，然后并且和我确认需求，在得到我的许可之后再去进行这个代码的修改。
硅基流动可灵模型的接口文档为:curl --request POST \
  --url https://api.siliconflow.cn/v1/images/generations \
  --header &#x27;Authorization: Bearer &lt;token&gt;&#x27; \
  --header &#x27;Content-Type: application/json&#x27; \
  --data &#x27;{
  &quot;model&quot;: &quot;Qwen/Qwen-Image-Edit-2509&quot;,
  &quot;prompt&quot;: &quot;an island near sea, with seagulls, moon shining over the sea, light house, boats int he background, fish flying over the sea&quot;
}&#x27;返回参数为:{
  &quot;images&quot;: [
    {
      &quot;url&quot;: &quot;&lt;string&gt;&quot;
    }
  ],
  &quot;timings&quot;: {
    &quot;inference&quot;: 123
  },
  &quot;seed&quot;: 123
},model 为:Kwai-Kolors/Kolors,API KEY为:【这里填写自己的APIKEY！！！！！】`
```

![](img/9041c4696e5b4569f51b66cad25c47dd.png)

cc 花了一些时间核对改动边界，并向我们确认了几个待回答的问题：

![](img/d85fa01f5b5af2d53030698b6f1ba045.png)

我们逐项回复：

Plain Text

```
`第一个问题，请你使用方案 a 进行生成。第
二个问题，OK，使用现有的 Openai 模型去生成一个提示词。
第三个关于错误策略的处理，就是我希望不要去降级使用随机图片，如果说没有去生图片失败的话，那直接跳过就 OK 了，然后只需要给用户提示，告知用户本次的文章生成出中有生成图片错误的情况就可以了。
第四的话不需要批量生成。
第五的话，硅基流动的 API 是有配额限制的，所以说请你不要去并发的获取生成所有的图片。同时不需要添加一个缓存机制。至于单张图片的生成时间，预估可能在1~3分钟之内，暂时可以不必考虑异步方案，请你帮根据我刚刚上面的补充，帮我实现我们最初的需求`
```

确认完需求，大约三十分钟后，cc 交付了这次改动：

![](img/4efef6eac9713b501821aa8c99fd1aab.png)

![](img/01c0f9e724ff971cd7f7626d711f5750.png)

把应用跑起来，随手产出一篇试稿，第一次执行就成功了：

![](img/099bca18fb9b2cf4a7efef3ec988584e.png)

## 02.发布模块：草稿流向小红书与公众号

接下来处理收尾环节：发布。目标是让写好的稿子经由平台开放接口送到外部。

本章只处理两条投递路径：公众号与小红书；两边门槛并不一样：

+   **公众号**：有正式开发接口，可把文章送进草稿箱并发布；但开发者要先拥有公众号权限，还要配好接口，例如 appid/secret、白名单之类。

+   **小红书**：开放平台有 API，用户走 OAuth 授权后就能调用内容发布接口。可开放的权限范围未必大，所以不少开发者会选模拟登录等替代方案。本教程仍按官方开放 API 发布来写。

实现时分成微信端和小红书端，但用户只看到一个统一发布界面。

### 1.公众号侧发布

#### 1.1 视频演示

这一节演示怎样把写好的内容投到公众号草稿区，预计要花 1—2 小时。

视频入口：

https://scys.com/view/docx/J4ETdEfOpo4P3kxAWQOcZJl7nWf#YzVBdwp1gocVikxRIZncvJEdn1m

建议先完整观看，再读下面的文字流程。

文字流程如下（动手约 1—2 小时）：

#### 1.2 用 ClaudeCode 接通公众号发布

公众号和小绿书这两条投递链路，我们选择通过第三方 API 来打通。

之所以绕开官方直连，是因为微信开放平台的基础接入本身就很繁琐，常常两三周都打不住。

因此第三方 API 更省时间。若你有自己的云服务器，并且公众号已经实名，也可以走官方接入；但过程复杂，这里不展开。想研究可看：https://developers.weixin.qq.com/doc/subscription/guide/（非技术背景大概率难以搞定）

操作顺序：

第一步：打开公众号开放平台，填入相应网址，先做公众号绑定。绑定成功后，账号下关联的公众号信息就能读取出来。

第二步，核心只有两处接口：

+   其一为“获取已绑定公众号”接口，调用后返回当前账号下全部已绑定公众号列表。

+   另一个是发布接口，给它标题、正文与目标账号名，稿子就会保存到对应草稿区。

功能层面，我们把需求交给 CC：为“发布公众号”按钮补齐逻辑——用户点击后弹出一个选择层，里面展示可用的已绑定账号，并允许选中其中一个；同时提供“小绿书/公众号”两个去向选项；按下发布，后台自动匹配接口并完成草稿投递。

流程清楚后，前往 https://wx.mgxingyuan.com/ 提交 API 申请，激活码填 2QGAW036。

扫码绑定微信后，在 https://wx.mgxingyuan.com/api-doc/publish 取接口文档，把它交给模型配合使用。

先让 cc 输出文档与实现设计：

![](img/20066c224b3fa81ea1fa3f587d087619.png)

![](img/b5229d6d110408fa1799027f89f1ff4e.png)

![](img/e54f30a47fc08bce817d899ed55d8a4e.png)

看完 cc 的方案，我们提出调整建议并确认，再让它执行；结果一次跑通，公众号发布功能就此完成：

![](img/1f4f8e07fa8d42eb6f646e2b4bff8dc0.png)

![](img/2c6902a9bc34d1661276ebe358a37736.png)

下面列出公众号发布环节的完整提示词：

ProtoBuf

```
`请你帮我修改发布管理这个页面，就我希望实现发布到公众号的逻辑，就是首先去用户点击发布到公众号这个按钮之后，要跳出来一个弹窗，这个弹窗上面可以去选择要发布的公众号和要发布的发布类型，发布类型同时支持发布到公众号文章和小绿书，用户选择之后去点击发布。

下面是涉及到的公众号发布的两个接口，第一个接口就是用于获取这一个 API key 下的所有的公众号的信息，第二个接口就是根据用户选择的公众号去执行一个发布的操作，下面是这两个接口对应的 API的文档。请你根据 API 文档以及提供的key 先进行一个流程和技术方案上的设计，请你务必去深入研究所有相关的代码，首先把改动的范围也去罗列出来，不要着急修改代码，先和我确认好了之后再进行代码的变动。

下面是文档：
# API接口文档：获取公众号列表

## 接口说明
获取当前用户授权的所有微信公众号信息

## 接口地址
POST https://wx.limyai.com/api/openapi/wechat-accounts

## 请求头
X-API-Key: your-api-key
Content-Type: application/json

## 请求示例 (cURL)
```bash

curl -X POST https://wx.limyai.com/api/openapi/wechat-accounts \

  -H &quot;X-API-Key: your-api-key&quot; \

  -H &quot;Content-Type: application/json&quot;

```

## 响应示例

```

{

  &quot;success&quot;: true,

  &quot;data&quot;: {

    &quot;accounts&quot;: [

      {

        &quot;name&quot;: &quot;测试公众号&quot;,

        &quot;wechatAppid&quot;: &quot;wx1234567890&quot;,

        &quot;username&quot;: &quot;gh_abc123&quot;,

        &quot;avatar&quot;: &quot;https://...&quot;,

        &quot;type&quot;: &quot;subscription&quot;,

        &quot;verified&quot;: true,

        &quot;status&quot;: &quot;active&quot;,

        &quot;lastAuthTime&quot;: &quot;2024-01-01T00:00:00.000Z&quot;,

        &quot;createdAt&quot;: &quot;2024-01-01T00:00:00.000Z&quot;

      }

    ],

    &quot;total&quot;: 1

  }

}

```

## 响应字段说明

+   name: 公众号名称

+   wechatAppid: 公众号AppID

+   username: 公众号原始ID

+   avatar: 公众号头像URL

+   type: 公众号类型（subscription=订阅号, service=服务号）

+   verified: 是否认证

+   status: 状态（active=正常, revoked=已解绑）

+   lastAuthTime: 最后授权时间

+   createdAt: 创建时间

# API接口文档：发布公众号文章

## 接口说明

将文章发布到指定的微信公众号草稿箱

## 接口地址

POST https://wx.limyai.com/api/openapi/wechat-publish

## 请求头

X-API-Key: your-api-key

Content-Type: application/json

## 请求参数

| 参数名 | 类型 | 必填 | 说明 |
| --- | --- | --- | --- |
| wechatAppid | string | 是 | 公众号AppID（从&quot;获取公众号列表&quot;接口获取） |
| title | string | 是 | 文章标题（最多64字符） |
| content | string | 是 | 文章内容（支持Markdown或HTML） |
| summary | string | 否 | 文章摘要（最多120字符） |
| coverImage | string | 否 | 封面图URL |
| author | string | 否 | 作者名称 |
| contentFormat | string | 否 | 内容格式：markdown（默认）或html |
| articleType | string | 否 | 文章类型：news（普通文章，默认）或newspic（图文/小绿书） |

## 请求示例 (cURL)

```

curl -X POST https://wx.limyai.com/api/openapi/wechat-publish \

  -H &quot;X-API-Key: your-api-key&quot; \

  -H &quot;Content-Type: application/json&quot; \

  -d &#x27;{

    &quot;wechatAppid&quot;: &quot;wx1234567890&quot;,

    &quot;title&quot;: &quot;测试文章&quot;,

    &quot;content&quot;: &quot;# 标题\n\n这是文章内容...&quot;,

    &quot;summary&quot;: &quot;这是文章摘要&quot;,

    &quot;contentFormat&quot;: &quot;markdown&quot;

  }&#x27;

```

## 响应示例（成功）

```

{

  &quot;success&quot;: true,

  &quot;data&quot;: {

    &quot;publicationId&quot;: &quot;uuid-here&quot;,

    &quot;materialId&quot;: &quot;uuid-here&quot;,

    &quot;mediaId&quot;: &quot;wechat-media-id&quot;,

    &quot;status&quot;: &quot;published&quot;,

    &quot;message&quot;: &quot;文章已成功发布到公众号草稿箱&quot;

  }

}

```

## 响应示例（失败）

```

{

  &quot;success&quot;: false,

  &quot;error&quot;: &quot;公众号不存在或未授权&quot;,

  &quot;code&quot;: &quot;ACCOUNT_NOT_FOUND&quot;

}

```

## 错误码说明

| 错误码 | 说明 |
| --- | --- |
| API_KEY_MISSING | API密钥未提供 |
| API_KEY_INVALID | API密钥无效 |
| ACCOUNT_NOT_FOUND | 公众号不存在或未授权 |
| ACCOUNT_TOKEN_EXPIRED | 公众号授权已过期 |
| INVALID_PARAMETER | 参数错误 |
| WECHAT_API_ERROR | 微信接口调用失败 |
| INTERNAL_ERROR | 服务器内部错误 |

## 注意事项

1.  文章内容支持Markdown和HTML格式

1.  图片会自动上传到微信服务器

1.  发布后文章会出现在公众号的草稿箱中

1.  如果未指定封面图，会自动从内容中提取第一张图片作为封面

## 小绿书（图文模式）说明

当 articleType 设置为 newspic 时，发布为图文消息（小绿书）：

+   系统会自动从内容中提取所有图片（最多20张）

+   内容中必须包含至少1张图片

+   文字内容仅支持纯文本，最多1000字

+   不支持HTML标签和复杂格式

+   图片会自动上传到微信服务器

+   适合以图片为主的内容发布

## 发布示例（小绿书）

```

curl -X POST https://wx.limyai.com/api/openapi/wechat-publish \

  -H &quot;X-API-Key: your-api-key&quot; \

  -H &quot;Content-Type: application/json&quot; \

  -d &#x27;{

    &quot;wechatAppid&quot;: &quot;wx1234567890&quot;,

    &quot;title&quot;: &quot;小绿书测试&quot;,

    &quot;content&quot;: &quot;这是纯文本描述\n\n![图片1](img/b1dbc962540e2ad64977ccd0adb7874c.png)\n![图片2](img/f9a3eb64cd013bf3b549085dc98a80a5.png)&quot;,

    &quot;articleType&quot;: &quot;newspic&quot;

# 公众号与小红书发布，一次讲清

这次围绕 cc 的方案先做了确认，随后 cc 按需求完成交付。下面按“发布前约定—接口与页面—配置与验收—小红书方案”的顺序，把整条链路讲清楚。

```

key是【xhs_c93162d909fed820d422e7dc138bc505】`

```

cc 的回复如下：

```

`好的，我已经深入研究了所有相关代码。现在我为你设计完整的技术方案和实施计划。

⏺ 📋 技术方案设计

一、功能流程

用户操作流程：

1.  用户在发布管理页面点击"发布到公众号"按钮（每篇文章的操作菜单中）

1.  弹出发布对话框

1.  对话框自动加载公众号列表（调用获取公众号列表 API）

1.  用户选择：

+   目标公众号（下拉选择）

+   发布类型（单选：公众号文章 / 小绿书）

1.  用户点击"发布"按钮

1.  显示发布进度

1.  发布成功/失败反馈

二、技术实现方案

1.  组件架构

+   新建组件：components/WechatPublishDialog.tsx

+   使用 React Hooks 管理状态

+   对话框使用原生样式（与项目现有风格一致）

+   支持加载状态、错误处理、成功反馈

1.  API 设计

创建两个 Next.js API 路由作为代理：

API 1：获取公众号列表

+   路径：/api/wechat/accounts

+   方法：GET

+   功能：调用外部 API 获取公众号列表

API 2：发布文章

+   路径：/api/wechat/publish

+   方法：POST

+   功能：接收文章内容和配置，调用外部 API 发布

1.  环境变量配置

在 .env.local 中添加：

WECHAT_API_KEY=xhs_ccaa687fa4cf6d78fc0b1d366d6fed74

WECHAT_API_BASE=https://wx.limyai.com/api/openapi

三、需要改动的文件清单

新建文件（5个）：

1.  components/WechatPublishDialog.tsx - 发布对话框组件

1.  app/api/wechat/accounts/route.ts - 获取公众号列表 API

1.  app/api/wechat/publish/route.ts - 发布文章 API

1.  lib/wechat.ts - 微信 API 工具函数封装

修改文件（2个）：

1.  app/publish/page.tsx - 集成发布对话框（line 382: 修改"发布到公众号"按钮点击事件）

1.  .env.local - 添加微信 API Key 配置

四、详细改动说明

1.  WechatPublishDialog 组件功能

接口：

+   open: boolean - 对话框开关状态

+   onClose: () => void - 关闭回调

+   articleId: number - 文章ID

+   articleTitle: string - 文章标题

+   articleContent: string - 文章内容

状态管理：

+   公众号列表加载状态

+   选中的公众号

+   选中的发布类型（news / newspic）

+   发布进度状态

+   错误信息

1.  发布管理页面改动

+   位置：app/publish/page.tsx:382-391

+   改动：

+   添加对话框状态管理

+   点击"发布到公众号"时打开对话框

+   传递文章信息到对话框

1.  API 路由实现

+   使用 API Key 认证

+   错误处理和重试机制

+   响应格式统一化

五、数据流转

前端操作 → WechatPublishDialog

↓

调用 /api/wechat/accounts 获取公众号列表

↓

用户选择公众号和发布类型

↓

调用 /api/wechat/publish 发布文章

↓

后端代理调用 https://wx.limyai.com/api/openapi/wechat-publish

↓

返回结果给前端

↓

显示成功/失败提示

六、关键技术点

1.  内容格式处理：

```

草稿箱里的内容按 Markdown 存储；真正发出时必须明确传 `contentFormat: "markdown"`。若选择小绿书模式，还得先把图片抽出来，并对纯文本做处理。

```

1.  错误处理：

```

异常处理要覆盖四类场景：API Key 失效、公众号授权到期、网络请求异常、参数校验不通过。

```

1.  用户体验优化：

```

交互反馈也不能少：加载中有提示，发布时有进度；成功则自动关闭弹窗，失败则把具体错误展示出来。

```

七、安全考虑

1.  API Key 存储在服务端环境变量，不暴露给前端

1.  所有外部 API 调用通过后端代理

1.  输入参数验证和清洗

1.  错误信息脱敏处理

---

📂 文件结构预览

content-factory/

├── .env.local (修改)

├── app/

│ ├── api/

│ │ └── wechat/

│ │ ├── accounts/

│ │ │ └── route.ts (新建)

│ │ └── publish/

│ │ └── route.ts (新建)

│ └── publish/

│ └── page.tsx (修改)

├── components/

│ └── WechatPublishDialog.tsx (新建)

└── lib/

└── wechat.ts (新建)

---

✅ 下一步

请确认以下几点：

1.  功能流程是否符合你的预期？

1.  发布类型选择（公众号文章/小绿书）的 UI 设计是否满足需求？

1.  是否需要添加其他功能，例如：

```

可选项包括：挑选封面图、填写作者名、自定义摘要，以及定时发布。

```

1.  发布成功后是否需要更新文章状态（在 Draft 表中添加发布记录）？

确认方案后，我将开始实施代码修改。`

```

围绕 cc 给出的计划，先做了一次确认。

```

1.符合 2.满足 3.可以加上,选填 4.需

```

cc 随后完成需求并交付：

```

`✅ 完成！发布到公众号功能已全部实现

所有代码修改已完成并通过测试。以下是完整的实施总结：

---

📝 实施总结

一、新建文件（4个）

1.  lib/wechat.ts - 微信 API 工具函数

```

交付物主要有三块：拉取公众号清单、把文章推送到公众号、处理 Markdown 内容。

```

1.  app/api/wechat/accounts/route.ts - 获取公众号列表 API

```

拉取公众号清单走 GET 请求，调用外部微信 API，再把公众号列表返回给前端。

```

1.  app/api/wechat/publish/route.ts - 发布文章 API

```

推送文章走 POST 请求：先取出草稿内容，再请求微信发布接口，最后回写草稿的发布状态。

```

1.  components/WechatPublishDialog.tsx - 发布对话框组件

```

界面部分加入了公众号下拉选择、发布类型切换（公众号文章 / 小绿书），封面图、作者、摘要作为可选填写项，并展示发布状态。

```

二、修改文件（3个）

1.  prisma/schema.prisma - 数据库表结构

```

数据层补了三个字段：publishStatus（发布状态）、publishPlatform（已发布平台）、publishData（发布记录详情）；数据库迁移已经执行 ✅。

```

1.  app/publish/page.tsx - 发布管理页面

```

前端侧则导入发布弹窗组件，补上弹窗状态管理，改动“发布到公众号”按钮的处理逻辑，并接入发布成功后的回调。

```

1.  .env.local - 环境变量配置

```

配置项需要补两个环境变量：WECHAT_API_KEY 和 WECHAT_API_BASE。

```

---

🎯 功能特性

核心功能

✅ 公众号列表自动加载✅ 支持两种发布类型：公众号文章 / 小绿书✅ 文章内容自动提取（Markdown 格式）✅ 发布状态实时反馈✅

发布成功后更新草稿状态

可选功能（均为选填）

✅ 文章摘要（最多120字）✅ 封面图片 URL（留空自动提取首图）✅ 作者名称

智能处理

✅ 小绿书模式自动提取图片和纯文本✅ 自动检查图片数量（小绿书需至少1张）✅ 文字长度限制（小绿书最多1000字）✅ 封面图自动提取逻辑

---

📊 数据库更新

已成功创建迁移：20251102111629_add_publish_fields

新增字段：

publishStatus String @default("draft") -- 发布状态

publishPlatform String? -- 已发布平台 (JSON)

publishData String? -- 发布记录 (JSON)

---

🔧 使用方式

用户操作流程

1.  打开发布管理页面 (/publish)

1.  点击文章操作菜单 → 选择"发布到公众号"

1.  在弹出的对话框中：

```

使用时先选目标公众号（列表自动加载），再定发布类型（公众号文章或小绿书），最后按需填摘要、封面图和作者。

```

1.  点击"发布"按钮

1.  等待发布完成 - 显示成功提示

1.  文章自动添加到公众号草稿箱

发布类型说明

公众号文章（news）

+   支持 Markdown 格式

+   自动转换为富文本

+   支持图片自动上传

+   适合长文章

小绿书（newspic）

+   图文消息模式

+   纯文本 + 图片

+   最多1000字文本

+   最多20张图片

+   必须至少有1张图片

---

🚀 测试建议

建议按以下顺序测试：

1.  测试公众号列表加载

```

验收第一项：点“发布到公众号”按钮，看公众号列表是否正常出现，并核对公众号信息是否完整。

```

1.  测试公众号文章发布

```

然后选公众号，类型定为“公众号文章”，填好可选字段，点发布并观察反馈。

```

1.  测试小绿书发布

```

再找一篇带图的文章，类型切到“小绿书”，点发布看结果。

```

1.  测试错误处理

```

边界情况也要测：无图文章发小绿书应报错；网络异常、授权过期分别模拟一遍。

```

1.  验证数据库更新

```

发布成功后，确认草稿的 publishStatus 变为 "published"，publishPlatform 中含 "wechat"，并检查 publishData 是否记录了发布信息。

```

---

📌 注意事项

1.  API Key 安全：API Key 存储在服务端环境变量，不会暴露给前端

1.  公众号授权：如果公众号授权过期，会显示错误提示，需要重新授权

1.  图片处理：

```

图片会从 Markdown 中自动抽取；外部图片链接会自动上传到微信服务器，所以图床稳定性很重要。

```

1.  内容格式：

```

草稿内容应保持 Markdown 格式；发布时自动带上 contentFormat: "markdown"。

```

1.  发布记录：

```

每次发布都会刷新 publishData，里面记录公众号 AppID、materialId、mediaId、发布时间等信息。

```

---

🎉 大功告成！

所有功能已实现并就绪。你可以立即开始测试发布功能！

如有任何问题或需要调整，随时告诉我！`

```

实际效果可以直接看：点“发布到公众号”会弹出窗口，点发布后，对应内容就会出现在草稿箱中。

![](img/8c882b973d6d0e1d12ed7fb2c008e52d.png)

![](img/288b37dce9a6cd7fa49fd5ec00143e6d.png)

![](img/7adc7d5981d94a3725854f82b0a216dd.png)

### 2. 小红书平台发布：把文章转成图文的轻量做法

小红书这边真正的难点，是把一篇文章转成小红书图文。单独做一版小红书编辑器成本太高；如果时间允许，或者你的业务主阵地就是小红书，可以用 Claude Code 按具体场景做一个编辑器。更省力的办法是直接把文章里的插图抽出来当图片。

#### 2.1 先看视频教程

**视频点击下方链接即可学习（强烈推荐先看完视频后，再学习文字部分）：**

https://scys.com/view/docx/J4ETdEfOpo4P3kxAWQOcZJl7nWf#Qd0VdCvmDomYVwx4s9nczljHnje

#### 2.2 借助 Claude Code 接入小红书发布

访问下面网址注册 API：

https://note.limyai.com/dashboard/open/publish_note，激活码是：H64Q4VRD

完整调用提示词如下（注意把最后的密钥换成自己的！）:

Plain Text

```

`请你帮我修改发布管理这个页面，就是我希望能够实现用户如果去点击发布到小红书这个按钮的时候，

首先做的第一步就是要把这篇文章的所有的图文去分离出来，然后把文字清洗为纯文本，再调用第三方平台的接口。

这个接口的返回格式中会包含对应的发布的 URL 的链接，你需要把这个 URL 的链接去渲染成一个二维码，就是一个弹窗二维码，然后方便手机端去进行扫描。

接下来请你参考我提供给你的文档以及一些密钥的信息，去帮我完成这样的流程，主要是首先你可以帮我去进行技术方案上的这样的一个设计，请你务必要深入的研究分析所有这些相关的代码，然后把涉及到的变动的范围罗列出来。先不要着急去修改代码，确认完成之后和我去进行沟通，我们再去进行代码的变动，下面是文档：# 发布笔记 API 接口文档

## 基本信息

**接口地址：** POST https://note.limyai.com/api/openapi/publish_note

**Content-Type：** application/json

**认证方式：** API Key 认证

+   在请求 Header 中添加 X-API-Key 字段

+   示例：X-API-Key: xhs_da7d4437bfb5a55897d59a34c1fb4571e8ae684e9b702f5503af6d02b5eeec68

## 请求参数

Body 参数（JSON 格式）：

| 参数名 | 类型 | 必填 | 说明 |
| --- | --- | --- | --- |
| title | string | 条件必填* | 笔记标题 |
| content | string | 条件必填* | 笔记正文内容 |
| coverImage | string | 必填 | 封面图片 URL |
| images | array | 可选 | 正文图片 URL 数组 |
| tags | array | 可选 | 标签数组 |
| noteId | string | 可选 | 自定义笔记 ID |

**验证规则：**

+   title 和 content 不能同时为空，至少需要填写其中一个

+   coverImage 必填，不能为空

## 请求示例

```

```bash
curl -X POST https://note.limyai.com/api/openapi/publish_note \
  -H "Content-Type: application/json" \
  -H "X-API-Key: xhs_da7d4437bfb5a55897d59a34c1fb4571e8ae684e9b702f5503af6d02b5eeec68" \
  -d '{
    "title": "如何提升工作效率",
    "content": "今天分享5个提升效率的小技巧...",
    "coverImage": "https://example.com/cover.jpg",
    "images": ["https://example.com/1.jpg", "https://example.com/2.jpg"],
    "tags": ["效率", "职场"]
  }'
```

```

## 响应格式

### 成功响应（HTTP 201）

```

返回结构示例：

```json
{
  "success": true,
  "data": {
    "id": "550e8400-e29b-41d4-a716-446655440000",
    "note_id": "efficiency_tips_001",
    "title": "如何提升工作效率",
    "status_id": 1,
    "publish_url": "https://your-domain.com/publish/note?pub_id=...",
    "xiaohongshu_qr_image_url": "https://your-domain.com/api/xiaohongshu/qr?note_id=..."
  }
}
```

**10分钟技术调研：给选题分析页面加上“公众号文章抓取”**

最近产品提了个新需求：在选题分析页面里，除了用关键词拉文章，还得支持输入公众号名称，自动抓取该公众号当天最新发布的文章，并按相同维度做分析。系统里目前只有“关键词搜文章”的现成链路，所以得先摸清代码现状，再给出可落地的方案。

我让 cc 快速调研了一下，他大概花了 10 分钟就给出了完整的技术方案。

```

### 响应字段说明

| 字段 | 类型 | 说明 |
| --- | --- | --- |
| success | boolean | 请求是否成功 |
| data.id | string | 笔记唯一标识符（UUID） |
| data.note_id | string | 笔记 ID（自定义或自动生成） |
| data.title | string | 笔记标题 |
| data.status_id | number | 笔记状态 ID |
| data.publish_url | string | 笔记发布页面 URL |
| data.xiaohongshu_qr_image_url | string | 小红书二维码图片 URL |
| data.cover_image | string | 封面图片 URL |
| data.images | array | 正文图片 URL 数组 |
| data.tags | array | 标签数组 |
| data.created_at | string | 创建时间（ISO 8601 格式） |

## 错误码说明

| HTTP 状态码 | 错误码 | 说明 | 解决方案 |
| --- | --- | --- | --- |
| 401 | AUTH_ERROR | API密钥验证失败 | 检查 API Key 是否正确 |
| 400 | VALIDATION_ERROR | 参数验证失败 | 检查必填参数是否完整 |
| 409 | DUPLICATE_NOTE_ID | 笔记ID已存在 | 更换 noteId 或不传 |
| 500 | SERVER_ERROR | 服务器内部错误 | 联系技术支持 |

---

文档生成时间：2025/11/4 11:01:25

密钥信息为:【这里替换为自己的密钥！！】`

```
cc 给出的技术方案如下：

![](img/a1b326fefc1b6623d0faa56a6eb7f23c.png)
Markdown

```

`好的！我已经深入研究了所有相关代码，现在为你提供完整的技术方案和变动范围。

📋 代码分析总结

现有架构分析

1.  发布管理页面 (app/publish/page.tsx:125-140)

```
- 微信公众号发布功能已经做完了，用的是 WechatPublishDialog 组件
- 小红书发布按钮目前只是个模拟实现，代码在 389-398 行

```

1.  微信发布参考实现

```
- WechatPublishDialog.tsx：发布对话框组件
- lib/wechat.ts：API 工具库，里面有图文分离函数
- app/api/wechat/publish/route.ts：发布 API 路由

```

1.  图文分离工具 (lib/wechat.ts:128-160)

```
- extractImagesFromMarkdown()：从 Markdown 里提取图片 URL
- extractTextFromMarkdown()：把 Markdown 清洗成纯文本

```

1.  数据模型 (prisma/schema.prisma:68-86)

```
- Draft 表存草稿，content 是 Markdown 格式
- images 字段用 JSON 数组存图片

```

---

🎯 小红书发布技术方案

API 对接分析

接口信息

+   URL: https://note.limyai.com/api/openapi/publish_note

+   认证: Header X-API-Key: xhs_da7d4437bfb5a55897d59a34c1fb4571e8ae684e9b702f5503af6d02b5eeec68

+   Content-Type: application/json

请求参数

{

title: string, // 笔记标题（与 content 至少一个）

content: string, // 纯文本内容（与 title 至少一个）

coverImage: string, // 封面图 URL（必填）

images: string[], // 正文图片数组（可选）

tags: string[], // 标签数组（可选）

noteId?: string // 自定义笔记 ID（可选）

}

响应数据

{

success: true,

data: {

publish_url: string, // 发布页面 URL

xiaohongshu_qr_image_url: string, // 二维码图片 URL ⭐

// ... 其他字段

}

}

实现流程设计

用户操作流程

1.  用户在发布管理页面点击"发布到小红书"按钮

1.  打开 XiaohongshuPublishDialog 对话框

1.  用户可选配置发布参数（默认自动处理）

1.  点击"发布"按钮

1.  调用后端 API 处理图文分离并发布

1.  发布成功后显示二维码弹窗

1.  用户手机扫码完成后续操作

技术实现流程

前端点击 → XiaohongshuPublishDialog 组件

↓

调用 /api/xiaohongshu/publish (POST)

↓

从数据库获取 Draft → 提取图片和文本

↓

调用小红书 API (lib/xiaohongshu.ts)

↓

返回二维码 URL → 在对话框中显示二维码

---

📁 文件变动清单

1.  新建文件

✅ lib/xiaohongshu.ts (新建)

功能: 小红书 API 工具库

内容:

+   publishToXiaohongshu(): 发布文章到小红书

+   extractImagesFromContent(): 从内容中提取图片

+   cleanContentForXiaohongshu(): 清洗文本为纯文本

+   类型定义：XiaohongshuPublishParams, XiaohongshuPublishResponse

✅ app/api/xiaohongshu/publish/route.ts (新建)

功能: 小红书发布 API 路由

处理逻辑:

1.  接收 draftId 参数

1.  从数据库查询草稿

1.  图文分离（提取图片、清洗文本）

1.  调用小红书 API

1.  更新草稿发布状态

1.  返回发布结果（包含二维码 URL）

✅ components/XiaohongshuPublishDialog.tsx (新建)

功能: 小红书发布对话框组件

UI 结构:

+   发布参数配置区

+   发布按钮

+   二维码显示区（发布成功后显示）

+   状态提示（加载中、成功、失败）

1.  修改文件

✅ app/publish/page.tsx (修改)

修改位置: 第125-140行的 handlePublish 函数

修改内容:

// 修改前（第131-139行）：

else {

setPublishingArticle(articleId)

setTimeout(() => {

setPublishingArticle(null)

alert(成功发布到${platformConfig[platform].label}！)

}, 2000)

}

// 修改后：

else if (platform === 'xiaohongshu') {

// 打开小红书发布对话框

setSelectedDraftId(articleId)

setShowXiaohongshuDialog(true)

setShowDropdown(null)

}

新增状态:

const [showXiaohongshuDialog, setShowXiaohongshuDialog] = useState(false)

新增组件引用:

import XiaohongshuPublishDialog from '@/components/XiaohongshuPublishDialog'

// 在组件底部添加

{selectedDraftId && (

<XiaohongshuPublishDialog

open={showXiaohongshuDialog}

onClose={() => setShowXiaohongshuDialog(false)}

draftId={selectedDraftId}

onSuccess={handleXiaohongshuPublishSuccess}

/>

)}

✅ .env.local (修改)

新增配置:

# 小红书 API 配置

XIAOHONGSHU_API_KEY=xhs_da7d4437bfb5a55897d59a34c1fb4571e8ae684e9b702f5503af6d02b5eeec68

XIAOHONGSHU_API_BASE=https://note.limyai.com/api/openapi

1.  可能需要的数据库变更

考虑更新 prisma/schema.prisma

在 Draft 模型中，publishPlatform 和 publishData 字段已经支持多平台，无需修改。但建议在 publishData 中存储小红书相关信息：

{

"xiaohongshu": {

"noteId": "...",

"publishUrl": "...",

"qrImageUrl": "...",

"publishedAt": "..."

}

}

---

🔍 关键技术点

1.  图文分离逻辑

从 Markdown 提取图片

// 正则匹配:

![](img/3639f5eebada0e76e26c52ed4f056971.png)

const imageRegex = /![.?]((.?))/g

清洗为纯文本

+   移除图片语法

![](img/fed3267673a736c214b30ffb71ba21fb.png)

+   移除链接语法，保留文本 text → text

+   移除标题标记 ### 标题 → 标题

+   移除粗体/斜体 **text** → text

+   移除代码块

1.  二维码显示方案

方案 A: 使用 API 返回的二维码图片 URL（推荐）

![](img/ebb9e4653ea2c8dfaef0b131088249b5.png)

优点: 简单直接，无需额外依赖

缺点: 依赖外部图片服务

方案 B: 使用 publish_url 前端生成二维码

需要安装 qrcode 或 qrcode.react 库

1.  参数处理

封面图处理

+   优先使用用户指定的封面图

+   如果未指定，从 images 数组取第一张

+   如果都没有，从 content 中提取第一张

标签处理

+   从 Draft 的 keywords 字段获取

+   最多取 5-10 个标签

---

⚠️ 注意事项

1.  API 限制

```
- title 和 content 至少有一个
- coverImage 是必填项
- 建议限制文本长度，小红书一般有字数限制

```

1.  错误处理

```
- API 调用失败要做重试机制
- 草稿发布状态要能更新，包括失败状态
- 错误提示要友好，别让用户一脸懵

```

1.  用户体验

```
- 发布过程中要有 loading 状态
- 二维码要够大，方便扫码
- 提供“复制链接”功能作为备用方案

```

1.  环境变量安全

```
- API Key 只能在服务端用
- 千万别在前端代码里暴露

```

---

📊 预计工作量

| 文件 | 难度 | 预计时间 |
| --- | --- | --- |
| lib/xiaohongshu.ts | ⭐⭐ | 30分钟 |
| app/api/xiaohongshu/publish/route.ts | ⭐⭐⭐ | 45分钟 |
| components/XiaohongshuPublishDialog.tsx | ⭐⭐⭐ | 60分钟 |
| app/publish/page.tsx | ⭐ | 15分钟 |
| .env.local | ⭐ | 2分钟 |
| 总计 |  | 约 2.5 小时 |

---

✅ 方案优势

1.  架构一致: 完全参考微信发布的实现模式，保持代码风格统一

1.  可维护性强: 模块化设计，各部分职责清晰

1.  可扩展性好: 未来添加其他平台（抖音、B站等）可复用相同模式

1.  用户体验佳: 对话框交互、二维码扫描，流程顺畅

---

请您确认：

1.  这个技术方案是否符合您的需求？

1.  是否需要调整任何细节？

1.  确认后我们就可以开始实现代码了！`

1. 符合 2.不需要 请开始帮我实现代码!

![](img/c7846265999284e64d63c00da84bb05d.png)

这个任务较复杂，大概经过 20 分钟左右，cc 已经帮助我们完成并且给了完整的反馈和测试路径：

![](img/669306160ddd5d52114b714c1554e04d.png)

我们回到我们的系统，点击“发布到小红书”

![](img/d093462aaef002b34718ccab74967ef2.png)

我们直接使用小红书 APP 扫描生成的二维码，这时候可以看到这篇完整的笔记并且可以进行点击发布了：

![](img/4a78255ddcb6ff206bc3da24a5f73d45.png)

# 选修篇

# 一、实现监控指定公众号数据采集与分析

## 01.监控公众号数据

### 1.背景需求

在第一章的数据获取部分，我们实现了根据关键词获取文章并且进行分析，那能不能实现监控指定的公众号进行数据获取与分析呢？比如之前我们只能实现根据关键词获取公众号文章：

![](img/004bfc45d2293ab8a04ceda0c47af817.png)

现在我们希望获取指定公众号当天发布的文章，如何实现呢？我们先看下效果图：

![](img/a08a1771ffcab73d4fbbebf9e07a0c64.png)

点击开始分析后获取到当前公众号当天发布的所有最新文章并进行初步分析：

![](img/1cf7214e960aa5a11957c3a122c4f8c9.png)

![](img/e098a6ef13c67a6baf4544cf3fe3fb8e.png)

### 2.视频版教程

视频点击下方链接即可学习（强烈推荐先看完视频后，再学习文字部分）：

https://scys.com/view/docx/J4ETdEfOpo4P3kxAWQOcZJl7nWf#HgMhdd5fnoydzVxwn3QceBAznug

首先我们生成提示词

SQL

```

接着是公众号文章的获取接口，认证方式可以参考系统里现有的“根据关键词获取文章”接口。

请求方式：curl POST 到 `https://www.dajiala.com/fbmain/monitor/v3/post_condition`，`Content-Type: application/json`，请求体里带 `biz`、`url`、`name`、`key`、`verifycode` 这些参数。

返回的数据结构大致是这样：

```typescript
export interface ApifoxModel {
    /**
     * 状态码
     */
    code: number;
    /**
     * 消费金额
     */
    cost_money: number;
    data: Datum[];
    /**
     * 公众号头像(仅name作为参数名调用时显示)
     */
    head_img?: string;
    /**
     * 群发总次数
     */
}
```

有了这个接口，再结合现有代码里的 Markdown 提取、清洗和发布逻辑，整个功能链路就通了。接下来就是按上面的范围去改代码，重点留意接口鉴权、失败重试、字段校验这些细节，落地起来应该很快。

# 公众号发文接口字段速查：从群发次数到文章状态

做公众号数据对接时，字段一多容易看花眼。下面把发文记录相关接口的返回结构和单篇文章明细拆开说明，方便对照使用。

**返回结构里的整体信息**

- `masssend_count`：群发次数，数值类型。
- `mp_ghid`、`mp_nickname`、`mp_wxid`：分别对应公众号原始 ID、公众号名称和公众号 wxid。这三个字段只在以 `name` 作为参数名调用时才会返回。
- `msg`：消息内容。
- `now_page`：当前页码。单次发文最多包含 8 篇文章；普通账号每页返回 5 次发文，屏蔽搜索账号每页返回 10 次发文。
- `now_page_articles_num`：当前页的文章篇数。
- `publish_count`：发布总次数。
- `remain_money`：账户剩余金额。
- `total_num`：发文总次数，群发和发布都计算在内。
- `total_page`：总页数。普通账号按每天 5 次内容分页；屏蔽搜索账号按每天 10 次内容分页，但这类账号无法获取总页数，价格会高出 0.06。
- 结构末尾还保留了 `[property: string]: any`，说明可能附带其他扩展属性。

**单篇文章明细 `Datum`**

- `appmsgid`：文章消息 ID，数值类型。
- `cover_url`：文章封面地址。
- `digest`：文章摘要。
- `is_deleted`：删除标记，0 表示正常，1 表示已被删除。
- `item_show_type`：内容形态，0 图文、5 纯视频、7 纯音乐、8 纯图片、10 纯文字、11 转载文章。
- `msg_fail_reason`：文章被删除或违规的原因。
- `msg_status`：消息状态，2 正常，7 已被删除，6 表示文章因违规发送失败。
- `original`：原创标识，1 原创，0 未声明原创，2 转载。
- `pic_cdn_url_16_9`、`pic_cdn_url_1_1`、`pic_cdn_url_235_1`：三张不同比例的封面 CDN 地址，分别对应 16:9、1:1 和 2.35:1。
- `position`：文章在本次推送中的位置，从头条到八条。
- `post_time`：发文时间戳。
- `post_time_str`：适合直接展示的发文时间文本。
- `pre_post_time`：定时发文时间戳。
- `send_to_fans_num`：群发消息触达的粉丝数量；发布类文章或发送失败的文章，这个值为 0。
- `title`：文章标题。
- `types`：类型标识，9 代表群发，有通知且一天发送一次；1 代表发布，没有通知也没有次数限制。
- `update_time`：更新时间。
- `url`：文章链接。
- 这个结构同样支持 `[property: string]: any` 的扩展属性。

最后保留原始需求：

```

输入提示词后大概几分钟 cc 就给到了我们方案：

![](img/6c675d4c835c350d41c12e159e6fd635.png)

![](img/64becf5507f3b1d325308b62699a2746.png)

粗略看了一遍问题不大，我们让 cc 按照方案实现即可：

Plain Text

```
请你按照方案帮我实现
```

![](img/9a1156d7b0e46e5a922227fd0488eaac.png)

一般来说，我们新增功能只要把粒度拆解为上面这种大小，小步快跑，基本上 cc 都是可以一遍过的。

最终的效果就是我们刚刚演示的这样了。
```