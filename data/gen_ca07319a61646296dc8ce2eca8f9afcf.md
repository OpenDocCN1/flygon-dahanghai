# 2.3.3 用 Code 节点统一数据格式
[PRE0]
[PRE1]

做数据清洗时，Code 节点的任务是把输出格式拉齐。代码可交给 AI 生成，提示词这样写：先把上一步的结果复制下来，再粘贴给 Claude。操作上仍然点右侧“+”，输入“Code”，再把它与 GNewsAPI 节点连接。
[PRE2]
[PRE3]
[PRE4]
GNewsAPI 的清洗同样用 Code 节点，但这里不能直接套用上一段代码：GNewsAPI 返回的数据结构与 NewsAPI 不同，必须让 Claude 重新生成。生成后的代码块在下方表格中可直接复制。参数这样设：Mode 选 Run Once for All Items，表示一次性处理所有项目；Language 选 JavaScript，也就是用 JavaScript 语言。
[PRE5]
[PRE6]
[PRE7]
# 2.4 合并两路数据：Merge 节点

点“+”，输入 Merge；把“Input1”与“Code”连接，“Input2”与“Code1”连接。
# 2.4.1 这个节点解决什么问题
清洗后的数据需要合并。上一步虽然分成两条分支，但并不会同时产出两组数据，实际始终只有一组。原因是 NewsAPI 要么成功、要么失败：成功时直接输出数据，不经过 GNews 节点；失败时输出为空，流程才走到 GNews 节点并拿到结果。问题在于，NewsAPI 与 GNewsAPI 的结果在 n8n 中属于两组不同变量；为了让它们变成一组变量，才用 Merge 节点做合并。
# 2.4.2 节点怎么设置
[PRE8]
参数设置：Mode 选 Append，即添加节点；Number of Inputs 设为 2。
# 2.5 清理空值：Filter 节点

点“+”，输入 Filter，并与 Merge 节点连接。
[PRE9]
[PRE10]
# 2.5.1 Filter 的作用
这一步用来过滤数据。测试时发现，有些单元格返回的内容为空，而空值并不是我们想要的。Filter 节点能剔除空值，只保留非空值。
# 2.5.2 Filter 配置步骤
先点“Execute Workflow”测试前面的工作流；如果一切正常，会得到类似下图的 INPUT。有了测试结果变量，再继续配置节点。
[PRE11]
把上一节点的 output 结果作为本节点 input，并把模式改成“schema”。
[PRE12]
按住“新闻链接”按钮，拖到右侧输入框；其余四个变量也依次拖入不同输入框。
[PRE13]
确保值存在：点击“exists”，鼠标悬停在 String 上点击“exists”，剩余变量同样设置。
[PRE14]
这里要求所有变量都存在，所以选择“AND”，取交集。
[PRE15]
[PRE16]
# 2.6 翻译并结构化：AI Agent 节点

点“+”，点“AI”，再点“AI Agent”，与 Filter 节点连接。
[PRE17]
[PRE18]
[PRE19]
# 2.6.1 为什么要加 AI Agent
走到上一步，其实已经可以把内容写进飞书多维表格。但由于信息源以英文为主，这里加一步 AI Agent 做中文翻译，并保证内容按结构化方式输出。
# 2.6.2 AI Agent 配置
先设置提示词。
[PRE20]
参数：Source for Prompt(User Message) 选 Define below，即自定义提示词；Prompt 填“翻译成中文，并按照制定格式输出”；Require Specific Output Format 打开，让输出遵循特定格式。注意仍要把模式改成“schema”，再按住鼠标拖到 Prompt 中。
[PRE21]
[PRE22]
模型选择：这里以 DeepSeek 为例。第一步，点“chat model”，选“deepseek chat model”。第二步，点“Credential to connect with”：如果之前在 n8n 里配置过 Deepseek account，直接选择即可；没有就点“Create new credential”。
[PRE23]
第三步，输入 API KEY 后保存。API KEY 的获取方式可参考前面的案例：进入 DeepSeek 官网 https://platform.deepseek.com/api_keys，点右上角 API 开发平台，可以先充 10r 测试。想接入任何大模型，基本都要找到它的开发平台页面，进入 API 调用板块，创建一个 key，再复制到 n8n。
[PRE24]
创建 API key，复制后粘贴到 n8n 中。
[PRE25]
输出格式：由于后续要以固定格式写入飞书，翻译完成时也要按固定格式输出。第一步，点“Output Parser”，选择“Structured Output Parser”。
[PRE26]
第二步，选择“Generate From JSON Example”，输入下面的 JSON 格式，并打开“Auto-Fix Format”。
[PRE27]
[PRE28]
[PRE29]
第三步，按第一步的方式再选择一个大模型，这里仍选 DeepSeek。
[PRE30]
[PRE31]
# 2.7 写入飞书：feishu-node 节点

准备阶段已经添加过 feishu 节点，所以直接搜索 feishu，点击“多维表格 新增记录”即可添加。
[PRE32]
[PRE33]
[PRE34]
# 2.7.1 节点作用
把 AI 资讯写入飞书多维表格。
# 2.7.2 节点设置
第一步，点“Credential to connect with”：如果之前在 n8n 中配置好 feishu account，直接选择；没有就点“Create new credential”。
[PRE35]
[PRE36]
第二步，Base URL 填“open.feishu.cn”；Appid 填准备阶段飞书自建应用的 AppID；AppSecret 填准备阶段飞书自建应用的 AppSecret。

第三步，回到节点页面，【Resource】选【多维表格】，【Operation】选【新增记录】。多维表格 token：回到多维表格 URL，“base”后、“？table”前的内容就是 token。
[PRE37]
多维表格 ID：“table=”后、“&view”前的内容就是 ID。
[PRE38]
第四步，填写请求体 JSON：
[PRE39]
到这里，这个 n8n 工作流就搭建完成了。点击“execute workflow”，等待运行结束，回到多维表格就能查看运行结果。
[PRE40]
[PRE41]
[PRE42]
# 3. 第三部分：直接拖动 JSON 文件快速搭建工作流

# 3.1 导入已经配置好的工作流
把文件下载后导入，或直接复制代码到 n8n 面板粘贴；打开 n8n，在右上角选择新建工作流，然后运行即可。JSON 文档