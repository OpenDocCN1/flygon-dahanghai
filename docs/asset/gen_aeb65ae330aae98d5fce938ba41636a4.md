[PRE0]

视频里用到的音效，可以按画面内容和自己的审美来搭：环境白噪音、狗叫、狗委屈叫、狗着急叫、狗舔舐声、拉布拉多玩耍声、汽车喇叭、汽车刹车、汽车发动机怠速声、浪花拍打声等。成片色彩也能根据表现去调，最后以4K 60帧导出。

# 4.1.5.5 提示词模板化，出图更稳

# 4.1.5.5.1 拆开提示词，做一个能复用的模板

为了提升出图效率、减少反复抽卡，我借助GPT和DeepSeek做过优化，把分镜头的文生图提示词拆成几个模块：主体描述、环境描述、镜头语言、图片质量。比如：

一只拉布拉多站在乡间公路上，

back to the camera,

米白色的皮毛，俊美的外表

The 拉布拉多 is facing a 橘黄色轿车 approaching the camera，

the 橘黄色轿车's front headlights turned on and clearly visible。

这条路右边是高大的岩石峭壁，左边是草原和苔藓

天空下着毛毛雨，蓝色的天空，夏天的季节

focusing on the 拉布拉多's back and the 橘黄色轿车's front。

Natural light enhances realistic details.

照片视角是从人站立的高度拍摄的，中距离镜头拍摄

The image is in cinematic composition, realistic style, ,Film Photography,4k quality,

其中，主体部分是绿色和红色内容，环境模块是黄色内容，剩下的是镜头语言和画质设定。

前期建议中英文混写来制作提示词模板。全英文容易分不清哪些是主体描述、哪些是环境描述；另外翻译软件对特定词尤其镜头语言的中译英不稳定，每次可能翻得不一样，导致只能靠特定词触发效果的图片总出不来想要的效果，所以直接用英文固定住，减少翻译错误。中英混合的好处是：能避免翻译错误带来的无效抽卡，抽卡概率明显降低，我基本一遍过，偶尔也会遇到变形问题；相比之前纯中文提示词，抽卡次数少了很多。

同理，狗狗从窗外向车内观看的提示词：

Shot from inside a car,

outside the car window is a 德国牧羊犬，

the 德国牧羊犬 is close to the glass，

gazing inside the car, the glass is clear with faint reflections,

outside is a 温馨的农场的自然环境，

focus on the 德国牧羊犬's face"

slightly blurred background, realistic details, Film Photography,4k quality,

[PRE1]

同理，后续分镜也能用同样方法做成固定模板。有了固定镜头模板，后续创作只需替换汉字部分，也就是主体和环境；镜头和画质部分保持不变。这样能提高生图速度、减少抽卡次数。

分镜1：动物拦车

# 💡

一只 [动物] 站在乡间公路上，

back to the camera,

[外貌特征] 保持角色一致性

The [动物] is facing a [车辆] approaching the camera，

the [车辆] 's front headlights turned on and clearly visible。

这条路右边是 [环境] ，左边是 [环境 2] 主要为后续灾难做适应性对照

[天气描述] 调节图片整体色彩构图

照片视角是从人的站立的高度拍摄的，中距离镜头拍摄

focusing on the [动物] 's back and the [车辆]'s front。

Natural light enhances realistic details. （自然光增强了逼真的细节）

The image is in cinematic composition, realistic style, ,Film Photography,4k quality,

分镜1样张：

A white moose stands on a rural road,

back to the camera,

white fur Huge antlers, domineering appearance

The moose is facing a dark green car approaching the camera,

The dark green sedan's front headlights turned on and clearly visible

On the right side of this road are tall rocky cliffs, and on the left side are grasslands and mosses

Blue sky, summer season

The photo perspective is taken from an individual's standing height, with medium range shots taken

Focusing on the white moose's back and the dark green sedan's front

Natural light enhances realistic details

