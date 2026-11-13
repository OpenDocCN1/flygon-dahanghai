# 6.3.2.1 短剧素材切片与字幕清理

下面这套流程，用剪映配合字幕提取和切分工具，把短剧素材处理成可用片段。按步骤走即可。

**Step1：复制主轨内容并合并副轨**

先在剪映里打开整部短剧，选中主轨全部视频按 Ctrl+C，再按 Ctrl+V 放到副轨。接着把副轨素材压成一个整体：全选副轨内容，右键选择“新建复合片段”。

[1.1.mp4](https://search01.shengcaiyoushu.com/upload/doc/SUYad816hofSjmxGHeWcbjoEnpc/IilUbNinloALaKxRlk8c1Ldinsf)

**Step2：给副轨加蒙版和模糊**

在副轨上挂蒙版，右上角进入“蒙版—镜面”，把蒙版的位置和粗细调到刚好盖住字幕。然后给副轨加模糊效果：从“特效—画面特效—基础—模糊”里拖到副轨上，模糊值设为 20 至 40。具体数值以两个效果为准：原字幕被遮住，同时无字幕区域的观看体验不受影响，在这个范围内微调。

[1.2.mp4](https://search01.shengcaiyoushu.com/upload/doc/SUYad816hofSjmxGHeWcbjoEnpc/GvXRbqPRMoHYVxxgT4YcqYLln1d)

**Step3：检查字幕是否全部遮住**

沿时间轴从头拖到尾，逐段确认副轨上的模糊蒙版有没有盖全字幕。若全部盖住，直接进入 Step4；若还有漏遮，先把这些片段从副轨切出来：选中副轨，播放头停在漏遮片段开头和结尾，各按一次 Ctrl+B（分割快捷键），再把对应蒙版的上下位置调好，然后继续 Step4。

[1.3.mp4](https://search01.shengcaiyoushu.com/upload/doc/SUYad816hofSjmxGHeWcbjoEnpc/SJWwbK9lboI3agxRvqLcddrvnxe)

**Step4：分段导出“模糊原字幕”视频**

先建文件夹“模糊原字幕”，再分段导出视频到里面。以 30 集为一段：播放头放到第 1 集开头按 I，放到第 30 集结尾按 O，用 I/O 把导出范围卡在 1-30 集，点右上角“导出”；导出设置选 720P、较低码率、24fps，目的是缩短剪映和后续软件的处理时间，文件命名为 01-30。Step3 里改过蒙版位置的片段，单独导出一次。

进阶做法：先选中副轨，把时间轴分别拖到 30 集和 60 集结尾，按 Ctrl+B 切成 1-30、31-60 两段；导出时只选中副轨 1-30 集那段，按 Shift+X 把范围锁定为 1-30 集，再点导出。

[1.4.mp4](https://search01.shengcaiyoushu.com/upload/doc/SUYad816hofSjmxGHeWcbjoEnpc/YdYtbaKbpoiMPYxENJxcrBAJnYg)

**Step5：导出“提取字幕”视频**

再建“提取字幕”文件夹，把副轨隐藏，导出目标改成“提取字幕”，再导一遍视频；这版视频留给后面提取字幕用。

[1.5.mp4](https://search01.shengcaiyoushu.com/upload/doc/SUYad816hofSjmxGHeWcbjoEnpc/WMmlb4K6woWQj7xi8oBcduy4n3T)

**Step6：用 VSE 提取硬字幕**

启动 VSE（硬字幕提取软件），从“提取字幕”文件夹里选文件，框好字幕识别区域，点开始识别。一般用快速识别模式，速度更快，约 20 分钟能识别 30 集合集，实际看电脑配置；代价是可能漏掉极少量字幕。漏字幕和个别错别字，可以在 Step7 精修时改，也可以等到后续用到问题片段时手动修。这样就把内嵌字幕转成了 srt 外挂字幕。也可换其他基于 OCR 图像识别的内嵌字幕提取工具，比如付费的 Videosrt Pro（性价比很高；VSE 跑不起来时可拿它替代 VSE 做这一步）。VideoSrt 开源地址：[`github.com/wxbool/video-srt-windows`](https://github.com/wxbool/video-srt-windows)。

[1.6.mp4](https://search01.shengcaiyoushu.com/upload/doc/SUYad816hofSjmxGHeWcbjoEnpc/JUhSbaQKeoIWZ5xq0kec7m2wnGg)

**Step7：精修字幕并导出**

建“精修字幕后”文件夹，把 VSE 得到的字幕和“模糊原字幕”里对应视频一起导入剪映。视频先做镜像。把字幕放到轨道上，注意字幕开头和视频开头对齐；调整字幕样式、字号和缩放，再把它挪到模糊蒙版遮住的位置。点任意一条字幕，在右上角字幕窗口看有没有过长字幕；若太长，在这条字幕最后的一两个字前按 Enter 回车键。最后导出精修后的视频和字幕文件：点右上角导出，在导出设置里勾选字幕导出。

[1.7.mp4](https://search01.shengcaiyoushu.com/upload/doc/SUYad816hofSjmxGHeWcbjoEnpc/TpvebEoFNoVJVzxhU5BckeTQnUf)

**Step8：按字幕分割素材**

打开大拍档剪辑助手（用来按字幕切视频的软件），进入素材裁剪器（APP—素材裁剪器），导入 Step7 精修后的视频；点“自动分割裁剪”，选“按字幕分割”，再选 Step7 生成的字幕文件，分割方式选一“用于文件名被搜索”，点“分割”；随后点右下角“裁剪设置”，保留默认设置并确定，导出切好的视频。新建“分割后片段”文件夹，把导出的视频移动进去。

[1.8.mp4](https://search01.shengcaiyoushu.com/upload/doc/SUYad816hofSjmxGHeWcbjoEnpc/CbfvbpbvooOWqEx0f2KcMEEwnAO)

按 Step1 到 Step8 走完，短剧素材的片段切分工作就完成了。