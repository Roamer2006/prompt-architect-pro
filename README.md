# Prompt Architect Pro PWA

这是可部署的纯静态 PWA，无需服务器端、账号或 API Key。生成提示词、质量评分和历史记录均在浏览器本地完成。

## Android 安装

1. 将本目录全部文件部署至任意支持 HTTPS 的静态站点（例如 GitHub Pages、Cloudflare Pages 或 Netlify）。
2. 在 Android 手机 Chrome 中打开部署后的 HTTPS 地址。
3. 使用 Chrome 菜单「添加到主屏幕」或「安装应用」。
4. 首次在线打开后，缓存成功时可离线使用。

**注意**：直接打开本地 index.html 可以使用大部分页面功能，但无法正常注册 Service Worker，也不能获得完整 PWA 安装体验。需要 HTTPS 网址（localhost 开发环境除外）。

## 本地测试

在目录内执行 `python -m http.server 8000`，用电脑浏览器打开 http://localhost:8000。

## 功能

- 中文移动端布局；任务场景自动识别与手动选择
- PPT、项目管理、邮件、数据分析、通用任务专业规则
- 启发式提示词完整度评分与信息缺口提醒
- 背景、约束、验收标准、交付形式、分析深度等配置
- 一键复制、系统分享、本地历史（最多 50 条）
- Service Worker 离线缓存和 Web App Manifest

本应用是**提示词生成器**，并不会自行调用 ChatGPT 或生成 PPT/Excel 文件；分享按钮可将生成的文本发送到 Android 分享目标。
