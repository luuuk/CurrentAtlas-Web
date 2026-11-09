# Current Atlas Web App

This is a mobile-first web conversion of the supplied Swift Playground project.

## Run locally
Open `index.html` in a desktop browser for a quick preview. GPS and offline installation require HTTPS (or localhost).

## Put it on your iPhone (recommended: GitHub Pages)
1. On a computer, create/sign in to a GitHub account.
2. Create a **public** repository named `current-atlas` (or another name).
3. Unzip this package. Upload the *contents* of the `CurrentAtlas-Web` folder (including `index.html`, `assets/`, `app.js`, `sw.js`, etc.) to the repository root. Do not upload only the zip file.
4. In the repository, open **Settings → Pages**. Under Build and deployment choose **Deploy from a branch**, select `main` and `/ (root)`, then Save.
5. Wait for GitHub Pages to publish. Your URL will look like `https://YOUR-USERNAME.github.io/current-atlas/`.
6. On your iPhone, open that URL in **Safari** (not an in-app browser). Wait for the maps to load once; the service worker caches the app and all atlas map PNGs for offline use. The first visit may take a little while because the atlas images are large.
7. Tap **Share** (square with arrow) → **Add to Home Screen** → optionally enable **Open as Web App** → **Add**. Launch it from the new Home Screen icon.

## Notes
- Location access requires HTTPS and your permission. GPS is used to select the matching atlas region and place the blue location marker.
- The date/time lookup uses the atlas's `America/Los_Angeles` Pacific time zone and its included 2026 lookup table.
- Browser storage remembers the selected region and favorites on this device.
- Offline use starts after the first successful load/cache. Do not clear Safari website data if you want to retain the cached app.
- This web app is a conversion of the supplied project, not an official publication of the atlas. Respect the atlas author's terms for the maps and data.
