**English** | [中文](CHANGELOG.zh-CN.md)

# Changelog

## v0.6.0 · September 7, 2026 · Chrome support

- Added a desktop Chrome ZIP using the same feature code as Safari: highlights, notes, gestures, laser pointer, collection, backups and both PDF export modes.
- Fixed the PDF preview to use Chrome extension storage as well as Safari storage.
- Kept local formula rendering and English-by-default language switching.
- Added Chrome installation and cross-browser backup instructions in English and Chinese.
- Added separate Chrome and Safari downloads on the website.
- Validation: 74 automated tests passed, including Chrome and Safari PDF-preview and popup integration checks. Chrome hardware testing is pending.

## v0.5.1 · September 6, 2026 · English by default

- English is now the initial language for the website, extension, Safari popup, PDF preview, Mac app and installation guide.
- The GitHub README, installation, privacy and changelog pages open in English, with links to the Chinese editions. Existing English links remain available.
- Chinese switching and saved language choices remain supported. Conversation text, notes and formulas are unchanged.

## v0.5.0 · September 6, 2026 · Chinese and English

- Added persistent Chinese/English switching to the website, extension settings, Safari popup, PDF preview, Mac app and installation guide.
- Translated feature examples, messages, copy-format headings, PDF labels and installation guidance. Conversation text, notes and formulas are preserved exactly.
- Added English GitHub documentation with language links, including installation, privacy and release notes.
- Switching languages preserves selected items, note drafts and the laser pointer state. Extension tabs share the language preference; the website and Mac app store their own preference.
- Retained the Safari formula fixes from v0.4.4.

## v0.4.4 · September 6, 2026 · Safari formula compatibility

- Fixed formulas becoming plain text when ChatGPT stores TeX on an outer Safari DOM wrapper.
- Reads `data-math-source` and formula `aria-label`, preserving Chinese underbrace labels, accents, subscripts, superscripts and large parentheses.
- Applies to conversation and single-reply export without duplicating formulas; preserves highlights and notes.
- Warns when formula source is missing instead of presenting fallback text as a properly typeset result.
- Passed 64 automated tests and checked formula extraction and rendering on the reported real page.

## v0.4.3 · September 6, 2026 · PDF formulas and examples

- Fixed missing formulas and raw TeX in PDFs by typesetting common formulas with bundled fonts.
- Added inline and display math, fractions, roots, integrals, matrices, piecewise and multiline formulas. Preserves safe MathML without TeX; keeps readable fallback content and warns on failure.
- Fits long formulas to print width and preserves highlights spanning formulas.
- Added conversation and single-reply PDF sections, instructions and exported fictional samples to the website and GitHub.
- Passed 62 automated tests and verified formula, highlight and note layout through Safari printing.

## v0.4.2 · September 6, 2026 · DMG preview

- Added a free DMG containing the Mac app and Safari extension.
- Universal Apple silicon and Intel app targeting macOS 14.2+ / Safari 17.2+. Older systems and Intel were not tested on hardware.
- Added a Safari settings shortcut and local guide explaining macOS app permission and Safari extension permission separately.
- The app stays installed, but unsigned-extension permission must be renewed after quitting Safari; no permanent trust.
- Included an alternative ZIP, JSON migration instructions and SHA-256 checksums.
- Retained highlighting, notes, batch collection and PDF functionality from v0.4.1.

## v0.4.1 · September 6, 2026 · First public preview

- Released the Mac Safari temporary-extension ZIP, installation guide and privacy notice.
- Four highlight colors, quick double-click highlighting, triple-click notes, margin notes and numbered navigation.
- Item selection, selection by color, single-item copying and insertion into the ChatGPT draft.
- Draggable tools that snap to the edge, plus a laser pointer.
- PDF export for loaded conversations and individual replies with highlights and complete notes.
- Fixed oversized ChatGPT citation icons in PDFs while keeping source links.

Validation: 56 automated tests, type checking and builds passed. Highlighting, notes, copying and PDF export were checked in local Safari 26.5.2 on real ChatGPT pages.

Limitations of this historical version: temporary extension loading; removal after quitting Safari or 24 hours; no developer signing or notarization; Mac only. PDFs included loaded messages, formulas as source text and images only when the original URLs were accessible.
