# Weak Kingsley Desktop Pet: Project Brief

## Goal
Build an interactive desktop pet featuring **Weak Kingsley** from *Cyberpunk: Edgerunners 2* (Netflix, Studio Trigger, 2026). He lives on the user's desktop, reacts to mouse and keyboard, and narrates what Claude Code is doing, in the style of the open-source project https://github.com/mochiiwuff/capri-desktop.

## Character
- **Name:** Weak Kingsley (formerly "King"), a veteran edgerunner who once was at the top of his game and now lives in the shadow of his former glory.
- **Voice (reference only):** Clancy Brown (English), Kentarou Tone (Japanese).
- **Tagline from the reveal:** "The weight of the crown is heavy."
- **Personality (to confirm with the owner after watching the show):** world-weary, sardonic, quietly caring underneath.
- **Art:** The owner holds a licence for the official images. Use them only as the owner's local reference and as permitted by that licence. Check the licence before committing any official images to a public repo.

## Platforms
- Must run on **macOS and Windows**.
- Code is pushed to **GitHub**. Repo: *(to be provided by the owner)*.
- License: the source project is PolyForm Noncommercial. Keep this project non-commercial and check license compatibility before forking.

## Reference projects
1. **capri-desktop** (https://github.com/mochiiwuff/capri-desktop): Electron app. The pet is a WebGL sprite with frame-by-frame animation, reacts to Claude Code hooks, sits on windows, and has a chat panel. It is Windows-only for the window-tracking features, so Mac needs its own version of that layer.
2. **Existing Weak prototype** in `Downloads/Weak_desktop_fig_foru/` (owner's folder). Electron app with `main.js`, `renderer.js`, `preload.js`, `styles.css`. It runs on Windows, Mac and Linux, with modes (idle, alert, scan, combat, charging), keyboard shortcuts (S/A/C/D/R, Ctrl+Alt+W, Ctrl+Alt+Q), and mouse gestures. Use it as the starting point for the character behaviour. Read it first, then decide what to keep.

## Requirements (first version)
- Transparent, always-on-top, click-through overlay that works on macOS and Windows.
- Weak idles, reacts to hover and clicks, and has a few poses/modes.
- A speech bubble shows short lines in Weak's voice.
- Optional: a hook that shows Claude Code activity (what it is doing, when it needs permission, when it is done).
- Start-up on login is optional, and the owner should be asked before it is enabled.
- Settings: size, show/hide shortcut, quit shortcut.

## Working rules
- Ask the owner before adding any feature that changes the system (hooks, login items, file access).
- Do not copy copyrighted Cyberpunk art or show frames into the public repo unless the licence allows it. Use placeholders until the owner confirms.
- Make it run on both platforms before calling any feature done. Test on each OS where possible and say which was not tested.
- Keep the README honest about what works on each platform.

## First steps for the coding session
1. Read the existing prototype in `Downloads/Weak_desktop_fig_foru/` and summarise what it does.
2. Propose the project structure and get the owner's approval.
3. Set up the Electron project so it runs on macOS and Windows with `npm start`.
4. Load a placeholder Weak sprite, get idle, hover and click working, and add speech bubbles.
5. Add the Claude Code hook as an optional step.
6. Push to GitHub once the owner has provided the repo URL.
