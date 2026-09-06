# 安装与使用 · v0.4.2

## DMG 测试安装包

下载 **ChatGPT-Marker-Safari-v0.4.2-unsigned.dmg**。这是免费测试包，没有 Apple 开发者证书签名和公证；仅使用本地临时签名（ad-hoc），让 Apple 芯片能够运行程序。

安装目标：macOS 14.2+、Safari 17.2+。包含 Apple 芯片与 Intel 两种架构。旧系统与 Intel 尚未实机验证；不支持 iPhone / iPad。

1. 打开 DMG，把 **ChatGPT Marker.app** 拖入 **Applications（应用程序）**。复制完成后弹出磁盘映像，不要直接在 DMG 中运行应用。
2. 从“应用程序”打开 ChatGPT Marker。若首次被 macOS 拦截，关闭提示，到 **系统设置 → 隐私与安全性 → 仍要打开**，按系统提示确认。系统会记住对这个应用的例外；更新后可能需要再次确认。
3. Safari → 设置 → 高级，启用 **显示网页开发者功能**（Show features for web developers）。
4. 设置 → 开发者，勾选 **允许未签名的扩展**（Allow unsigned extensions）。如需身份验证，请自行输入密码或使用 Touch ID。
5. 点击应用中的 **打开 Safari 扩展设置**，或手动进入 Safari → 设置 → 扩展，启用对话荧光笔，并允许访问 `chatgpt.com`。
6. 刷新一段已保存的 ChatGPT 对话。页面边缘出现两支笔后，选中文字，再选择颜色或批注图标。

## “永久信任”与以后使用

- **macOS 应用许可**：系统会记住对这个应用的“仍要打开”例外，并不是信任这个开发者未来所有软件。
- **Safari 扩展许可**：Apple 规定，退出 Safari 后“允许未签名扩展”会重置，下一次启动必须重新开启，必要时再次启用扩展。DMG 无法提供永久信任。
- **应用是否需要重装**：应用可以保留在“应用程序”中。这是随应用安装的扩展，不是临时文件夹加载；不需要每 24 小时重新下载。关闭浏览器窗口不等于完全退出 Safari。

## 从旧 ZIP 迁移

1. 在旧扩展仍可用时，先从荧光笔列表导出 JSON 备份。
2. 在 Safari 设置中停用旧的临时扩展，保留备份；不要同时运行新旧两份。
3. 安装并启用 DMG 版，刷新 ChatGPT 后，用荧光笔列表中的“恢复”导入备份。
4. 确认批注已恢复后，再移除旧的临时扩展。

临时扩展与 DMG 版使用不同的扩展身份，笔记不会自动迁移。应用安装和更新都不会读取你的旧笔记文件，必须由你选择备份文件恢复。

## 常用操作

- 高亮：选中文字，再选颜色。完成选字后 4 秒内双击鼠标左键，沿用上次颜色；三击插入批注。
- 复制：点击荧光笔图标打开列表，使用复选框或颜色圆点选择，再点击“复制”。“发送到对话框”只追加到草稿，不提交消息。
- PDF：荧光笔列表 → 设置 → 导出本段对话 PDF。或点击回复下方分享 → 导出该回复 PDF。在 Safari 打印窗口选择 PDF → 存储为 PDF。
- 备份：荧光笔列表 → 备份，保存 JSON 文件。恢复时使用列表中的恢复入口。
- 激光笔：点击上面的激光笔按钮，或按 Option + Shift + L；Esc 退出。

整段导出包括页面已经加载的提问与回答，以及保存的高亮和批注，不受复选框选择影响。长对话请先向上滚动加载。公式目前以公式源文本导出；无法加载的图片会在预览中提示。

## 更新与卸载

更新前先导出 JSON 备份。退出 ChatGPT Marker 应用，使用新 DMG 中的应用替换“应用程序”里的旧版。刷新 ChatGPT，并检查 Safari 的扩展启用与网站权限。以后版本会保持相同的扩展标识，但仍建议更新前备份。

卸载前先备份，停用 Safari 中的对话荧光笔，再把应用移到废纸篓并刷新页面。不要依赖卸载后仍保留扩展数据。

## 排查

- 扩展列表没有显示：确保应用在“应用程序”中并已打开过；先允许未签名扩展，再重新进入 Safari 的“扩展”设置。
- 页面没有笔工具：检查扩展是否启用、网站访问权限是否到期，然后刷新页面。新建空对话和临时聊天暂不保存标记，请打开已保存的 `/c/…` 或 `/share/…` 页面。
- 如果更新后首次启动受阻：使用系统提供的“仍要打开”，无需关闭系统整体安全保护。

## ZIP 备用安装方式

**ChatGPT-Marker-Safari-v0.4.2.zip** 仍可用作临时扩展测试：解压后，在 Safari 设置 → 开发者 → 添加临时扩展中选择直接包含 `manifest.json` 的 ChatGPT-Marker 文件夹。这种安装方式在退出 Safari 或 24 小时后会被移除。日常测试优先使用上面的 DMG。

## 官方说明

- [Apple：运行 Safari Web Extension](https://developer.apple.com/documentation/safariservices/running-your-safari-web-extension)
- [Apple：分发 Safari Web Extension](https://developer.apple.com/documentation/safariservices/distributing-your-safari-web-extension)
- [Apple：打开未知开发者的 Mac 应用](https://support.apple.com/guide/mac-help/mh40616/mac)
