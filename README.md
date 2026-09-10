**English** | [中文](README.zh-CN.md)

# ChatGPT Marker

**Long answers? Highlight the point. Questions or disagreement? Add a note. Several things unclear? Collect them into one follow-up.**

ChatGPT Marker is a desktop Chrome extension and a Safari extension for Mac. Both versions share the same features. Highlight text in ChatGPT, keep your thoughts beside the source, and copy selected quotes and notes together or add them to your draft. You can also **export a conversation or a single reply as a PDF with formulas, highlights and complete notes**.

**[Add to Chrome](https://chromewebstore.google.com/detail/chatgpt-marker/dbhfheghjjebbkjjpgmdgeagnckljcoa)** · [Website and examples](https://chatgpt-marker.chaohui-97.chatgpt.site/?lang=en) · [Download Chrome ZIP](https://github.com/ChaohuiGuoCN/chatgpt-marker/releases/download/v0.6.0/ChatGPT-Marker-Chrome-v0.6.0.zip) · [Download Safari DMG preview](https://github.com/ChaohuiGuoCN/chatgpt-marker/releases/download/v0.6.0/ChatGPT-Marker-Safari-v0.6.0-unsigned.dmg) · [GitHub Releases](https://github.com/ChaohuiGuoCN/chatgpt-marker/releases)

Current version: **v0.6.0 · Chrome + Safari**. Chrome: install directly from the Chrome Web Store, with no developer mode required. Safari: install the Mac app from the unsigned DMG; unsigned-extension permission must be renewed after fully quitting Safari.

## Three common problems, three practical answers

| The problem | What Marker does | What you gain |
| --- | --- | --- |
| Long replies bury the key point. You have to find it again later. | **Highlight text** in four colors. | The important part stays visible in its original context. |
| Advice does not fit your situation, or a phrase is unclear. | **Add a note beside the source** with your perspective or question. | Remember why you disagreed or what you did not understand. |
| Copying unfamiliar terms one by one is tedious. | **Select and collect items** into one copy or draft insertion. | Bring the source text and your questions together for a follow-up. |

The following fictional examples all start with one question: **“How should I learn Python to build an expense tracker?”**

## 1. Long answers: highlight the sentence you need

ChatGPT covers syntax, tools, study schedules and testing. You may only want to remember what to do today.

> Start with variables, lists and functions. Install your tools, learn to run a file, then practice input and output. Combine tutorials, documentation and exercises…
>
> You do not need a complete interface to start an expense tracker. **🟨 Save a single transaction, then practice calculating the total.** Once that works, add monthly searches, file exports and category totals.
>
> Later, explore storage, error handling and testing. After each feature, review what you learned and plan the next step…

**The solution:** select the bold sentence and choose yellow. When you return, your first step is easy to find without reading the whole answer again.

Choose yellow, green, blue or pink. **Double-click within 4 seconds of selecting text** to reuse the last color.

## 2. Questions or disagreement: keep your thoughts beside the text

A highlight alone may not remind you why you disagreed or what confused you. Notes keep those thoughts with the source.

| Example source | My note |
| --- | --- |
| “Study for three uninterrupted hours each day.” | **[1]** I only have 30 minutes a day. Can you adapt the plan? |
| “Then cover the edge cases.” | **[2]** What does “edge cases” mean here? Does a zero balance count? |

The first note explains **why the advice does not fit**; the second records **a phrase that needs clarification**.

**The solution:** select the text and click the note icon. Notes appear in the margins and can be collapsed. Click a numbered reference to open the matching note and scroll to it. You can also **triple-click within 4 seconds of selecting text** to insert a note.

## 3. Several unclear terms: collect them into one draft

“Minimal working example”, “edge cases” and “unit tests” are scattered through the answer. Repeatedly selecting, copying and switching to the composer makes it easy to miss one.

Mark the terms and write your questions:

- [x] **Minimal working example** — Can you show an example in 10 lines or fewer?
- [x] **Edge cases** — Which edge cases should an expense tracker handle?
- [x] **Unit tests** — Can you demonstrate a test using a single transaction?

**The solution:** open the highlights list, select these items, then choose **Copy** or **Add to draft**. Color buttons can select all items of one color.

The English collection format keeps quotes and notes together:

```text
[1]
Source:
Minimal working example

Note:
Can you show an example in 10 lines or fewer?

──────────

[2]
Source:
Edge cases

Note:
Which edge cases should an expense tracker handle?

──────────

[3]
Source:
Unit tests

Note:
Can you demonstrate a test using a single transaction?
```

**Copy** only writes to the clipboard. **Add to draft** appends to the existing draft, **which you review and send manually**. Questions come from your own notes; the extension does not generate or send them. Plain highlights can also be collected and show “(No note)” when no note was added.

## PDF export: keep a conversation or just one reply

Save an explanation for review, share a plan or archive a discussion without taking screenshots or rebuilding the layout.

| What to save | Where to export | What the PDF includes |
| --- | --- | --- |
| **A conversation** | Highlights → Settings → Export conversation PDF | Loaded questions and answers, formulas, tables, code, source links, highlights and complete notes |
| **One reply** | Share below that reply → Export this reply as PDF | Only that reply’s content, formulas, highlights and notes |

In Chrome, choose **Destination → Save as PDF**. In Safari, choose **PDF → Save as PDF**. The extension does not create a public share link.

**Fictional example:** ask for an explanation of the quadratic formula. Highlight “Calculate the discriminant first to find the number of real roots” and add “Find Δ first, then use the quadratic formula.” The PDF keeps the typeset fractions and square roots, yellow highlight and note.

[Conversation PDF example — Chinese content](https://chatgpt-marker.chaohui-97.chatgpt.site/samples/conversation.pdf) · [Single-reply PDF example — Chinese content](https://chatgpt-marker.chaohui-97.chatgpt.site/samples/reply.pdf)

![Exported PDF with formulas, highlights and notes; fictional example in Chinese](https://chatgpt-marker.chaohui-97.chatgpt.site/samples/pdf-preview.png)

Common formulas are typeset locally with bundled fonts. Unrecognized formulas retain readable content and show a notice. Scroll up to load long conversations before exporting; images must be accessible at their source URLs. JSON backups restore editable notes, while PDFs are for reading, printing and sharing.

## English / 中文

English is the default on first use. A language you choose manually is remembered.

- **Website:** use 中文 / English in the header. The URL can include `?lang=en` or `?lang=zh`.
- **Extension:** open Highlights → Settings → Interface language, or use the browser toolbar popup. The preference is saved and shared across extension tabs.
- **PDF preview:** use its language selector to change generated headings and print instructions.
- **Mac app and installation guide:** use 中文 / English at the top. The app and website keep their own preferences.
- **GitHub:** use the language links at the top of each document.

Language changes affect interface labels and collection-format headings. **Your conversation text, notes and formulas remain unchanged.**

## Download and install

### Chrome

1. Open **[ChatGPT Marker in the Chrome Web Store](https://chromewebstore.google.com/detail/chatgpt-marker/dbhfheghjjebbkjjpgmdgeagnckljcoa)**.
2. Click **Add to Chrome**, review the permissions, and confirm **Add extension**.
3. Open or refresh a saved ChatGPT conversation and start highlighting or adding notes.

For desktop Chrome on macOS, Windows and Linux. Use an up-to-date version. Mobile Chrome is not supported. Hardware testing is still pending. The store version requires neither developer mode nor an installation folder.

**Switching from a manual installation:** export a JSON backup from the old version first, then restore it in the store version. Check your notes before removing the old installation. Do not enable both copies at once.

**Move Safari notes to Chrome:** export a JSON backup in Safari, then restore it in Chrome. Notes do not sync automatically between browsers.

[Full Chrome installation guide](INSTALL-CHROME.md) · [Alternative: manual-install ZIP](https://github.com/ChaohuiGuoCN/chatgpt-marker/releases/download/v0.6.0/ChatGPT-Marker-Chrome-v0.6.0.zip)

### Safari on Mac

Download **ChatGPT-Marker-Safari-v0.6.0-unsigned.dmg**, not GitHub’s automatically generated “Source code” files.

1. Open the DMG, drag **ChatGPT Marker.app** to **Applications**, then eject the disk image.
2. Open the app from Applications. If macOS blocks it, go to **System Settings → Privacy & Security → Open Anyway** and follow the system prompts.
3. Safari → Settings → Advanced → Show features for web developers. Then **Developer → Allow unsigned extensions**.
4. Click **Open Safari Extension Settings** in the app. Enable ChatGPT Marker and allow access to `chatgpt.com`.
5. Refresh a saved ChatGPT conversation and start marking.

**Permanent trust?** macOS remembers the app’s “Open Anyway” exception, but Safari permission is separate. After fully quitting Safari, you must allow unsigned extensions again. The app remains installed; the DMG does not require a download or temporary-folder installation every 24 hours.

Before switching from the old ZIP, export a JSON backup and restore it after enabling the DMG version. Notes do not transfer automatically. Do not enable both copies at once.

Targets macOS 14.2+ / Safari 17.2+. Includes Apple silicon and Intel builds; older systems and Intel Macs have not been tested on hardware. iPhone and iPad are not supported. Local ad-hoc signing allows Apple silicon to run the app; this is not Apple developer signing or notarization.

[Install, update and uninstall](INSTALL.md) · [Privacy](PRIVACY.md) · [Changelog](CHANGELOG.md)

## Project and licensing

An independent project, not affiliated with OpenAI, ChatGPT, Google or Apple. This repository distributes runtime files and documentation, not development source code, and does not grant an open-source license. Browser extension runtime files contain JavaScript.

Formula rendering uses KaTeX. Its MIT license is included in `katex/LICENSE` in the package and does not change this project’s source distribution scope.
