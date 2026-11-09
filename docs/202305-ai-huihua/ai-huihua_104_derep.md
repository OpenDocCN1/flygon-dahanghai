# 5.8.2.5 ControlNet 组合玩法

组合技，说白了就是让多个 ControlNet 一起上场干活。拿素材里那两只狗狗来说，做法是先用 Canny 提取出两张预处理图，再分别交给两个 ControlNet 来控制。

![](img/b2e0994306452f1c5334a2af12adfd9e.png)

ControlNet0

![](img/dd3aff8bc67b6cda3def363e88a10e4b.png)

ControlNet1

![](img/523360da53c24d822165ecc55d3b925c.png)

生成结果

可玩的搭配远不止这一种：线稿配骨骼、线稿配深度图、骨骼配语义分割……各种组合都值得大胆试一试。不同搭配往往能带来意想不到的效果，甚至收获小惊喜。

• 多个 ControlNet 怎么开启

![](img/7a5d5b32c76174148bf4a7142bd87959.png)

照这个方式操作，就能同时启用多个 ControlNet，组合招式随便安排，连续出招也不成问题。

![](img/1ee789506ec81b3060a7c2f2c15117e4.png)

当你顺利搞定插件安装、日常使用，并且完成模型炼制，恭喜你——这时候你已经称得上一位出色的高阶魔法师了。

![](img/e12d1c8b9f4ffdf6c4edf913cceed533.png)