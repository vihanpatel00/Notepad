# Notepad

A simple web-based rich text editor. This repository contains an editable Notepad with formatting, autosave, and export features.

Features
- Rich-text editing using contenteditable and document.execCommand (works in most modern browsers).
- Selection-preserving toolbar so formatting buttons don't lose the current selection.
- Autosave to localStorage (key: `notepad_content_v1`).
- Export as plain text (.txt) and export HTML (.html).
- Ready to be published via GitHub Pages from the `docs/` folder.

Files added
- `Notepad.html` — an HTML version of the editor (kept in repo root).
- `docs/index.html` — same editor published for GitHub Pages.
- `Notepad.me.bak` — backup copy of the original Notepad.me file.
- `Notepad.me` — updated to point to the published HTML.

Viewing the app (GitHub Pages)
After the Pages workflow runs, the site will be published at:

https://vihanpatel00.github.io/Notepad/

How to run locally
1. Download or clone the repository.
2. Open `Notepad.html` (or `docs/index.html`) in a modern browser (Chrome/Firefox/Edge/Safari).

Notes
- `document.execCommand` is deprecated but still supported by most browsers today. For a long-term solution consider integrating a modern editor library (Quill, Slate, ProseMirror).