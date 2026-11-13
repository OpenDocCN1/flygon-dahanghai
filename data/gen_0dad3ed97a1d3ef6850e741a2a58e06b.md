# 5.4.1.1 正反描述词速通

Prompt，说白了就是你敲给 AI 的那段文字。圈内常把它叫描述词、tag，也有人戏称“魔咒”。它分成两路：一路告诉 AI“要画什么”，另一路提醒 AI“别画什么”。

**先说正向描述词。** 它装的是你希望画面里出现的内容。写单词行，写短句也行，多个要素之间拿英文逗号断开，并且用英文表达。比如最基础的 `1girl, long hair`。想先把画质托住，常用 `masterpiece, the best quality`。排列时大致可以照这个路子走：画面质量提示词在前，接着画面主体与风格，再放相关艺术家，最后补其他细节。一个完整示例：
`（masterpiece），（best quality），（ultra-detailed），（full body:1.2），1girl，chibi，cute，smile，white Bob haircut，red eyes，earring，white shirt，black skirt，lace legwear，（sitting on red sofa），seductive posture，smile，A sleek black coffee table sits in front of the sofa and a few decorative items are placed on the shelves，（beautiful detailed face），（beautiful detailed eyes），`

**再看负向描述词。** 它负责列出你不想让 AI 画出来的东西。常见的负向清单可以按类别记，下面这些词及权重都来自常用配置：
- 画质与色调：`（worst quality:2），（low quality:2），（normal quality:2），lowres，normal quality，lowers，blurry，（（monochrome）），（（grayscale））`
- 肢体与解剖：`extra arms，extra limbs，mutated hands，（poorly drawn hands:1.5），（bad anatomy:1.21），（bad proportions:1.331），（missing arms:1.331），（extra legs:1.331），（fused fingers:1.61051），（too many fingers:1.61051），bad hands，missing fingers，extra digit，bad hands，missing fingers，（（（extra arms and legs））），disfigured，deformed，（disfigured:1.331），（mutilated:1.21），（duplicate:1.331），（morbid:1.21），（tranny:1.331）`
- 面部、皮肤与眼神：`cross-eye，skin spots，acnes，skin blemishes，age spot，（ugly:1.331），（unclear eyes:1.331）`
- 构图与内容限制：`body out of frame，NSFW`

一句话收束：正向词负责“添料”，负向词负责“排雷”；两边配合好，AI 出图才更接近你脑子里的画面。