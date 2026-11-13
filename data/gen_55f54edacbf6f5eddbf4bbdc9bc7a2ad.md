# 视频链接别放附件字段

先给结论：视频生成接口返回的 MP4 网页地址，本质是一串 URL 字符，不是实体文件。所以多维表格里要用**文本字段**来接，不能拿“附件”字段硬塞。Fal.ai 等平台回传的是字符串，附件字段类型对不上，会直接报错，后面的自动化也会被卡住。

**字段配置操作**

把第三列原来的日期字段删掉，点表格第三列现成的【附件】，在字段类型列表里改成“文本”。这一步是根据 API 实际返回值（String 字符串）来配存储容器，避免容器类型错误让自动化运行失败。

字段名建议写成“视频链接”；当然不改、继续叫“附件”也可以。关键是把标签打清楚：这一列放的是可访问地址，用户点链接就能看内容。

点确认保存。这样后续自动化里的“修改记录”环节就有数据写入的位置。

注意：第三列该字段是文本，专门收集海螺或其他工具生成好的视频链接。

[PRE0]

## 2.2.4 获取 fal 平台海螺 API Key 的方法

**注意**：这一节覆盖完整 HTTP 节点配置，其中 fal 平台海螺 API Key 的获取最要紧。不过海螺 API 需要海外充值，为了降低大家充值门槛，工作流搭建环节我们改用云雾平台 API。你要是能搞定海螺 API 充值，就继续看下面的内容；如果充不了，直接跳到下一步工作流搭建继续学即可。视频里演示的节点 API 同样属于海螺 API。

**案例一：用多维表格工作流跑通流程**

在 AI Agent 节点下方点加号，选“发送 HTTP 请求”。这一步是建一个网络请求发射器，把上一步准备好的 Prompt 送到远程服务器。

[PRE1]

打开海螺地址（https://fal.ai/models/fal-ai/minimax/hailuo-02/standard/text-to-video），点 API，再点 HTTP（CURL）。下面会出现 submit a request，这段指令就是我们要填的请求。照着下面教的方式逐项对比，下次遇到类似请求就知道怎么填。

[PRE2]

请求方式设为 POST。因为要向服务器提交数据（Prompt）并创建新任务，这符合 RESTful API 规范。

URL 一栏放：https://queue.fal.run/fal-ai/minimax/hailuo-02/standard/text-to-video。它的作用是指定请求终点：调用 FAL.AI 的 Minimax Hailuo-02 模型，执行文字生成视频任务。

（纯文本）

[PRE3]

Headers 里新增一行：Key 填 Authorization，Value 写成“Key + 一个空格 + 你的 API_KEY”。这是身份验证环节，API Key 就是通行证，服务器据此判断你有没有权限发起请求、费用记在谁账上。注意 Key 和具体密钥之间通常要留一个空格。

（纯文本）

[PRE4]

这里用的是 fal 平台的海螺 API。获取 fal 平台海螺 API Key 的方法：

点官方链接 https://fal.ai/models/fal-ai/minimax/hailuo-02/standard/text-to-video

[PRE5]

用谷歌或 GitHub 账号登录。

[PRE6]

点这里的加号进入充值积分页面，选好金额后点 quick buy。

[PRE7]

按步骤创建你的 API Key。注意：这里的 Key 都是一次性的，创建后必须立刻粘贴保存，否则不会显示第二遍。

[PRE8]

[PRE9]

[PRE10]

[PRE11]

Request Body 选 Raw 格式（JSON），填入下面内容：

（纯文本）

[PRE12]

注意：JSON 里的“2。 AI Agent”部分，要点输入框右上角加号，选择“2。 AI Agent”节点下的“AI 回复内容（Output）”，不要手动复制内容。这一步是把上一节点生成的专业提示词封装成接口能看懂的 JSON 数据包发出去。

[PRE13]

Response Body 同样选 Raw 格式（JSON），把下面的示例代码复制进去。这是按 fal API 文档格式配置的示例返回结果，直接照搬即可：

（JSON）

[PRE14]

这一步是告诉飞书自动化系统：接下来预期的返回数据长什么样，方便后续节点准确识别和提取 response_url 等关键字段。不配置的话，后续节点可能引用不到返回数据。

[PRE15]

[PRE16]

## 2.3 工作流搭建

表格字段的基础建设完成后，就进入核心环节：搭建自动化工作流。它能让原本静态的表格具备处理复杂业务逻辑的能力。

### 2.3.1 创建工作流

这一步是进入自动化逻辑的可视化编辑界面，新建一张画布来绘制业务流程。选“从空白开始”而不是模板，是因为视频生成需求涉及特定第三方 API 调用和字段映射；空白画布配置自由度最大，也能避开模板预设逻辑的干扰。

操作：点屏幕左侧导航栏底部的工作流图标，然后在弹出的界面中心点“从空白开始”按钮。这样能得到一个干净的编辑环境，为后续添加触发器和执行动作做好准备。

[PRE17]

[PRE18]

### 2.3.2 配置触发器

这是个监听节点，专门接收用户在表格界面上的点击指令。触发方式选“点击按钮时”，是为了做成人工确认后再执行的机制：只有用户明确点了“生成”按钮，工作流才启动，从而精准控制 API 消耗、防止误触。

