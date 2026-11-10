# 👸号与📕发布，一次讲清

这次围绕 cc 的方案先做了确认，随后 cc 按需求完成交付。下面按“发布前约定—接口与页面—配置与验收—📕方案”的顺序，把整条链路讲清楚。

```bash
curl -X POST https://note.limyai.com/api/openapi/publish_note \
  -H "Content-Type: application/json" \
  -H "X-API-Key: xhs_da7d4437bfb5a55897d59a34c1fb4571e8ae684e9b702f5503af6d02b5eeec68" \
  -d '{
    "title": "如何提升工作效率",
    "content": "今天分享5个提升效率的小技巧...",
    "coverImage": "https://example.com/cover.jpg",
    "images": ["https://example.com/1.jpg", "https://example.com/2.jpg"],
    "tags": ["效率", "职场"]
  }'
```

cc 的回复如下：

```json
{
  "success": true,
  "data": {
    "id": "550e8400-e29b-41d4-a716-446655440000",
    "note_id": "efficiency_tips_001",
    "title": "如何提升工作效率",
    "status_id": 1,
    "publish_url": "https://your-domain.com/publish/note?pub_id=...",
    "xiaohongshu_qr_image_url": "https://your-domain.com/api/xiaohongshu/qr?note_id=..."
  }
}
```

草稿箱里的内容按 Markdown 存储；真正发出时必须明确传 `contentFormat: "markdown"`。若选择小绿书模式，还得先把图片抽出来，并对纯文本做处理。

[PRE2]

异常处理要覆盖四类场景：API Key 失效、👸号授权到期、网络请求异常、参数校验不通过。

[PRE3]

交互反馈也不能少：加载中有提示，发布时有进度；成功则自动关闭弹窗，失败则把具体错误展示出来。

[PRE4]

可选项包括：挑选封面图、填写作者名、自定义摘要，以及定时发布。

[PRE5]

围绕 cc 给出的计划，先做了一次确认。

[PRE6]

cc 随后完成需求并交付：

[PRE7]

交付物主要有三块：拉取👸号清单、把文章推送到👸号、处理 Markdown 内容。

[PRE8]

拉取👸号清单走 GET 请求，调用外部🛰️ API，再把👸号列表返回给前端。

[PRE9]

推送文章走 POST 请求：先取出草稿内容，再请求🛰️发布接口，最后回写草稿的发布状态。

[PRE10]

界面部分加入了👸号下拉选择、发布类型切换（👸号文章 / 小绿书），封面图、作者、摘要作为可选填写项，并展示发布状态。

[PRE11]

数据层补了三个字段：publishStatus（发布状态）、publishPlatform（已发布平台）、publishData（发布记录详情）；数据库迁移已经执行 ✅。

[PRE12]

前端侧则导入发布弹窗组件，补上弹窗状态管理，改动“发布到👸号”按钮的处理逻辑，并接入发布成功后的回调。

[PRE13]

配置项需要补两个环境变量：WECHAT_API_KEY 和 WECHAT_API_BASE。

[PRE14]

使用时先选目标👸号（列表自动加载），再定发布类型（👸号文章或小绿书），最后按需填摘要、封面图和作者。

[PRE15]

验收第一项：点“发布到👸号”按钮，看👸号列表是否正常出现，并核对👸号信息是否完整。

[PRE16]

然后选👸号，类型定为“👸号文章”，填好可选字段，点发布并观察反馈。

[PRE17]

再找一篇带图的文章，类型切到“小绿书”，点发布看结果。

[PRE18]

边界情况也要测：无图文章发小绿书应报错；网络异常、授权过期分别模拟一遍。

[PRE19]

发布成功后，确认草稿的 publishStatus 变为 "published"，publishPlatform 中含 "wechat"，并检查 publishData 是否记录了发布信息。

[PRE20]

图片会从 Markdown 中自动抽取；外部图片链接会自动上传到🛰️服务器，所以图床稳定性很重要。

[PRE21]

草稿内容应保持 Markdown 格式；发布时自动带上 contentFormat: "markdown"。

[PRE22]

每次发布都会刷新 publishData，里面记录👸号 AppID、materialId、mediaId、发布时间等信息。

[PRE23]

实际效果可以直接看：点“发布到👸号”会弹出窗口，点发布后，对应内容就会出现在草稿箱中。

[PRE24]

[PRE25]

[PRE26]

### 2. 📕平台发布：把文章转成图文的轻量做法

📕这边真正的难点，是把一篇文章转成📕图文。单独做一版📕编辑器成本太高；如果时间允许，或者你的业务主阵地就是📕，可以用 Claude Code 按具体场景做一个编辑器。更省力的办法是直接把文章里的插图抽出来当图片。

#### 2.1 先看视频教程

**视频点击下方链接即可学习（强烈推荐先看完视频后，再学习文字部分）：**

https://scys.com/view/docx/J4ETdEfOpo4P3kxAWQOcZJl7nWf#Qd0VdCvmDomYVwx4s9nczljHnje

#### 2.2 借助 Claude Code 接入📕发布

访问下面网址注册 API：

https://note.limyai.com/dashboard/open/publish_note，激活码是：H64Q4VRD

完整调用提示词如下（注意把最后的密钥换成自己的！）:

Plain Text

[PRE27]

```bash
curl -X POST https://note.limyai.com/api/openapi/publish_note \
  -H "Content-Type: application/json" \
  -H "X-API-Key: xhs_da7d4437bfb5a55897d59a34c1fb4571e8ae684e9b702f5503af6d02b5eeec68" \
  -d '{
    "title": "如何提升工作效率",
    "content": "今天分享5个提升效率的小技巧...",
    "coverImage": "https://example.com/cover.jpg",
    "images": ["https://example.com/1.jpg", "https://example.com/2.jpg"],
    "tags": ["效率", "职场"]
  }'
```

[PRE28]

返回结构示例：

```json
{
  "success": true,
  "data": {
    "id": "550e8400-e29b-41d4-a716-446655440000",
    "note_id": "efficiency_tips_001",
    "title": "如何提升工作效率",
    "status_id": 1,
    "publish_url": "https://your-domain.com/publish/note?pub_id=...",
    "xiaohongshu_qr_image_url": "https://your-domain.com/api/xiaohongshu/qr?note_id=..."
  }
}
```