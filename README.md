# PDD 福袋互助码实时页

这是一个适用于 GitHub Pages 的轻量页面，直接嵌入原站 `https://fudai.y1g.cc/pdd.php`。原站页面、互助码列表和提交/复制/举报操作都在原站域名中运行，所以会继续使用原站数据和后端逻辑；本仓库不保存或转发互助码。

原站列表会定时刷新（当前观察到约每 5 秒一次）。这个页面只负责显示原站，不需要构建步骤或 API 密钥。

## 发布到 GitHub Pages

1. 在 GitHub 新建一个仓库（例如 `pdd-fudai-live`），把本目录中的 `index.html` 放到仓库根目录并推送到 `main` 分支。
2. 打开仓库 **Settings → Pages**。
3. 在 **Build and deployment** 中选择 **Deploy from a branch**，分支选 `main`，目录选 `/(root)`，保存。
4. 等 GitHub Pages 完成部署。项目页地址会是 `https://<你的用户名>.github.io/<仓库名>/`。

以后只要原站仍在线且允许被嵌入，互助码会继续从原站实时读取，无须重新部署。若原站关闭嵌入、调整登录/浏览器策略或停止服务，GitHub Pages 的静态页面无法自行绕过这些限制。
