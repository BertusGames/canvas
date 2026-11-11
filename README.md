# Canvas Notes

A personal infinite canvas: notes, pasted screenshots and pen ink. Static files, no build step, no accounts. Your boards never leave your computer.

## Files

| File | What it is |
|---|---|
| `index.html` | The whole app (markup, styles, code) |
| `sw.js` | Makes it work offline |
| `manifest.webmanifest` | Makes it installable as an app |
| `icon-192.png`, `icon-512.png`, `icon-maskable-512.png` | App icons |

## Put it on GitHub Pages

1. On GitHub, create a new **public** repository, for example `canvas`.
2. **Add file → Upload files**, drop in all six files (not this README if you prefer), commit.
3. **Settings → Pages → Build and deployment**: Source = *Deploy from a branch*, Branch = `main`, folder = `/ (root)`, Save.
4. After a minute the app is at `https://<your-account>.github.io/canvas/`.

## Install it on the PC

1. Open that address in **Edge or Chrome**.
2. Click the install icon in the address bar (or ⋯ → Apps → Install this site as an app).
3. It now has its own window and taskbar icon, and opens without internet.

## Save boards as real files

Board menu (top left) → **Save boards to a folder…** → pick or create a folder such as `D:\Canvas`.

- Each board is one file: `<Board name>.<id>.board.json`
- Screenshots sit in `images\<id>\`
- Boards you already made in the browser move into the folder automatically.
- If the browser asks to open the folder again after a restart, it is one click. In the installed app you can choose "Allow on every visit".

Put that folder inside Google Drive or OneDrive if you want a backup for free.

## Pen tablet

The pen draws, the mouse selects and moves. The eraser end or the side button erases whole strokes.
If the pen behaves like a mouse (it pans instead of drawing, or lines have no pressure), switch on **Windows Ink** in the tablet driver settings. Until then, press **D** to draw with any pointer.

## Updating the app

Upload the changed files to the repository. The app loads instantly from its offline copy and fetches the new version in the background, so the change shows the **second** time you open it.

## Keys

| Key | Action |
|---|---|
| Double-click empty space | New note |
| Ctrl + V | Paste a screenshot (plain text becomes a note) |
| Drag empty space, Space + drag, middle button | Move around |
| Scroll wheel | Zoom toward the cursor |
| Shift + drag | Select several things |
| F / 0 | Fit everything / 100% |
| Ctrl + Z / Ctrl + Y | Undo / redo |
| Delete | Delete the selection |
| Ctrl + D | Duplicate |
| Ctrl + F | Search notes |
| [ / ] | Send to back / bring to front |
| Arrow keys | Nudge (Shift for bigger steps) |
| D | Draw with the mouse (right-drag erases) |
