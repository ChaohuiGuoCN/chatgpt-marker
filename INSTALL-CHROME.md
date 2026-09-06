**English** | [中文](INSTALL-CHROME.zh-CN.md)

# Chrome installation · v0.6.0

Download **ChatGPT-Marker-Chrome-v0.6.0.zip** from [GitHub Releases](https://github.com/ChaohuiGuoCN/chatgpt-marker/releases/tag/v0.6.0) or the [website](https://chatgpt-marker.chaohui-97.chatgpt.site/?lang=en#install). Do not download GitHub's automatic “Source code” archive or the Safari DMG.

This is a desktop Chrome extension, installed with developer mode. It has not been published in the Chrome Web Store. The package targets Chrome 105+ on macOS, Windows and Linux; use an up-to-date Chrome. This preview has not yet completed hardware testing. Mobile Chrome is not supported.

## Install

1. Extract the ZIP. Move **ChatGPT-Marker-Chrome** to a permanent folder. It must directly contain `manifest.json`, `content.js` and `pdf.html`.
2. Enter `chrome://extensions/` in Chrome's address bar.
3. Turn on **Developer mode** at the top right.
4. Click **Load unpacked** and select **ChatGPT-Marker-Chrome**, not the ZIP or its parent folder.
5. Open or refresh a saved conversation at `https://chatgpt.com/c/…`. The laser pointer and highlighter appear at the page edge.

Keep the folder where it is: Chrome loads the files from that location. Do not remove the extension when updating. This installation has no Safari-style 24-hour expiration. An organization-managed browser may restrict developer-mode extensions.

## The same features as Safari

- Highlight selected text in yellow, green, blue or pink. Within 4 seconds of selecting text, double-click to reuse the last color, or triple-click to add a note.
- Write notes next to their source; collapse them or use numbered links to jump to them. Drag the pen tools to move them and snap them to an edge.
- Select items individually or by color. **Copy** writes to the clipboard; **Add to draft** appends quotes and notes without sending. Each item also has its own Copy button.
- Use the laser pointer for presentations. Press **Alt/Option + Shift + L** to toggle it, **Alt/Option + Shift + H** to highlight a selection, and **Esc** to exit the laser pointer.
- Export the loaded conversation via **Highlights → Settings → Export conversation PDF**, or one reply via **Share below the reply → Export this reply as PDF**. In Chrome's print dialog, choose **Destination → Save as PDF → Save**. Formulas, highlights and full notes are retained. No public share link is created.
- Back up and restore marks as JSON. Choose English or 中文 in Settings, the toolbar popup or the PDF preview. English is the initial default; your choice is remembered.

## Move notes from Safari

In Safari, open the highlights list and click **Backup**. In Chrome, open the list and click **Restore**, then select that JSON file. Open the same ChatGPT conversation to see its notes. Browser storage is separate; notes do not sync automatically. Backup files contain your selected text and notes and stay on your device unless you share them.

## Update or uninstall

Before updating, export a JSON backup. Extract the new ZIP and replace the contents of the **same installed folder**, preserving its name and location. Click the extension's **Reload** button at `chrome://extensions/`, then refresh ChatGPT. Loading a second folder may create a separate installation with separate notes.

Before uninstalling, back up your notes. Click **Remove** at `chrome://extensions/`, then delete the folder if no longer needed. Uninstalling may delete the extension's stored data.

## Troubleshooting

- **Could not load manifest:** choose the folder directly containing `manifest.json`.
- **No pen tools:** confirm the extension is enabled and allowed on `chatgpt.com`, then refresh the chat. Empty new chats and temporary chats do not support saved marks.
- **PDF content missing:** reopen the export from the chat. Scroll up first to load long conversations. Images must be accessible at their original URLs; unsupported formulas retain readable content and show a notice.
- **After an update:** reload the extension and the ChatGPT page; refreshing only the page does not reload extension files.

[Google's installation instructions](https://developer.chrome.com/docs/extensions/get-started/tutorial/hello-world#load-unpacked) · [Privacy](PRIVACY.md)
