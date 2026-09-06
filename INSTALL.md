# 安装与使用 · v0.4.1

## 下载前先看

- 适用：Mac 上具有“添加临时扩展”入口的 Safari。本机实测 Safari 26.5.2；未测试 iPhone / iPad。
- 当前是未签名的开发预览版 ZIP，需要手动加载；尚无正式的 .app、.dmg 或 App Store 版本。
- Apple 说明：临时扩展在退出 Safari 或 24 小时后被移除。请经常备份笔记，移除或重新安装可能丢失扩展存储。

## 安装

1. 下载 **ChatGPT-Marker-Safari-v0.4.1.zip**，双击解压，得到 **ChatGPT-Marker** 文件夹。
2. 打开 Safari → 设置 → 高级，启用“显示网页开发者功能”（Show features for web developers）。已经看到“开发者”标签时可跳过。
3. 打开 Safari → 设置 → 开发者，点击“添加临时扩展”（Add Temporary Extension…）。按系统提示允许未签名扩展；如需身份验证，请自行输入密码或使用 Touch ID。
4. 选择解压后的 **ChatGPT-Marker** 文件夹。该文件夹中应直接包含 `manifest.json`，不要选择外层下载文件夹。
5. 打开设置 → 扩展，启用“对话荧光笔 · ChatGPT Marker”，允许访问 `chatgpt.com`。旧域名 `chat.openai.com` 也在扩展声明的支持范围内。
6. 打开或刷新一段已保存的 ChatGPT 对话，页面边缘会出现两个竖排笔工具。先选中文字，再点击颜色或批注图标。

如果没有“添加临时扩展”入口，请先确认 Safari 是否提供可用更新；此 ZIP 无法在不支持该入口的版本中直接安装。当前也不提供 iPhone / iPad 的安装包。

## 常用操作

- 高亮：选中文字，再选颜色。完成选字后 4 秒内双击鼠标左键，沿用上次颜色；三击插入批注。
- 复制：点击荧光笔图标打开列表，使用复选框或颜色圆点选择，再点击“复制”。“发送到对话框”只追加到草稿，不提交消息。
- PDF：荧光笔列表 → 设置 → 导出本段对话 PDF。或点击回复下方分享 → 导出该回复 PDF。在 Safari 打印窗口选择 PDF → 存储为 PDF。
- 备份：荧光笔列表 → 备份，保存 JSON 文件。恢复时使用列表中的恢复入口。
- 激光笔：点击上面的激光笔按钮，或按 Option + Shift + L；Esc 退出。

整段导出包括页面已经加载的提问与回答，以及保存的高亮和批注，不受复选框选择影响。长对话请先向上滚动加载。公式目前以公式源文本导出；无法加载的图片会在预览中提示。

## 更新或重新加载

1. 在旧扩展仍可用时，先导出 JSON 备份。
2. 下载并解压新版本，保留解压后的文件夹。
3. 如果继续使用同一个扩展文件夹，替换文件后在 Safari 设置 → 扩展中点击“重新加载”（Reload），再刷新 ChatGPT。
4. 如果临时扩展已被移除，按安装步骤重新添加，再恢复 JSON 备份。不要依赖重新添加后仍能保留旧数据。
5. 检查批注已恢复后，再处理旧版本文件和备份。

如果没有出现笔工具，检查网站访问权限是否到期，确认扩展已启用并刷新页面。新建空对话和临时聊天暂不保存标记；请打开已保存的 `/c/…` 对话或 `/share/…` 页面。

## 卸载

先备份需要的笔记，再到 Safari → 设置 → 扩展中移除“对话荧光笔”。刷新已打开的 ChatGPT 页面后，页面工具会消失。不要依赖卸载后仍能保留标记。

## 官方说明

- [Apple：运行 Safari Web Extension](https://developer.apple.com/documentation/safariservices/running-your-safari-web-extension)
- [Apple：分发 Safari Web Extension](https://developer.apple.com/documentation/safariservices/distributing-your-safari-web-extension)
