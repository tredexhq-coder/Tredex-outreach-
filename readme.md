# TREDEX Email Outreach — Android PWA

## Files in this package
- `index.html` — The main app
- `sw-1.js` — Service worker (enables offline use + installation)
- `manifest.json` — PWA manifest (app name, icon, theme)
- `20261006_172013.png` — TREDEX logo and app icon

---

## How to install on Android

### Option A — Host on GitHub Pages (Free, Recommended)
1. Create a free GitHub account at github.com
2. Create a new repository (e.g. `tredex-app`)
3. Upload all 4 files (`index.html`, `sw-1.js`, `manifest.json`, `20261006_172013.png`)
4. Go to **Settings → Pages → Deploy from branch: main**
5. Your app URL will be: `https://YOUR-USERNAME.github.io/tredex-app/`
6. Open that URL in **Chrome on Android**
7. Tap the **⋮ menu → "Add to Home Screen"**
8. TREDEX appears on your home screen like a native app ✅

### Option B — Host on Netlify (Drag & Drop)
1. Go to netlify.com → "Deploy manually"
2. Drag the folder containing the app files, including the logo image
3. Get your live URL instantly
4. Open in Chrome on Android → Add to Home Screen

### Option C — Local server (Advanced)
If you have a local web server on your PC on the same Wi-Fi:
```bash
npx serve .   # or python3 -m http.server 8080
```
Then open `http://YOUR-PC-IP:8080` in Chrome on Android.

> ⚠️ PWAs cannot be installed from `file://` paths — they must be served over HTTP/HTTPS.

---

## Features added for Android
- ✅ **Install banner** — prompts user to add to home screen
- ✅ **Offline support** — works without internet once installed
- ✅ **Safe area insets** — respects notch/gesture bar
- ✅ **44px touch targets** — all buttons easy to tap
- ✅ **Haptic-friendly** — tap animation on buttons
- ✅ **Standalone display** — no browser UI when installed
- ✅ **Offline badge** — shows when device is offline
- ✅ **Smooth scrolling** — iOS/Android momentum scrolling on lists
- ✅ **Theme color** — orange status bar when installed
- ✅ **Content rotation** — write multiple email variants (A, B, C…) and rotate them across recipients in order or randomly; each recipient's variant is remembered
- ✅ **Campaign preflight** — checks pending addresses, duplicates, and complete subject/body content before a run
- ✅ **Run limits and recovery** — cap a run at 1–500 drafts and resume a paused campaign after reopening the app
- ✅ **Draft vs sent status** — draft handoffs and user-confirmed sent status are tracked separately; delivery is not verified
- ✅ **Recipient pagination** — browse 50 recipients per page, with filtering and sorting
- ✅ **Quick draft shortcut** — press `Alt` + `↓` outside a text field to open the next pending draft
