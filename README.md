# Jean Learns! — PWA bundle

This is the web-app version that PWABuilder turns into an installable Android APK for Jean's Fire tablet.

## Files

- `index.html` — the app
- `manifest.json` — PWA metadata (name, icons, colors)
- `sw.js` — service worker (offline support, required for PWABuilder)
- `icons/icon-192.png`, `icons/icon-512.png`, `icons/icon-512-maskable.png` — app icons

## What to do with this folder

See the parent folder's `INSTALL_FIRE_KIDS.md` for the full step-by-step. The short version:

1. Push this `pwa/` folder to a new public GitHub repo.
2. Enable GitHub Pages (Settings → Pages → main branch / root).
3. Wait ~1 minute for the URL to go live.
4. Paste the URL into [pwabuilder.com](https://www.pwabuilder.com).
5. Click "Package for Stores" → "Android" → download the signed APK.
6. Sideload the APK to the Fire and add it to Jean's profile in the Parent Dashboard.

## Local testing

Open `index.html` in any browser to use the app directly. The service worker only registers when served over HTTP(S), so for `file://` access you'll see a console warning that you can ignore.
