# PDD 福袋互助码实时页

这是一个适用于 GitHub Pages 的轻量页面，外层提供响应式视觉界面，互助页面由 `https://fudai.y1g.cc/pdd.php` 原站嵌入提供。互助码列表、提交、复制和举报操作都仍在原站页面中执行，本仓库不保存或转发互助码。

原站列表会定时刷新（当前观察到约每 5 秒一次）。GitHub Pages 是静态托管，原站 API 不允许从 GitHub Pages 浏览器端跨域读取，因此这里保留原站 iframe 来使用它的实时数据和后端逻辑。若需要重新设计 iframe 内部的表格和按钮，需要原站开放跨域 API，或增加受控的服务端代理。

## 发布到 GitHub Pages

1. 将 `index.html` 放在仓库根目录并推送到 `main` 分支。
2. 打开仓库 **Settings → Pages**。
3. 在 **Build and deployment** 中选择 **Deploy from a branch**，分支选 `main`，目录选 `/(root)`。

项目页地址：<https://mofan6.github.io/pdd-fudai-live/>。
