✅ 一、什么是 CSP

CSP（Content Security Policy） 是浏览器安全策略，用来限制：

- 页面可以加载哪些 JS

- 可以请求哪些 API

- 可以建立哪些 WebSocket

- 可以加载哪些 iframe / 图片 / 字体

👉 本质作用：

   🔐 防止 XSS 攻击 + 第三方脚本注入 + 数据泄露


✅ 二、开启 CSP 的两种方式

⭐ 方式1（推荐）
通过 HTTP Header 设置

这是 生产环境标准做法

例如：
```nginx

Content-Security-Policy: default-src 'self';

```

⭐ Nginx 配置示例

```nginx

add_header Content-Security-Policy "
default-src 'self';
script-src 'self' https://cdn.jsdelivr.net;
style-src 'self' 'unsafe-inline';
img-src 'self' data:;
connect-src 'self' https://api.example.com;
frame-src https://www.youtube.com;
";

```

✅ 五、开发调试技巧（非常重要）

先用：

```nginx

Content-Security-Policy-Report-Only

```

例如：

```nginx

add_header Content-Security-Policy-Report-Only "
default-src 'self';
report-uri /csp-report;
";

```

👉 浏览器：

✔ 会记录违规
✔ 不会真正阻止

适合上线前测试 👍
