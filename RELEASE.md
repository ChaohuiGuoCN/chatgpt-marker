# 对话荧光笔 v0.4.4 · Safari 公式结构修复 · 免费 DMG 测试版

**回答太长，先划重点；有疑问或不同想法，就地批注；多处看不懂，勾选后一起追问。**

[下载网站与功能示例](https://chatgpt-marker.chaohui-97.chatgpt.site) · [完整介绍](https://github.com/ChaohuiGuoCN/chatgpt-marker#readme)

## 三个问题，三个办法

以下是围绕“自学 Python，做一个记账工具”编写的虚构示例。

1. **回答太长，找不到重点 → 高亮重点。** 回答写了好几屏，你只想记住“先把一条收支记录存起来，再练习统计总额”。选中这句话高亮，下次回看更容易找到。
2. **不符合自己的情况，或者没看懂 → 原文批注。** 看到“建议每天连续学习三小时”，在旁边记下“我每天只有 30 分钟，能按这个时间重排吗？”；看到“边界条件”，记下“余额为 0 算吗？”。把不同看法和疑问留在对应原文旁。
3. **多个词不懂，逐个复制太麻烦 → 勾选后批量整理。** 把“最小可运行示例”“边界条件”“单元测试”及自己的问题勾选起来，一次复制，或点击“发送到对话框”，把原文和批注一起追加到草稿。检查后由你手动发送。

## 下载与安装

下载 Assets 中的 **ChatGPT-Marker-Safari-v0.4.4-unsigned.dmg**，打开后把 **ChatGPT Marker.app** 拖进“应用程序”。首次被拦截时，可使用系统设置 → 隐私与安全性 → 仍要打开。随后在 Safari 设置中允许未签名扩展，启用对话荧光笔并授权访问 chatgpt.com。

[完整安装与旧版迁移指南](https://github.com/ChaohuiGuoCN/chatgpt-marker/blob/main/INSTALL.md)

**关于永久信任：** macOS 会记住对这个应用的打开例外；Safari 每次完全退出后，仍需重新允许未签名扩展。DMG 不能取消这个限制，但应用可以保留，不用每 24 小时重新下载安装。

没有 Apple 开发者证书签名、未公证；本地临时签名仅用于运行。包含 Apple 芯片与 Intel 通用程序；安装目标 macOS 14.2+ / Safari 17.2+，旧系统与 Intel 尚未实机验证。仅限 Mac，不支持 iPhone / iPad。

旧版 ZIP 用户请先导出 JSON 备份，停用旧临时扩展，再在 DMG 版中恢复。笔记不会自动转移。

**其他附件：** ZIP 备用临时扩展（退出或 24 小时后会移除）、安装指南、隐私说明、SHA-256 校验值。不要下载 GitHub 自动生成的 “Source code” 文件。

## 本次修复：带中文说明的公式不再变成一行文字

ChatGPT 在 Safari 中会把部分公式的源码放在外层节点。v0.4.3 漏读了这一结构，导致帽子符号、上下标、括号和中文说明变成普通文字。本版补上这类公式的提取，整段对话和单条回复都适用。

- **整段对话**：荧光笔列表 → 设置 → 导出本段对话 PDF。
- **单条回复**：回复下方“分享” → 导出该回复 PDF。

两种方式都保留所属高亮与完整批注。在 Safari 打印窗口选择“PDF → 存储为 PDF”。

[整段对话 PDF 示例](https://chatgpt-marker.chaohui-97.chatgpt.site/samples/conversation.pdf) · [单条回复 PDF 示例](https://chatgpt-marker.chaohui-97.chatgpt.site/samples/reply.pdf) · [网站功能演示](https://chatgpt-marker.chaohui-97.chatgpt.site/#pdf)

示例为虚构内容，通过本机 Safari 实际导出，不包含真实用户对话。

## 验证与限制

64 项自动化测试通过，覆盖 Safari 的外层公式源码、中文下括号说明、上下标、公式去重、高亮与批注、单条回复范围和安全处理。旧系统与 Intel 尚未实机验证。

已安装本版 DMG，并从真实 ChatGPT 回复导出 PDF，逐页检查了带中文下括号说明的状态预测公式、高亮及批注。测试使用的真实对话文件仅留在本机，不包含在公开下载中。

整段 PDF 只包括页面已加载的对话；无法识别的公式保留可读取的内容并提示，图片需要原图可访问。

[版本记录](https://github.com/ChaohuiGuoCN/chatgpt-marker/blob/main/CHANGELOG.md) · [隐私说明](https://github.com/ChaohuiGuoCN/chatgpt-marker/blob/main/PRIVACY.md)
