# 对话荧光笔 · ChatGPT Marker

给 Mac Safari 中的 ChatGPT 对话划重点、写批注，导出带标记的 PDF。

**当前版本：v0.4.1 · 开发预览版**

[下载 Safari 预览版](https://github.com/ChaohuiGuoCN/chatgpt-marker/releases/download/v0.4.1/ChatGPT-Marker-Safari-v0.4.1.zip) · [下载网站与安装指南](https://chatgpt-marker.chaohui-97.chatgpt.site) · [所有版本](https://github.com/ChaohuiGuoCN/chatgpt-marker/releases)

> 这是需要手动加载的临时扩展，尚未签名或公证，不是双击安装的 macOS 应用。Safari 在退出或 24 小时后会移除临时扩展，使用期间请定期导出 JSON 备份。

## 可以做什么

- 四种颜色高亮文字；完成选字后，4 秒内双击沿用上次颜色。
- 完成选字后，4 秒内三击插入批注；批注在侧边显示，支持折叠和编号跳转。
- 按颜色或复选框选择笔记，复制原文和批注；也可追加到 ChatGPT 草稿，不会自动发送。
- 导出整段已加载对话或单条回复的 PDF，保留高亮与完整批注。
- 可拖动并自动靠边的笔工具，以及用于临时指示的激光笔。
- 标记保存在本机，可备份和恢复。

## 下载安装

1. 下载上面的 **ChatGPT-Marker-Safari-v0.4.1.zip** 并解压。不要下载 GitHub 自动生成的 “Source code” 文件。
2. 在 Safari → 设置 → 高级中打开“显示网页开发者功能”。
3. 打开设置 → 开发者 → 添加临时扩展，按系统提示允许未签名扩展。
4. 选择解压后的 **ChatGPT-Marker** 文件夹，其中应直接包含 `manifest.json`。
5. 在设置 → 扩展中启用“对话荧光笔”，允许访问 `chatgpt.com`，然后刷新一段已保存的对话。

本机实测 Safari **26.5.2**。需要有“添加临时扩展”入口的 Mac Safari；没有此入口的版本不能用此 ZIP 直接安装。iPhone / iPad 暂未支持。

[详细安装、更新和卸载步骤](INSTALL.md) · [隐私说明](PRIVACY.md) · [版本说明](CHANGELOG.md)

## 使用提示

PDF：打开荧光笔列表 → 右上角设置 → 导出本段对话 PDF。单条回复：点击回复下方分享 → 导出该回复 PDF。在打印窗口选择 **PDF → 存储为 PDF**，扩展不会创建公开分享链接。

整段 PDF 只包含页面已加载的消息和保存的笔记；较长对话请先向上滚动加载。公式目前导出为公式源文本，图片需要原图可访问。

这是独立项目，与 OpenAI、ChatGPT 或 Apple 无隶属关系。此仓库用于发布运行文件和说明，不包含开发源码，也未授予开源许可证。浏览器扩展的运行文件包含 JavaScript。