The image is in cinematic composition, realistic style, ,Film Photography,4k quality,

分镜2、3：动物出现异常动作

# 💡

Shot from inside a car,

outside the car window is a [动物]

白色的皮毛。巨大的鹿角，霸气的外表

the [动物] is close to the glass，

gazing inside the car, the glass is clear with faint reflections,

outside is a [其中一侧环境]

[同步分镜一天气描述]

focus on the [动物]'s face"

The image is in cinematic composition, realistic style, ,Film Photography,4k quality,

分镜样张：

Shot from inside a car,

Outside the car window is an albino moose

White fur Huge antlers, domineering appearance

The albino moose is close to the glass,

gazing inside the car, the glass is clear with faint reflections,

Outside is a primitive forest with thick trunks

Blue sky, summer season,

Focus on the face of the albino moose

The image is in cinematic composition, realistic style, ,Film Photography,4k quality,

分镜2、3：动物出现异常动作

# 💡

驾驶员视角透过 [车辆] 挡风玻璃的极端特写，画面最底部边缘隐约可见方向盘，

一只[动物]站立在 [车辆] 前的公路上，

白色的皮毛。巨大的鹿角，[动物]脸部占据画面 60%，唾液滴在引擎盖上，张开嘴巴，有口水流下来，

右边高大的岩石峭壁，左边是草原和苔藓，

[同步分镜一天气描述]

The image is in cinematic composition, realistic style, ,Film Photography,4k quality,

分镜样张：

Through the extreme close-up of the dark green car windshield from the driver's perspective, the steering wheel can be vaguely seen at the bottom edge of the image,

A white skinned Rangifer Taranduss stands on the road of a dark green sedan,

White fur The huge antlers of the albino reindeer occupy 60% of the screen, and saliva drips onto the hood. Opening its mouth, saliva flows down,

On the right is a tall rocky cliff, and on the left is grassland and moss,

Blue sky, summer season,

The image is in cinematic composition, realistic style, ,Film Photography,4k quality,

照着这个思路，分镜4的灾难或动物救治（救治时要让动物呈现病态），分镜5的人与动物友好互动（抚摸、拥抱；若是救治，要展示包扎后的动物形象），也能整理成一套经过验证的模板。

# 4.1.5.5.2 模板要改，别和对标一模一样

即使有了固定镜头模板，实际创作仍会做变化。截图对标账号的分镜图再图生图当然可以，但容易被原作者刷到后一眼认出，可变性也偏弱。有时只需微调分镜，表达同样的意思，又能和对标视频区分开。

比如拆解动物示警后，通用模板是：

分镜一：动物拦车

分镜二、三：动物异常举动

分镜四：灾害发生

分镜五：人与动物接触互动

我们保留关键分镜，在意思不变的前提下略作调整。比如分镜二、三表现动物异常举动，可以改动物动作、动物与车互动的相对位置、镜头视角（车内向外拍，还是车外后视图等）。不同视角效果不同，但整体仍表达动物想用异常行为示警。

自然灾害镜头则按前面提示词里的环境描述来定，如山体滑坡、泥石流、巨石坠落、桥梁崩塌、地面塌陷、猛兽出没等，可灵活变换。其次，修改提示词让动物示警变成动物自救、动物救援等，就能切换赛道。只要拆解出视频思路，分镜头就很好处理。

内容来源：《YT shorts 复盘——动物赛道的爆点因子分析及提示词模板》

[PRE2]

# 4.1.6 AI 转绘玩法 @龙

# 4.1.6.1 AI 转绘类视频怎么理解？

AI转绘类视频，就是用AI生成两张主体一致但风格不同的图片，再借助剪辑和比较魔性的BGM制造反差。先看三个案例，能更直观感受特点：

Evolution of Cat Motor Sports Cow Maiw Milky cat cute love shorts720p.mp4【在线播放】

