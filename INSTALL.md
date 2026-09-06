**English** | [中文](INSTALL.zh-CN.md)

# Installation and use · v0.6.0

**Chrome users:** follow the [Chrome ZIP installation guide](INSTALL-CHROME.md). The instructions below are for Safari on Mac.

## Safari on Mac

Download **ChatGPT-Marker-Safari-v0.6.0-unsigned.dmg**. This free preview has no Apple developer signature or notarization. Local ad-hoc signing allows it to run on Apple silicon.

Targets macOS 14.2+ and Safari 17.2+. Includes Apple silicon and Intel builds. Older systems and Intel Macs have not been tested on hardware. iPhone and iPad are not supported.

## Install the DMG

1. Open the DMG and drag **ChatGPT Marker.app** to **Applications**. Eject the disk image when copying finishes. Do not run the app directly from the DMG.
2. Open ChatGPT Marker from Applications. If macOS blocks it, dismiss the warning and go to **System Settings → Privacy & Security → Open Anyway**. Follow the system prompts. macOS remembers the app exception; an update may require confirmation again.
3. Safari → Settings → Advanced → **Show features for web developers**.
4. Settings → Developer → **Allow unsigned extensions**. Complete any system authentication yourself.
5. Click **Open Safari Extension Settings** in the app, or go to Safari → Settings → Extensions. Enable ChatGPT Marker and allow access to `chatgpt.com`.
6. Refresh a saved ChatGPT conversation. When the pen tools appear at the edge, select text and choose a color or the note icon.

## Language

English is the default on first use. A saved Chinese preference is respected.

Use **中文 / English** at the top of the Mac app or installation guide. In ChatGPT, open **Highlights → Settings → Interface language**, or change it in the Safari toolbar popup. The extension remembers its language across tabs. The website and Mac app remember their own preferences. PDF previews also have a language selector. Your source text and notes are never translated automatically.

## Permanent trust and later use

- **macOS app permission:** remembers the “Open Anyway” exception for this app, not blanket trust for all future software from its developer.
- **Safari extension permission:** Safari resets “Allow unsigned extensions” when you quit. Enable it again next time and, if necessary, re-enable the extension. A DMG cannot provide permanent trust.
- **Reinstallation:** keep the app in Applications. This is an app-installed extension, not a temporary folder; no new download is required every 24 hours. Closing a window is different from fully quitting Safari.

## Migrate from a temporary ZIP installation

1. Export a JSON backup from the old highlights list while that extension is still available.
2. Disable the old temporary extension in Safari and keep the backup. Do not run both copies at once.
3. Install and enable the DMG version, refresh ChatGPT, then choose **Restore** in the list and select your JSON backup.
4. Confirm your notes were restored before removing the old temporary extension.

The two installation methods use different extension identities. Notes do not transfer automatically. Installing or updating the app does not read old backup files; choose the backup yourself to restore it.

## Common actions

- **Highlight:** select text and choose a color. Double-click within 4 seconds to reuse the last color; triple-click to add a note. Option + Shift + H also highlights.
- **Copy:** open the highlights list, select items with checkboxes or color buttons, then choose Copy. Add to draft appends to the composer without sending.
- **PDF:** Highlights → Settings → Export conversation PDF, or Share below a reply → Export this reply as PDF. Choose PDF → Save as PDF in Safari’s print dialog.
- **Backup:** Highlights → Back up saves a JSON file. Use Restore to import it.
- **Laser pointer:** click the upper tool button or press Option + Shift + L. Esc exits.

Conversation export includes loaded questions and answers and saved highlights and notes, regardless of checkbox selection. Scroll up to load long conversations first. Bundled fonts support fractions, roots, subscripts, superscripts, integrals, matrices and piecewise formulas. Without TeX, the extension attempts to preserve safe MathML. Unrecognized formulas retain readable content with a preview notice. Missing images also produce a notice.

## Update and uninstall

Back up first. Quit ChatGPT Marker, then replace the old app in Applications with the one from the new DMG. Refresh ChatGPT and check Safari’s extension and website permissions. The DMG extension identifier remains the same across updates, but backups are still recommended.

Before uninstalling, back up, disable the extension in Safari, remove the app and refresh the page. Do not assume data survives uninstalling.

## Troubleshooting

- **Missing from Extensions:** ensure the app is in Applications and has been opened at least once. Allow unsigned extensions, then reopen Safari’s Extensions settings.
- **No pen tools:** check that the extension is enabled and has website access, then refresh. Open a saved `/c/…` or `/share/…` page; empty and temporary chats do not save marks.
- **Blocked after an update:** use macOS Open Anyway. You do not need to disable system-wide security protections.

## Alternative ZIP installation

**ChatGPT-Marker-Safari-v0.6.0.zip** can be loaded temporarily. Extract it, then use Safari Settings → Developer → Add Temporary Extension and select the ChatGPT-Marker folder containing `manifest.json`. Safari removes this temporary installation after quitting or 24 hours. Prefer the DMG for everyday testing.

## Official documentation

- [Apple: Running a Safari Web Extension](https://developer.apple.com/documentation/safariservices/running-your-safari-web-extension)
- [Apple: Distributing a Safari Web Extension](https://developer.apple.com/documentation/safariservices/distributing-your-safari-web-extension)
- [Apple: Open an app from an unidentified developer](https://support.apple.com/guide/mac-help/mh40616/mac)
