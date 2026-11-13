waoowaoo 全流程部署：从环境到成片

想把故事线自动拆成分镜，再生成画面、配音，最后合成一个能下载的 MP4？这套 waoowaoo 流程值得先收藏。它的好处是四个阶段都有明确的验收点：每走完一步，你都能亲眼确认系统真的在干活，而不是靠感觉猜。

先在终端准备工具，把 openclaw-lark-tools 安装好：

[PRE0]

npx -y @larksuite/openclaw-lark-tools install

接着按四道关卡推进，每一关都有一个“看到即成功”的标志：

[PRE1]

第一阶段：环境准备 ────────────── 🏁 看到 waoowaoo 首页，API 连接全绿

↓第二阶段：故事变分镜 ─────────── 🏁 看到 AI 分析出的角色和画面描述

↓第三阶段：分镜变画面和声音 ──── 🏁 看到第一张漫画图 + 听到角色配音

↓第四阶段：画面变完整视频 ────── 🏁 下载到一个完整的 MP4 文件

换句话说，首页 API 全绿只是起点；随后要让 AI 把故事拆出角色和画面描述；再往后要看到首张漫画图、听到角色配音；最终拿到完整 MP4。每一步都有可检查的成果，流程会清晰很多。

下面进入服务器部署。先通过 SSH 连上你的机器：

[PRE2]

ssh root@你的服务器IP

然后执行一键安装脚本：

[PRE3]

curl -fsSL https://cnb.cool/fuliai/waoowaoo/-/git/raw/main/install.sh | bash

装完后看看容器有没有跑起来：

[PRE4]

cd /opt/waoowaoo &amp;&amp; docker compose ps

如果服务还没启动，补上这一条：

[PRE5]

docker compose up -d

之后在浏览器访问：

[PRE6]

http://你的服务器IP:13000

打开页面后，先完成登录。把下面的邮箱和密码替换成你自己的，脚本会自动处理 CSRF 和 cookie：

[PRE7]

# 把邮箱和密码换成你自己的

MY_EMAIL=&quot;你的邮箱&quot;

MY_PASSWORD=&quot;你的密码&quot;

rm -f /tmp/auth_cookies.txt

CSRF=$(curl -s -c /tmp/auth_cookies.txt http://localhost:13000/api/auth/csrf | python3 -c &quot;import json,sys; print(json.load(sys.stdin)[&#x27;csrfToken&#x27;])&quot;)

curl -s -c /tmp/auth_cookies.txt -b /tmp/auth_cookies.txt \

  -X POST http://localhost:13000/api/auth/callback/credentials \

  -H &quot;Content-Type: application/x-www-form-urlencoded&quot; \

  -d &quot;csrfToken=$CSRF&amp;username=$MY_EMAIL&amp;password=$MY_PASSWORD&amp;callbackUrl=http%3A%2F%2Flocalhost%3A13000&quot; &gt; /dev/null

echo &quot;✅ 登录完成&quot;

登录成功后，把火山引擎 Ark、Google、FAL 三个平台的 Key 填进去。下面三段 Key 都要换成你自己的，别直接照抄：

[PRE8]

# 把三个 Key 换成你自己的

curl -s -b /tmp/auth_cookies.txt \

  -X PUT http://localhost:13000/api/user/api-config \

  -H &quot;Content-Type: application/json&quot; \

  -d &#x27;{

    &quot;providers&quot;: [

      {&quot;id&quot;: &quot;ark&quot;, &quot;name&quot;: &quot;火山引擎 Ark&quot;, &quot;apiKey&quot;: &quot;你的ARK_API_KEY&quot;},

      {&quot;id&quot;: &quot;google&quot;, &quot;name&quot;: &quot;Google&quot;, &quot;apiKey&quot;: &quot;你的GOOGLE_API_KEY&quot;},

      {&quot;id&quot;: &quot;fal&quot;, &quot;name&quot;: &quot;FAL&quot;, &quot;apiKey&quot;: &quot;你的FAL_API_KEY&quot;}

]}&#x27;echo &quot;✅ API Key 配置完成&quot;

部署完成后别急着出片，先做一次自检。下面会检查 curl、python3、docker、ffmpeg 是否就绪，也会确认 waoowaoo 服务是否正常响应：

[PRE9]

echo &quot;=== 环境检查 ===&quot;

for cmd in curl python3 docker ffmpeg; do

  if command -v $cmd &gt; /dev/null 2&gt;&amp;1; then

    echo &quot;✅ $cmd 已安装&quot;

  else

    echo &quot;❌ $cmd 未安装，请先安装&quot;

  fi

done

echo &quot;&quot;

echo &quot;=== 服务检查 ===&quot;

HTTP_CODE=$(curl -s -o /dev/null -w &quot;%{http_code}&quot; http://localhost:13000)

if [ &quot;$HTTP_CODE&quot; = &quot;200&quot; ] || [ &quot;$HTTP_CODE&quot; = &quot;302&quot; ]; then

  echo &quot;✅ waoowaoo 服务正常（HTTP $HTTP_CODE）&quot;

else

  echo &quot;❌ waoowaoo 服务异常（HTTP $HTTP_CODE），请运行: cd /opt/waoowaoo &amp;&amp; docker compose up -d&quot;

fi

如果提示 ffmpeg 缺失，就补装一下：

[PRE10]

apt update &amp;&amp; apt install -y ffmpeg

最后再执行一次登录确认，确保后续操作能正常带着身份访问：

[PRE11]

MY_EMAIL=&quot;你的邮箱&quot;

MY_PASSWORD=&quot;你的密码&quot;

rm -f /tmp/auth_cookies.txt

CSRF=$(curl -s -c /tmp/auth_cookies.txt http://localhost:13000/api/auth/csrf | python3 -c &quot;import json,sys; print(json.load(sys.stdin)[&#x27;csrfToken&#x27;])&quot;)

curl -s -c /tmp/auth_cookies.txt -b /tmp/auth_cookies.txt \

  -X POST http://localhost:13000/api/auth/callback/credentials \

  -H &quot;Content-Type: application/x-www-form-urlencoded&quot; \

  -d &quot;csrfToken=$CSRF&amp;username=$MY_EMAIL&amp;password=$MY_PASSWORD&amp;callbackUrl=http%3A%2F%2Flocalhost%3A13000&quot; &gt; /dev/null

echo &quot;✅ 登录完成&quot;

整套流程走完，只要服务检查正常、首页 API 连接全绿，就可以按四个阶段继续产出内容了。记得把服务器 IP、邮箱、密码以及三个平台的 Key 全部替换成自己的，再按顺序执行，基本就能从故事一路做到成片。