这类视频靠剪辑让两张风格不同的图片慢慢显现，勾起观众好奇心，且总时长很短（约5秒），所以完播率通常较高，观众平均会看2次及以上，播放量能维持在不错的平均水平（平均每条视频1w播放起步）。

[PRE3]

这是我实操的后台数据：每条视频5秒，观众平均观看时长10秒及以上，也就是平均观看次数至少2次及以上。

这类视频的爆款上限也高，下面两个对标账号的数据显示，爆款视频基本能到千万级别。

[PRE4]

这个赛道开通YPP也没问题，大多数对标账号已经开通YPP，没开的我也列了一个。

[PRE5]

[PRE6]

[PRE7]

看上去这个赛道制作简单、开通YPP前景好，像蓝海，但有个问题：

多数对标账号所在地区是印度或印度尼西亚（有一个开通YPP的是美国，但不多）。我自己账号后台数据也显示，观众多为印度用户。

这意味着开通YPP后收益可能偏低；如果不能接受，可以考虑换赛道。接下来详细拆解制作方法。

# 4.1.6.2 第一步：拿到对标视频

先把对标账号的爆款视频下载下来，方便后续操作。两种方法：

第一种：用现成的在线YouTube下载网站，不限次数且免费，效果不错。把分享的Excel文件里“url”那一列的链接放上去，或打开想下载的对标视频复制链接粘贴过去即可。

第二种：我用cursor写了一个python程序，可用Excel批量导入视频链接并自动下载，封装好的软件放在百度网盘，大家自行下载使用。

百度网盘链接：https://pan.baidu.com/s/1_zFUb72xeABeVpldlqambQ?pwd=xrmc

提取码：xrmc

使用说明：Youtube自动化工具分享 & 开发复盘

[PRE8]

# 4.1.6.3 第二步：截出静态帧

下载好对标视频后，第二步是从中截取两张风格不同的图片备用。同样三种方法：

第一种：直接点开对标视频播放，用win+shift+s截图（Windows系统的方法，Mac不太清楚）。

第二种：用剪映或capcut的“导出静态画面”功能。打开剪映，点左上角“导入”，找到对标视频，选中，点“打开”导入。

[PRE9]

[PRE10]

然后，把对标视频从左上方拖进轨道。

[PRE11]

接着，把时间轴拉到视频开头，点视频右上角三条横杠，选择“导出静帧画面”，选好保存位置，就能把窗口中看到的图片保存下来，这是第一张要用的风格图。

[PRE12]

[PRE13]

[PRE14]

最后照同样操作，把时间轴拉到视频末尾，导出第二张风格图，这样就得到两张对标视频的风格图片备用。

[PRE15]

[PRE16]

[PRE17]

第三种：用@老馬🐎内容出海 开发的视频帧截取软件，使用教程详见：【点击这里直接跳转】

# 4.1.6.4 第三步：靠 GPT-4o 或 DALL E 还原风格

准备好两张对标视频的风格图后，下一步是1:1复刻，这一步用ChatGPT的GPT-4o或DALL E模型（MJ我试下来效果不如GPT，也可能是我提示词没到位，熟悉MJ的圈友可以自己探索）。

先进入GPT官网：https://chatgpt.com/

（我做AI转绘基本用官网原生模型，中转或套壳站没尝试过，效果不保证，有条件尽量用官网）

然后点左上角“探索GPT”，往下滑找到DALL E模型（之前用过会直接显示在侧边栏）。

[PRE18]

[PRE19]

下面正式开始复刻，我用DALL E模型演示一遍（也建议优先用DALL E，次选GPT-4o）。

打开DALL E，点聊天框左边回形针，上传要复刻的图片。

[PRE20]

这里注意：我一般选色彩比较接近生活的对标图片来复刻，不选风格色彩很浓的。比如下面四张图，我会复刻第一张和第三张；第二张和第四张转换风格后的图片，我会用即梦AI实现（后面会讲）。

[PRE21]

[PRE22]

[PRE23]