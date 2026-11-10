先提醒一句：gen_id 的作用范围仅限于单个聊天窗口，换到另一个窗口就失效了。另外，若走 Dall-E3 API 出图，同样没法靠 gen_id 锁定同一角色——API 每次请求都是一次性会话，前后不互通。因此我放弃了写代码调 API 的路线，改在网页版里直接操作。

在 GPT 里也能这样用 gen_id，不妨试试下面这段提示词：

从现在开始，你的核心目标就是保持角色一致性。必须使用与上一张图像相同的提示和 gen_id 来制作相同角色的新图像，以保证人物一致，且能适配更多的表情、动态、服装与场景。做的好的话我给你 1000 美元小费。明白的话请回复明白。

提示词复制👉 https://gitee.com/tudoujunha/rpa-gpt/blob/master/prompt_genid.txt

当然，像眼前这种两个主体本身就是不同动物、外形差异很大的场景，若对一致性要求不高，完全可以直接用国内中转的 DALL-E3 API 来出图。

[PRE0]

以后想复用同一角色时，只要把对应的 gen_id 交给它即可。

[PRE1]

# 4.1.3.4 第四步：后期剪片

图片全部拖进剪映，给画面加上自动推近的缩放动效，基本就成型了。若想更贴近原片，再补一些音效和画面特效。这套流程只需跑通一次，下次直接找到剪映草稿里源图的存放位置，把图片替换掉再打开剪映，就能一键套用之前的剪辑效果，效率会高很多。

[PRE2]

BGM 方面，我用手机版 YouTube 自带的语音识别去搜对标视频里的音乐，找到源曲后再用工具下载。通常只需下载一个视频，下面这个站点基本覆盖各类自媒体平台：https://tiqu.cc/

不过这次我是把整套原创流程走了一遍，并非直接重绘图片，因此成片只和对标视频在故事层面相似，其余部分都不一样；声音方面我也没做更精细的打磨。说到底这还只是初版，视频创作仍有很大优化空间，故事脚本和剪辑特效都值得继续打磨。放到现在，还可以把 AI 视频加进来。

[PRE3]

[PRE4]

# 4.1.3.5 更多可参考账号

Cute Animals Story: https://wx.zsxq.com/group/1824528822/topic/1525442481188482

该账号 7 月 23 日上线首条视频，同样走 AI 动物故事路线，先用 shorts 起量，再转长视频开通 YPP 变现。shorts 更利于涨粉，而靠长视频攒够观看时长来开 YPP 则相对轻松。

[PRE5]

Meow Story: https://www.YouTube.com/@MeowStory1234

这个频道 8 月 21 日才注册，内容仍是 PPT 讲故事的形式，并未生成 AI 视频，却已经积累 10.9 万粉丝。

[PRE6]

Cat's Wonderland: https://www.YouTube.com/@CatsWonderland289

该频道 2024 年 7 月 23 日注册，主打 AI 视频生成的猫咪短篇故事。

[PRE7]

内容来源：《【生财技能】AI 动物故事视频复刻与批量生产》

[PRE8]

# 4.1.4 AI 怪物融合 @Gary @土豆君

# 4.1.4.1 参考账号案例

AI 短视频里有一类“融合怪”玩法，借助 AI 视频把两三种动物合成到一起，例如：

https://www.YouTube.com/hashtag/fusion/shorts

[PRE9]

[PRE10]

若想做融合怪视频，可以先参考下面几类对标账号。这里只是举例，具体选谁还要结合自身情况判断：

【第一类】动物融合，纯图片呈现，不借助 AI 生成视频：https://www.YouTube.com/@HeshanMalinda-nf6ws

[PRE11]

【第二类】动物融合，并用 AI 视频展示怪物融合的过程：https://www.YouTube.com/shorts/XU0yhFEnzrQ

[PRE12]

【第三类】人与动物融合：https://www.YouTube.com/@AnimolFacts/featured

【第四类】人与动物融合的达人秀风格，会混入一些达人秀视频剪辑：https://www.YouTube.com/@TalentSnap

[PRE13]

下面展示两个案例：左侧的参考视频靠纯图片生成，门槛较低，用 Dalle3 或 Midjourney 就能做出相近图片；右侧的案例多了一段融合过程，需要用到首尾帧视频生成。

