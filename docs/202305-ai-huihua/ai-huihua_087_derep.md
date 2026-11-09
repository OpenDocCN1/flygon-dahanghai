# 5.7.3.2 安装包下载与准备

这套 LoRa 训练工具没有可视化界面，操作起来反而让人觉得干净利落。

我们要下载的 LoRa 解压包出自 B 站 UP 主 [秋葉 aaaki](https://space.bilibili.com/12566101)，他提供了三个下载渠道：

- 夸克网盘：[pan.quark.cn/s/d81b8754a484](https://pan.quark.cn/s/d81b8754a484)
- 百度网盘：[pan.baidu.com/s/1WMjja4uHB9tkZoBvgmm_ZA?pwd=lora](https://pan.baidu.com/s/1WMjja4uHB9tkZoBvgmm_ZA?pwd=lora)，提取码：`lora`
- GitHub：[github.com/Akegarasu/lora-scripts](https://github.com/Akegarasu/lora-scripts)

把压缩包拉下来后，你会看到三个文件：

![](img/5575b130df1e9e3d84efda3c328c4790.png)

简单说明一下各自的用途：

- 第一个压缩包是训练主程序，需要先解压；解压位置随意，但路径里尽量不要出现中文。
- 第二个是文本编辑器，方便你直接修改训练相关的文本配置。
- 第三个是 Python 安装包，原作者建议的版本是 3.10.8。

接着按下面几步操作。

① 安装 Python 环境

直接用刚才下载的 Python 3.10.8 安装包，双击运行即可。在安装界面左下角，`addPython.exe to PATH` 这个选项务必勾上，它是用来配置环境变量的。然后按顺序点击数字 1、2 开始安装；安装结束后，点击箭头指示的位置，再点 `close` 收尾。

![](img/1339330ed58fd689e38b912996fe43ab.png)
![](img/a477e7ebaafb9f546e3f702b06924aaf.png)

② 关闭 PowerShell 签名校验，并确认 Python 装好了

先打开命令行窗口（黑色终端），打开方法如下：

![](img/691d9439637dd74fdecad4a9dcc5493d.png)

③ 在终端里执行这条命令，作用是取消 PowerShell 脚本签名校验：

`Set-ExecutionPolicy -ExecutionPolicy RemoteSigned`

![](img/cfecae854ab23b84be75de8f4afced69.png)

执行完后，接着输入 `python` 回车，只要能正常显示版本信息，就说明 Python 已经 OK。这个窗口随后可以关掉。

④ 配置 Notepad 文本编辑器

按下面的图示依次操作即可：

![](img/9df5c5c9c2e4ec01970b82f3519ca689.png)
![](img/168543e5445c1ae7d0e04ae5bc190a46.png)
![](img/c5a06ef1261cb08a5943ae5aa30b8883.png)

⑤ 更新主程序文件

![](img/ca5308c69d1fd53ea8e89a17d218ddf0.png)

⑥ 用 PowerShell 运行依赖安装脚本

执行 `install-cn.ps1`，把所需的依赖文件装好：

![](img/c52261d8d15b843fe13a8fe227b39e9d.png)
![](img/7c8534dfa2fbddd1d0ac5f7a5b1be7a9.png)