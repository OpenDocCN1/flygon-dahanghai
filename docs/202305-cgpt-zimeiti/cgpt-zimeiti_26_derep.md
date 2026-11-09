# 4.1.4 角色 Prompt 没头绪？两招帮你快速搞定

新手想独立写一份好用的人设 Prompt，通常会卡在无从下笔。与其硬想，不如借助外部工具。下面分享两种可行路线。

（一）用自动生成服务搭初稿

AICosplay 是一套基于 ChatGPT 的在线生成工具，根据你给出的关键字或一小段描述，就能自动构建一段人设 Prompt。

输出内容偏向“我是谁、我要做什么”，也就是身份和任务部分，但通常缺少行为边界，需要你自行补充约束条件。

想要结果更贴合预期，可以在请求里补充更多限定条件。比如把“会议纪要助手”扩写为“按待办事项输出会议纪要的助手”，效果会明显不同。

第一轮不满意就多试几次，把多次生成的结果合并起来做调整。

另外，由于要兼容不同角色，AICosplay 生成的内容里会带一些多余字段。参考时删掉用不上的即可。

入口：role.aicosplay.com.cn/zh?f=scys

![](img/40a07f1ce4421e1f0f4c486540803e1a.png)

（二）套用现成的人设资源

这里再分两条路。

第一条路：Awesome-ChatGPT-Prompts

GitHub 上已有开发者把各类人设整理成公开仓库，可在这里获取：github.com/f/awesome-chatgpt-prompts。

![](img/dcc7282e2fd6879dc31c42da4b8c3d9f.png)

相中哪类人设，直接把对应的英文 Prompt 贴进对话窗口即可。

因为仓库内容是英文，AI 的回复也会是英文。想换回中文，在提问时附带一句“用简体中文回复我接下来的问题”即可。

![](img/9f7fabcb83b0395a0580ed7cb45b14f8.png)

这样，这套 AI 就会以对应领域专家的口吻输出内容，专业度自然上来了。

英文不好的朋友也不用慌，我们另备了一份中文版，叫《ChatGPT 身份指令关键词》，用法和上面相同。

![](img/ec5fd537eaf338bc452d49b5518a1a44.png)

第二条路：非官方 ChatGPT 客户端

有开发者把上面那套 Prompt 资源封装成了 App，装好后在对话窗口里直接输入“/”，就能唤起人设列表。

操作流程：

1. 进入 github.com/lencx/ChatGPT/releases，按系统选版本。下面以 Mac M1 为例：

![](img/6a3f2759fba173092231d2242110971b.png)

2. 下载并安装，然后打开“访达”→“应用程序”，启动 ChatGPT。

![](img/49e2f3aefb0811d32c37064b4eab78a4.png)

3. 登录账户，在左上角“preference”菜单中进入“Control Center”。

![](img/f59119e1a5b0b11b3c2734a5c41dc093.png)

4. 前往“Language Model”区域，开启“Sync Prompts”并按下“Sync”按钮，即可完成同步。

![](img/d01ec04b8fb152e05865c2b518d205b4.png)

![](img/9138777647070c350bd317b15df7c651.png)

5. 同步结束后，回到对话窗口输入“/”，会看到多出许多人设选项。

挑一个需要的角色，直接对话即可。

![](img/1ea8dfe007380902410edd21ef04c5de.png)

目前，围绕 Prompt 生态的插件也层出不穷。这里推荐两个口碑不错的项目，感兴趣不妨一试：

• FlowGPT: Amplify your workflow with best prompts（https://flowgpt.com/）
• Get the most out of AI.（https://www.aiprm.com/）

![](img/6ee508850b27e2c7d179da2f3eea659e.png)