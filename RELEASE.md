# ChatGPT Marker v0.6.0 · Chrome + Safari

**English** | [中文](https://github.com/ChaohuiGuoCN/chatgpt-marker/blob/main/README.zh-CN.md)

The same highlights, margin notes, quick gestures, laser pointer, batch copy / draft insertion, JSON backups and PDF exports are now available in desktop Chrome and Safari on Mac. Both packages use the same feature code, with English as the initial language and a persistent Chinese option.

- **Chrome:** download **ChatGPT-Marker-Chrome-v0.6.0.zip**, extract it, open `chrome://extensions/`, enable Developer mode and choose Load unpacked. Select the folder containing `manifest.json`. Keep this folder in place. This preview is not in the Chrome Web Store.
- **Safari:** download **ChatGPT-Marker-Safari-v0.6.0-unsigned.dmg**. The app remains unsigned and non-notarized; Safari requires unsigned-extension permission again after each full quit.
- **Move notes:** back up as JSON in Safari and restore in Chrome. The browsers do not sync notes automatically.
- **PDFs:** the preview now reads Chrome extension storage correctly. Formulas, highlights and full notes are preserved in conversation and single-reply exports. In Chrome's print dialog choose Destination → Save as PDF.

74 automated tests passed, including PDF preview and popup checks using each browser's extension API. Chrome hardware testing is pending. See the installation guides and privacy notice attached below.

---

新增电脑版 Chrome，功能与 Mac Safari 一致：四色高亮、侧边批注、双击/三击快捷操作、激光笔、批量复制及追加到草稿、JSON 备份、整段对话和单条回复 PDF。两版使用同一套功能代码，默认英文，可切换中文。

- **Chrome：**下载 **ChatGPT-Marker-Chrome-v0.6.0.zip**，解压后在 `chrome://extensions/` 开启开发者模式，通过“加载已解压的扩展程序”选择包含 `manifest.json` 的文件夹。安装后保留文件夹。当前未上架 Chrome 应用商店。
- **Safari：**下载 **ChatGPT-Marker-Safari-v0.6.0-unsigned.dmg**，仍为未签名、未公证测试包，每次完全退出 Safari 后需重新允许未签名扩展。
- **笔记迁移：**在 Safari 导出 JSON 备份，再到 Chrome 恢复；不会自动同步。
- **PDF：**修复 Chrome 预览读取扩展存储的问题，保留公式、高亮与完整批注。Chrome 打印窗口选择“目标打印机 → 另存为 PDF”。

74 项自动化测试通过，包含两种浏览器 API 下的 PDF 预览与弹窗检查。Chrome 实机测试尚未完成。详细安装说明与隐私说明见附件。