[PRE14]

# 4.1.4.2 第一步：策划脚本

动物类型：选择与哪种动物融合变身

动作类型：设计具体动作，比如跳舞、转圈等

场景布置：确定视频发生的环境，例如舞台、户外等

服装配色：明确穿什么衣服、用什么颜色

这一步可以直接让 KIMI、GPT 等 AI 工具帮忙，把所需要素交给它们，让 AI 做排列组合即可。

[PRE15]

# 4.1.4.3 第二步：生成图片

总共要准备四张图，分别对应四个关键帧。制作时只需替换动作和人物形象相关的提示词，背景等部分保持不动。下面以我视频号那条千万播放视频为例，它在各平台数据都不错，应该有一定通用参考价值。

[PRE16]

1.

人物主体与动物主体出镜，动作不限

示例：full body，facing the camera，a breathtakingly beautiful 20-year-old woman in a very delegant white formal dress dress dance next to a big seal on brightly thick ice，barefoot，realistic，sunshine，bright，Slip dresses，ice and snow，long，blurred background，include as much detail as possible， ultra-high image quality， 4K，shot on canon a7c2 --no sexy --ar 9:16 --v 6.1

[PRE17]

2.

人物主体与动物主体出镜，动作依然不限，但最好与第一张相近或保持连贯，否则生成视频的效果会差很多

示例：参考上一条；在 Discord 里可以直接点对应按钮生成相似图片，V 几就表示基于第几张图来生成

[PRE18]

[PRE19]

3.

人物主体与动物主体，最好呈现拥抱或非常靠近的姿态，否则后续视频生成会很吃力

示例：full body，facing the camera，a breathtakingly beautiful 20-year-old woman in a very delegant white formal dress dress hugging a big seal on brightly thick ice，barefoot，realistic，sunshine，bright，Slip dresses，ice and snow，long，blurred background，include as much detail as possible， ultra-high image quality， 4K，shot on canon a7c2 --v 6.1 --no sexy --ar 9:16

[PRE20]

4.

融合后的主体最好保持站立姿态，这样更便于视频生成

示例：垫图链接 full body，facing the camera，a big tall seal in an elegant white dress stading on brightly thick ice，barefoot，realistic，sunshine，bright，Slip dresses，ice and snow，long，blurred background，include as much detail as possible， ultra-high image quality， 4K，shot on canon a7c2 --no sexy --ar 9:16 --v 6.1 --personalize hlfxj7l

[PRE21]

中途若遇到整体不错但细节崩坏的情况，比如手指或肢体错乱，可以点局部重绘按钮，在弹窗里框选区域后重新生成。

[PRE22]

[PRE23]

四张关键帧图片齐备后，就可以进入图生视频环节。

[PRE24]

# 4.1.4.4 第三步：图片转视频

这里用 Runway AI：左侧上传图片并填写提示词，右侧查看生成结果。整条视频共分四段。

[PRE25]

关键帧 1→关键帧 2：a beauty 【dance】 （on tiptoes） next to a 【XXX】，（bare feet），camera rolate，dynamic motion

圆括号里的内容是根据“踮脚”“光脚”等实际画面补充的提示词，按图片情况填写；方括号内是动作和动物主体，按需替换；加粗部分是针对镜头画面的全局提示，分别表示镜头旋转和动态画面，有助于稳定出图效果。遇到好用的动作种子记得保存，下次还能继续用。

1.

关键帧 2→关键帧 3：动作若有变化，把第一段里的动作词替换掉即可

2.

关键帧 3→关键帧 4：a beauty fuse with the XXX ，camera rolate to the right，dynamic motion。动作变化幅度大就补上变化后的动作，否则直接把原有动作替换成 fuse（融合）即可

3.

关键帧 4→跳舞：这一步只上传关键帧 4 这一张图，提示词写成 a XXX dance in a dress，camera follow，dynamic motion，描述越简单越好

熟悉上述流程后，提示词完全可以自己发挥，反复出图，直到凑齐 4 个满意结果即可。

也可以用即梦 AI 或可灵 AI 的“首尾帧视频生成”功能来完成。

目前即梦 AI 可免费生成且不用排队，更建议优先试试。

