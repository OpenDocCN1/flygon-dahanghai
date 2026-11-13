# AI配图+一键发布，一小时跑通

这期视频聚焦一个具体难题：给文章配上符合语义的 AI 图片。思路是用硅基流动提供的免费可灵模型，让配图跟着文章内容走。完整动手时间大约 60 分钟。

视频入口在下方，建议先完整看一遍，再对照文字版操作：

https://scys.com/view/docx/J4ETdEfOpo4P3kxAWQOcZJl7nWf#ErqSdwWUwoGFp2xVNABccIwmnbJ

文字版操作步骤在下面（动手时间约 1 小时）：

#### 2.2 让 Claude code 把功能落地

先进入硅基流动模型广场：https://cloud.siliconflow.cn/me/models

在模型广场把筛选条件切到“生图”，挑免费的可灵模型：

[PRE0]

接着点开 API 文档：

[PRE1]

把请求参数和返回数据复制出来，拼装成提示词，再交给 cc：

[PRE2]

JSON

[PRE3]

[PRE4]

没多久，cc 先把改动范围确认清楚，又抛出几个问题等我们回答：

[PRE5]

我们逐条答复：

Plain Text

[PRE6]

需求敲定后约半小时，cc 就把这次改动交付了：

[PRE7]

[PRE8]

打开应用，生成一篇测试文章，结果首测即成功：

[PRE9]

## 02.发布模块：一次操作同步到📕与👸号

接下来进入最后一块：发布模块。目标是把草稿文章借助各平台开放 API 推送出去。

这一章聚焦🛰️👸号和📕两条发布路径。两个平台的情况并不一样：

+   **🛰️👸号**：有正式的开发接口，能把文章传到👸号草稿箱并发布，但前提是开发者具备👸号权限，还要完成接口配置，例如获取 appid/secret、设置白名单等。

+   **📕**：提供开放平台 API，通过 OAuth 拿到用户授权后，可以调用内容发布接口。不过开放权限可能有限，不少开发者会转向模拟登录等方式。本教程按使用官方开放 API 发布来假设。

实现上拆成🛰️端与📕端两条线，但对外只留一个统一发布入口，方便用户操作。

### 1.👸号端发布

#### 1.1 视频教程

这节视频主要讲怎么把生成好的文章一键送进👸号草稿箱，预计动手 1—2 小时。

视频入口在下方，建议先看完视频，再照着文字版做：

https://scys.com/view/docx/J4ETdEfOpo4P3kxAWQOcZJl7nWf#YzVBdwp1gocVikxRIZncvJEdn1m

文字版步骤在下面（动手时间约 1—2 小时）：

#### 1.2 借助 ClaudeCode 打通👸号发布

按照👸号和小绿书的发布流程，需要采用第三方 API 对接。

之所以选第三方 API，是因为直接走👸号官方接入流程非常复杂——单是完成🛰️开放平台的基础接入，往往就要耗掉两到三周。

所以用第三方 API 会更省事。当然，如果你有自己的云服务器，而且👸号已完成实名，也可以自行接入，但这里流程很复杂，就不展开了。感兴趣可参考：https://developers.weixin.qq.com/doc/subscription/guide/（如果你不是技术出身，大概率搞不定这个）

具体操作步骤：

第一步：进入👸号开放平台，输入对应网址后，先完成👸号绑定。绑定完成后，就能拿到所有关联的👸号信息。

第二步：核心用到两个接口：

+   第一个是“获取已绑定👸号”接口，点击即可获取当前账号下所有已绑定的👸号列表。

+   第二个是发布接口，只需传入标题、正文和目标👸号名称，就能把内容直接保存到对应👸号的草稿箱。

功能实现上，把需求给到 CC：需要实现“发布👸号”按钮的对应功能，具体是——点击按钮后弹出弹窗，显示所有已绑定的👸号账号，支持选择指定👸号；同时弹窗需提供选项，让用户选择发布到“小绿书”还是“👸号”；选定后点击发布，系统会自动调用对应发布接口，完成草稿发布。

明白流程以后，先去 https://wx.mgxingyuan.com/ 申请 API，激活码为：2QGAW036

可以直接扫码绑定🛰️，然后在 https://wx.mgxingyuan.com/api-doc/publish 获取接口，拿它和模型配合。

第一步把需求直接告诉 cc，要求他出文档和技术方案：

[PRE10]

[PRE11]

[PRE12]

针对 cc 的方案给出建议并确认，然后要求 cc 执行，最终一次跑通，👸号发布功能落地：

[PRE13]

[PRE14]

👸号发布用到的完整提示词见下：

ProtoBuf

[PRE15]bash

curl -X POST https://wx.limyai.com/api/openapi/wechat-accounts \

  -H &quot;X-API-Key: your-api-key&quot; \

  -H &quot;Content-Type: application/json&quot;

[PRE16]

{

  &quot;success&quot;: true,

  &quot;data&quot;: {

    &quot;accounts&quot;: [

      {

        &quot;name&quot;: &quot;测试👸号&quot;,

        &quot;wechatAppid&quot;: &quot;wx1234567890&quot;,

        &quot;username&quot;: &quot;gh_abc123&quot;,

        &quot;avatar&quot;: &quot;https://...&quot;,

        &quot;type&quot;: &quot;subscription&quot;,

        &quot;verified&quot;: true,

        &quot;status&quot;: &quot;active&quot;,

        &quot;lastAuthTime&quot;: &quot;2024-01-01T00:00:00.000Z&quot;,

        &quot;createdAt&quot;: &quot;2024-01-01T00:00:00.000Z&quot;

      }

    ],

    &quot;total&quot;: 1

  }

}

[PRE17]

curl -X POST https://wx.limyai.com/api/openapi/wechat-publish \

  -H &quot;X-API-Key: your-api-key&quot; \

  -H &quot;Content-Type: application/json&quot; \

  -d &#x27;{

    &quot;wechatAppid&quot;: &quot;wx1234567890&quot;,

    &quot;title&quot;: &quot;测试文章&quot;,

    &quot;content&quot;: &quot;# 标题\n\n这是文章内容...&quot;,

    &quot;summary&quot;: &quot;这是文章摘要&quot;,

    &quot;contentFormat&quot;: &quot;markdown&quot;

  }&#x27;

[PRE18]

{

  &quot;success&quot;: true,

  &quot;data&quot;: {

    &quot;publicationId&quot;: &quot;uuid-here&quot;,

    &quot;materialId&quot;: &quot;uuid-here&quot;,

    &quot;mediaId&quot;: &quot;wechat-media-id&quot;,

    &quot;status&quot;: &quot;published&quot;,

    &quot;message&quot;: &quot;文章已成功发布到👸号草稿箱&quot;

  }

}

[PRE19]

{

  &quot;success&quot;: false,

  &quot;error&quot;: &quot;👸号不存在或未授权&quot;,

  &quot;code&quot;: &quot;ACCOUNT_NOT_FOUND&quot;

}

[PRE20]

curl -X POST https://wx.limyai.com/api/openapi/wechat-publish \

  -H &quot;X-API-Key: your-api-key&quot; \

  -H &quot;Content-Type: application/json&quot; \

  -d &#x27;{

    &quot;wechatAppid&quot;: &quot;wx1234567890&quot;,

    &quot;title&quot;: &quot;小绿书测试&quot;,

    &quot;content&quot;: &quot;这是纯文本描述\n\n[PRE21]\n[PRE22]&quot;,

    &quot;articleType&quot;: &quot;newspic&quot;