[English](INSTALL-CHROME.md) | **中文**

# Chrome 安装说明 · v0.6.0

从 [GitHub Releases](https://github.com/ChaohuiGuoCN/chatgpt-marker/releases/tag/v0.6.0) 或[网站](https://chatgpt-marker.chaohui-97.chatgpt.site/?lang=zh#install)下载 **ChatGPT-Marker-Chrome-v0.6.0.zip**。不要下载 GitHub 自动生成的 “Source code” 或 Safari 的 DMG。

当前通过 Chrome 开发者模式安装，尚未上架 Chrome 应用商店。安装目标为电脑上的 Chrome 105+，适用于 macOS、Windows 和 Linux，建议使用最新版本。本版尚未完成实机验证；暂不支持手机 Chrome。

## 安装

1. 解压 ZIP，把 **ChatGPT-Marker-Chrome** 文件夹放在准备长期保留的位置。该文件夹内应直接包含 `manifest.json`、`content.js` 和 `pdf.html`。
2. 在 Chrome 地址栏输入 `chrome://extensions/`。
3. 打开右上角的 **开发者模式 / Developer mode**。
4. 点击 **加载已解压的扩展程序 / Load unpacked**，选择 **ChatGPT-Marker-Chrome** 文件夹，不要选择 ZIP 或上一级目录。
5. 打开或刷新一段 `https://chatgpt.com/c/…` 的已保存对话，页面边缘会出现激光笔和荧光笔。

安装后请保留文件夹，不要移动或删除；Chrome 会直接读取这里的文件。更新时不要先卸载。此方式没有 Safari 临时扩展的 24 小时到期限制。由公司或学校管理的浏览器可能限制开发者模式扩展。

## 功能与 Safari 一致

- 黄色、绿色、蓝色、粉色高亮；选字后 4 秒内双击沿用上次颜色，三击添加批注。
- 批注显示在原文旁，可以折叠；点击编号跳转。拖动笔工具可改变位置，松手自动吸边。
- 用复选框或颜色筛选条目，批量复制或追加到对话草稿；每条也能单独复制。“发送到对话框”只填入草稿，不会提交消息。
- 激光笔用于演示。**Alt/Option + Shift + L** 开关激光笔，**Alt/Option + Shift + H** 高亮选区，**Esc** 退出激光笔。
- 荧光笔列表 → 设置 → 导出本段对话 PDF；回复下方“分享” → 导出该回复 PDF。在 Chrome 打印窗口选择 **目标打印机 / Destination → 另存为 PDF / Save as PDF → 保存**。保留公式、高亮和完整批注，不创建公开分享链接。
- JSON 备份与恢复。设置、工具栏弹窗和 PDF 预览均可切换中英文，默认英文并记住选择。

## 把 Safari 的笔记带过来

在 Safari 的荧光笔列表点击“备份”，保存 JSON 文件；再到 Chrome 的列表点击“恢复”，选择该文件。打开同一段 ChatGPT 对话即可看到对应笔记。两个浏览器的存储独立，不会自动同步。备份包含所选原文和批注，请按自己的笔记保管。

## 更新与卸载

更新前先导出 JSON 备份。解压新版 ZIP，用新版文件替换**原来已安装文件夹内的内容**，保留文件夹的名称和位置。在 `chrome://extensions/` 点击扩展的“重新加载”，然后刷新 ChatGPT。加载另一个位置的文件夹可能产生新的安装副本，其笔记存储也会分开。

卸载前先备份，在扩展管理页点击“移除”，再删除不需要的文件夹。卸载可能同时删除扩展保存的数据。

## 排查

- **无法加载 manifest：**选择直接包含 `manifest.json` 的文件夹。
- **没有笔工具：**检查扩展是否启用、是否允许访问 `chatgpt.com`，再刷新对话。新建空对话和临时聊天暂不支持保存标记。
- **PDF 缺少内容：**从对话重新导出。长对话先向上滚动加载；图片需原图可访问。无法排版的公式保留可读取的内容并提示。
- **更新后还是旧版：**先重新加载扩展，再刷新 ChatGPT，只刷新网页不会重新加载扩展文件。

[Google 官方安装步骤](https://developer.chrome.com/docs/extensions/get-started/tutorial/hello-world#load-unpacked) · [隐私说明](PRIVACY.zh-CN.md)
