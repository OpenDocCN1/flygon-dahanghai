# 5.8.1.2 插件下载全攻略

给 Stable Diffusion 装插件，常见做法有三条路，下面分别说明。

**在 WebUI 界面里下载**
界面中提供了两个入口：
![](img/86a8f46bec0cf6b20d249c9922cea57c.png)
可用插件
![](img/12a994c0aee613bf33570dceb9717ae6.png)
从网址直接装

**用 Git 手动拉取**
前提是电脑上已装好 Git 工具。点开后会弹出黑色命令行窗口，按顺序执行：
输入 `cd ..` 回车；
输入 `cd extensions` 回车；
输入 `git clone XXXXX.git` 回车；
等待下载完成即可。
注1：上面的 XXXXX 指你要安装的插件地址。
注2：通过 Git 安装的好处是，后续插件更新会更方便。
![](img/cab94c2790f2a2b1d0447041f1fcaaab.png)
示例：
![](img/7d139d3c451d672e355b8010c3d3c2c4.png)

**解压 zip 包**
这种方式不太推荐，因为以后更新插件会比较麻烦。
操作步骤：从网站下载插件压缩包，解压到 Stablediffusion 根目录\extensions 文件夹内，重启后就能使用。
![](img/af4f5e3bb11246407ad66665c9fe757e.png)
![](img/e12d1c8b9f4ffdf6c4edf913cceed533.png)