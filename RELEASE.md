# 对话荧光笔 v0.4.3 · PDF 公式修复 · 免费 DMG 测试版

**回答太长，先划重点；有疑问或不同想法，就地批注；多处看不懂，勾选后一起追问。**

[下载网站与功能示例](https://chatgpt-marker.chaohui-97.chatgpt.site) · [完整介绍](https://github.com/ChaohuiGuoCN/chatgpt-marker#readme)

## 三个问题，三个办法

以下是围绕“自学 Python，做一个记账工具”编写的虚构示例。

1. **回答太长，找不到重点 → 高亮重点。** 回答写了好几屏，你只想记住“先把一条收支记录存起来，再练习统计总额”。选中这句话高亮，下次回看更容易找到。
2. **不符合自己的情况，或者没看懂 → 原文批注。** 看到“建议每天连续学习三小时”，在旁边记下“我每天只有 30 分钟，能按这个时间重排吗？”；看到“边界条件”，记下“余额为 0 算吗？”。把不同看法和疑问留在对应原文旁。
3. **多个词不懂，逐个复制太麻烦 → 勾选后批量整理。** 把“最小可运行示例”“边界条件”“单元测试”及自己的问题勾选起来，一次复制，或点击“发送到对话框”，把原文和批注一起追加到草稿。检查后由你手动发送。

## 下载与安装

下载 Assets 中的 **ChatGPT-Marker-Safari-v0.4.3-unsigned.dmg**，打开后把 **ChatGPT Marker.app** 拖进“应用程序”。首次被拦截时，可使用系统设置 → 隐私与安全性 → 仍要打开。随后在 Safari 设置中允许未签名扩展，启用对话荧光笔并授权访问 chatgpt.com。

[完整安装与旧版迁移指南](https://github.com/ChaohuiGuoCN/chatgpt-marker/blob/main/INSTALL.md)

**关于永久信任：** macOS 会记住对这个应用的打开例外；Safari 每次完全退出后，仍需重新允许未签名扩展。DMG 不能取消这个限制，但应用可以保留，不用每 24 小时重新下载安装。

没有 Apple 开发者证书签名、未公证；本地临时签名仅用于运行。包含 Apple 芯片与 Intel 通用程序；安装目标 macOS 14.2+ / Safari 17.2+，旧系统与 Intel 尚未实机验证。仅限 Mac，不支持 iPhone / iPad。

旧版 ZIP 用户请先导出 JSON 备份，停用旧临时扩展，再在 DMG 版中恢复。笔记不会自动转移。

**其他附件：** ZIP 备用临时扩展（退出或 24 小时后会移除）、安装指南、隐私说明、SHA-256 校验值。不要下载 GitHub 自动生成的 “Source code” 文件。

## PDF 现在可以保留公式排版

修复公式在 PDF 中缺失或只显示源码的问题。常见分数、根号、积分、矩阵和多行公式会重新排版，字体随扩展提供。无法识别的公式保留源码并提示。

- **整段对话**：荧光笔列表 → 设置 → 导出本段对话 PDF。
- **单条回复**：回复下方“分享” → 导出该回复 PDF。

两种方式都保留所属高亮与完整批注。在 Safari 打印窗口选择“PDF → 存储为 PDF”。

[整段对话 PDF 示例](https://chatgpt-marker.chaohui-97.chatgpt.site/samples/conversation.pdf) · [单条回复 PDF 示例](https://chatgpt-marker.chaohui-97.chatgpt.site/samples/reply.pdf) · [网站功能演示](https://chatgpt-marker.chaohui-97.chatgpt.site/#pdf)

示例为虚构内容，通过本机 Safari 实际导出，不包含真实用户对话。

## 验证与限制

62 项自动化测试通过，包含公式提取、重新排版、源码回退和单条回复范围检查。使用 Safari 打印流程导出虚构对话并检查公式、高亮与批注排版。完整 DMG 的真实 ChatGPT 页面验证仍受手动启用步骤限制；旧系统与 Intel 尚未实机验证。

整段 PDF 只包括页面已加载的对话；无法识别的公式保留源码，图片需要原图可访问。

[版本记录](https://github.com/ChaohuiGuoCN/chatgpt-marker/blob/main/CHANGELOG.md) · [隐私说明](https://github.com/ChaohuiGuoCN/chatgpt-marker/blob/main/PRIVACY.md)