即梦 AI：

国内版：https://jimeng.jianying.com/

海外版（不推荐，目前功能不全）：https://dreamina.capcut.com/

可灵 AI：

国内版：https://klingai.kuaishou.com/

海外版：https://klingai.com/

下图中，左侧使用的是即梦 AI（视频模型 1.2），右侧则是可灵 AI：

[PRE26]

[PRE27]

先生成三张图片

第一张，生成美女与白马的画面

提示词：舞台上，一位美女和一匹白马并肩行走。

即梦 AI 会一次给出四张图，挑一张合适的即可。我这里选了第二张，欧美面孔。

[PRE28]

接着生成融合后的结果图，我同样选了第二张。

提示词：舞台上，一位长着马耳朵的欧美美女，身穿白色礼服，留着金色长发。

[PRE29]

这是融合前的图片，此处我用了参考图。

提示词：舞台上，一匹白马与一位穿白色礼服的欧美美女靠在一起。

[PRE30]

[PRE31]

2.

生成三段视频

先做融合过程的视频：

[PRE32]

再做融合前的视频：

[PRE33]

[PRE34]

最后做融合后的视频：

[PRE35]

[PRE36]

# 4.1.4.5 第四步：后期合成

保留对标视频的剪辑画面，只用剪映的基础功能即可。关键是对齐音乐卡点，时长尽量压在 18 秒以内。像惊讶一类的画面，可以用 AI 生成，也能从其他视频里截图；我这里直接保留了原视频画面。随后把 AI 生成的视频替换进去，沿用同一首音乐，成片就完成了。

[PRE37]

内容来源：《【生财技能】AI Shorts 两类视频复刻教程（怪物融合+动物跳舞）》、《24 天 7w 粉开通 YPP 收益 108 刀，我的 AI 达人秀变身千万播放视频制作流分享》

[PRE38]

# 4.1.5 AI 风格转绘 @龙

# 4.1.5.1 AI 转绘视频是什么？

所谓 AI 转绘视频，就是先用 AI 做出两张主体相同、画风不同的图片，再通过剪辑手法搭配魔性 BGM，制造强烈的反差感。这类视频会借剪辑让两张不同风格的图慢慢显露，勾起观众好奇，而且总时长很短，约 5 秒，所以完播率通常较高，观众平均会看 2 次甚至更多，播放量也能稳定在不错的平均线，平均每条起步约 1 万播放。

[PRE39]

下面是我实操的后台数据：单条视频时长 5 秒，观众平均观看时长达到 10 秒以上，相当于平均每人至少看了 2 遍。这类视频的爆款上限也不低，下面是两个对标账号的数据，其爆款视频基本都能冲到千万级播放。

[PRE40]

[PRE41]

其他对标账号的频道与视频数据（百万播放以上）都整理在下面的 Excel 里，已经帮大家采集好了。

[PRE42]

AI转绘对标数据.xlsx

这个赛道开通 YPP 同样可行，多数对标账号已经开通，少数没开的我也做了标注。

[PRE43]

[PRE44]

[PRE45]

[PRE46]

乍看之下，这个赛道制作简单、YPP 前景也不错，似乎是一片蓝海，但实际存在一个隐患：该赛道多数对标账号来自印度或印度尼西亚，开通 YPP 的账号里美国地区的很少。我自己的后台数据也显示，观众以印度用户为主。

[PRE47]

这就意味着，即便开通 YPP，收益可能也偏低。如果无法接受这一点，不妨换一个赛道。下面我就详细拆解这类视频的制作方法。

# 4.1.5.2 第一步：下载参考视频

先把对标账号的爆款视频下载下来，方便后续操作。这里有两种方式：

第一种，使用现成的在线 YouTube 下载站，免费且不限次数，效果尚可。可以直接把分享的 Excel 中“url”列的链接放进去，也可以打开想下载的对标视频，复制链接后粘贴过去。

第二种，我用 cursor 写了一个 Python 程序，支持从 Excel 批量导入视频链接并自动下载，打包好的软件已放百度网盘，可自行取用。

百度网盘链接：https://pan.baidu.com/s/1_zFUb72xeABeVpldlqambQ?pwd=xrmc