[PRE19]

操作：在触发器列表菜单里找到并选择“点击按钮时”。这一步等于告诉系统：启动信号来自用户点击，不是数据被动变化。

[PRE20]

进入配置详情页，把按钮类型设为“按钮字段”。在选择按钮字段所在的数据表下拉框里选中当前数据表，再在下方按钮列表中勾选“生成”（也就是 2.2.2 节配置的按钮）。这一步把触发器和具体按钮绑定起来，确保只有点击这一特定列的按钮，系统才能正确识别当前行数据上下文并启动流程。

选择按钮字段，选我们刚配置好的表格，同时选择“生成”那列字段去匹配按钮。

[PRE21]

[PRE22]

### 2.3.3 配置 AI Agent 节点

这是一个智能处理节点，把用户简短的创意扩写成包含丰富细节、光影和构图的专业 AI 绘画提示词。视频生成模型对提示词精度要求很高，直接用简单词汇生成，画面往往缺质感和逻辑；通过 AI Agent 做中间层优化和标准化，能明显提升最终视频生成质量。

[PRE23]

操作：在触发器节点下方点加号图标，在搜索栏输入并选择 AI Agent。这一步是引入一个具备自然语言处理能力的智能单元，作为连接用户输入与视频生成接口的“翻译官”。

[PRE24]

在输入指令（Prompt）编辑框里粘贴下方系统提示词，并在提示词中的主体位置点编辑框右上角加号，在弹出的“1。点击按钮时”菜单中选择“创意描述”（或“动物”）字段，然后保存。这样静态提示词模板和动态用户输入就融合了：每次生成的 Prompt 既符合固定场景构图要求，又能根据用户填写的不同动物做个性化调整。

注意：红框部分需要从右上角加号去添加（如下图所示）。

系统提示词模板（直接复制）：

（纯文本）

[PRE25]

[PRE26]

[PRE27]

[PRE28]

### 2.3.4 发送生成视频的请求

这是一个发送 HTTP 请求节点，用来调用 yunwu 平台的 veo3 模型接口（https://yunwu.ai/register?aff=zUII），正式发起文生视频任务。飞书本身没有视频生成能力，必须通过标准化 API 协议与外部专业 AI 视频生成服务通讯。

注意：这里的图文内容示范如何用云雾平台 API 完成 HTTP 节点配置，具体推荐先看视频学习：云雾平台 API 配置 + 节点配置（补录学习）。

[PRE29]

操作：在 AI Agent 节点下方点加号图标，选择“发送 HTTP 请求”。这一步是创建一个网络请求发射器，把上一步准备好的 Prompt 发给远程服务器。

[PRE30]

这是刚才提到的 yunwu 平台接口文档。选择“创建视频”，再选 Shell。下面会出现请求示例代码，这段指令就是我们要填的请求。大家可以按下面教的方式对比请求里的内容，下次就知道这类请求怎么填。

[PRE31]

请求方法选 POST。因为要向服务器提交数据（Prompt）并创建新任务，符合 RESTful API 规范。

URL 填：https://yunwu.ai/v1/video/create。这一步是指定请求目标终点：调用 yunwu 的 Veo3 模型，执行文字生成视频任务。

（纯文本）

[PRE32]

Headers 部分点添加：Key 填 Authorization，Value 填“Key + 一个空格 + 你的 API_KEY”。这是身份验证环节，API Key 是通行证，告诉服务器你有权限发起请求、费用记在谁账上。注意 Key 和具体密钥之间通常需要一个空格。

（纯文本）

[PRE33]

[PRE34]

这里用到的是 yunwu 平台的 API Key。获取 yunwu 平台 veo3 API Key 的方法：

点官方链接 https://yunwu.ai/register?aff=zUII ，登录后点右上角“API 令牌”。

[PRE35]

点 1 的位置进入充值页面充值；点 2 的位置创建自己的 API Key。

[PRE36]

Request Body 选 Raw 格式（JSON），填入以下内容：

（纯文本）

[PRE37]

注意：JSON 里的“2。 AI Agent”部分，需要点输入框右上角加号，选择“2。 AI Agent”节点下的“AI 回复内容（Output）”，而不是复制的内容。这一步是把上一节点生成的专业提示词封装成接口能看懂的 JSON 数据包发送出去。

[PRE38]

Response Body 同样选 Raw 格式（JSON），把下面的示例代码复制进去。这是按 fal API 文档格式配置的示例返回结果，直接照搬即可：

（JSON）

[PRE39]

响应示例中的英文画面描述如下：

> A surreal and whimsical digital painting of a majestic brown cow with large, feathered wings soaring gracefully through a vibrant blue sky. The cow has a joyful expression, its tail streaming behind it as it flies among fluffy white clouds. Below, a patchwork of green farmland stretches into the distance, with tiny farm buildings and a group of astonished farmers looking up in amazement. The scene is bathed in warm golden sunlight, creating a dreamlike and magical atmosphere. Art style inspired by fantasy illustrations with soft brushstrokes and rich, saturated colors.