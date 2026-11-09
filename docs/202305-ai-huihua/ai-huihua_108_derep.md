# 6.1 提示词进阶指南

无论你用的是哪款AI绘图工具，想让出图又快又稳，提示词都是绕不开的核心。之前我们断断续续提过一些写法，今天系统聊透。

## 提示词有哪些类别？

写提示词时，可以从下面这些维度去拆解：

- **画质类**：masterpiece、(the best quality)、extremely detailed、ultra high res、best quality、photo、4k、(photorealistic:1.4)
- **主题/场景**：Indoor、outdoor、grass
- **人物属性**：包括头发长短、颜色、发型，脸部特征、头饰、装饰、服装等，比如 hair length、hair color、hair style、decorations on head
- **姿势与视角**：pov_hands、sitting、the_whole_body，还有 look at、look up、look down、bird's-eye view
- **物体**：book、cloud、gun、pen、teacup
- **时间与光线**：day、evening、morning、night、twilight，以及 rim light、Warm light、soft light、back light
- **画风**：cartoon、steampunk、Disney style
- **艺术家**：Van Gogh、Hayao Miyazaki
- **镜头语言**：depth of field
- **模型引入**等等

## 提示词的权重怎么调？

权重决定了AI优先处理哪些信息。掌握这几种写法，你就能控制表达的分寸：

- `(word)`：权重提升1.1倍，例如 `(best quality)`、`(masterpiece)`
- `((word))`：权重变为1.21倍（1.1×1.1），括得越多，倍数越高
- `[word]`：权重降为原来的90.91%，比如 `[flower]`
- `(word:1.5)`：权重直接变为1.5倍
- `(word:0.25)`：权重只剩原来的25%
- `\(word\)`：加反斜杠表示字面括号，AI不会把它理解成加权操作

另外，提示词越长，单个词分到的权重就会越少。

## 提示词可以怎么写？

表达形式可以很灵活：

- **单词**：1girl、smile、street
- **句子**：A smiling girl, walking in the street
- **短语**：A girl is walking down the street with a smile and an ice cream in her hand
- **Emoji**：比如 money-mouth face、smiling face with hearts、smiling face with heart-eyes，可以参考 [unicode.org/emoji/charts/emoji-list.html](https://unicode.org/emoji/charts/emoji-list.html)
- **颜文字**：像 o_O 这类，参考 [表情符号列表](https://zh.wikipedia.org/wiki/表情符号列表)
- **分隔规则**：不同提示词之间用英文逗号隔开，空格和换行不会影响识别
- **同类词混用**：比如 blonde hair、blue hair 这类同类型的词，AI可能会分别呈现，也可能混合在一起
- **AND 连接**：想让多个元素都稳定出现，可以用大写 AND，比如 `blonde hair AND blue hair`；用逗号不一定都能保证出现

### 正向提示词

正向提示词是你希望AI画出来的内容，可以是单词也可以是句子，用英文写，逗号分隔。通用质量词优先上：`masterpiece`、`the best quality`。

推荐顺序大致是：画面质量 → 主题内容 → 风格 → 相关艺术家 → 其他细节。举个例子：

`(masterpiece), (best quality), (ultra-detailed), (full body:1.2), 1girl, chibi, cute, smile, white Bob haircut, red eyes, earring, white shirt, black skirt, lace legwear, (sitting on red sofa), seductive posture, smile, A sleek black coffee table sits in front of the sofa and a few decorative items are placed on the shelves, (beautiful detailed face), (beautiful detailed eyes)`

### 反向提示词

反向提示词是你不希望出现的内容。平时可以直接用一套通用模板，把常见问题全塞进去，例如：

`extra arms, disfigured, deformed, cross-eye, body out of frame, NSFW, (worst quality:2), (low quality:2), (normal quality:2), lowres, normal quality, ((monochrome)), ((grayscale)), skin spots, acnes, skin blemishes, age spot, (ugly:1.331), (duplicate:1.331), (morbid:1.21), (mutilated:1.21), (tranny:1.331), mutated hands, (poorly drawn hands:1.5), blurry, (bad anatomy:1.21), (bad proportions:1.331), extra limbs, (disfigured:1.331), (missing arms:1.331), (extra legs:1.331), (fused fingers:1.61051), (too many fingers:1.61051), (unclear eyes:1.331), lowers, bad hands, missing fingers, extra digit, bad hands, missing fingers, (((extra arms and legs)))`

## 进阶玩法：关键词替换与循环

你还能让关键词在生成过程中按时间线变化：

- **加入关键词**：`[to:when]`，等价于 `[关键词:数字]`，表示在生成的第几步把这个词加进去
- **删除关键词**：`[from::when]`，等价于 `[关键词::数字]`。数字大于1时代表步数，比如 `[bow tie:12]` 表示第12步之后不再使用 bow tie
- **切换关键词**：`[from:to:when]`，等价于 `[关键词1:关键词2:数字]`。数字大于1，表示在第多少步之前用前者，之后换成后者；数字小于0则按百分比理解，比如0.5就是前50%步数用前者，后50%用后者

如果想要多个关键词轮流出现，用竖线分隔：`[关键词1|关键词2|关键词3]`，原理等同 `[a|b|c]`，AI会按 a→b→c→a 的顺序循环生成。

## 模型调用：LORA 与 Embedding

- **LORA**：格式为 `<lora:模型名称:权重>`，例如 `<lora:blindbox_V1Mix:1>`。权重越小，使用程度越低，建议最大不超过1；多个LORA可以同时使用，但权重总和建议不要超过1.3，否则画面容易崩坏。
- **Embedding**：直接在模型处点击调用即可。这里有个大坑：任何模型（包括LORA和Embedding）都不能写进反向提示词里。

## 几点提醒

1. 不要出现拼写错误的单词，否则AI会乱识别。
2. 用词尽量具体，别写太模糊宽泛的描述，否则随机性会很大。
3. 提示词的读取顺序是从左到右，越靠后的词权重越低。

把这些规则吃透，你会发现出图质量和对画面的掌控力都会明显提升。

![](img/e12d1c8b9f4ffdf6c4edf913cceed533.png)