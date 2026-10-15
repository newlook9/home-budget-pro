# Home Budget Pro / ہوم بجٹ پرو

Offline personal & household budget manager. One HTML file, no server, no internet needed.
English + اردو (RTL). Data stays in your browser (localStorage). Use **Backup & Restore** to download JSON backups.

**Live app (GitHub Pages):** `https://YOUR-USERNAME.github.io/home-budget-pro/`

## Use locally
Download `index.html` and double-click it.

## Publish on GitHub Pages
1. Create a new public repository named `home-budget-pro`.
2. Upload `index.html`, `.nojekyll` and `README.md` (Add file -> Upload files -> Commit).
3. Repository **Settings -> Pages -> Build and deployment**: Source = *Deploy from a branch*, Branch = `main`, Folder = `/ (root)` -> Save.
4. Wait 1-2 minutes; the link appears at the top of the Pages screen.

Or with git:
```
git init
git add .
git commit -m "Home Budget Pro"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/home-budget-pro.git
git push -u origin main
```

Note: each browser/device/site address keeps its own data. Data saved from the local file is not shared with the GitHub Pages link; move it with a JSON backup.

Developed by Muhammad Ashraf - 03083286645

## Install as an app (PWA) / ایپ کی طرح انسٹال
After opening the GitHub Pages link once with internet, the app is cached and works fully offline.
- **Android (Chrome):** menu (three dots) -> *Install app* / *Add to Home screen*.
- **iPhone (Safari):** Share -> *Add to Home Screen*.
- **Windows/Mac (Chrome/Edge):** install icon in the address bar.
Service worker needs `https` (GitHub Pages is https); it does not run from a local `file://` copy.
To force an update after changing `index.html`, increase the version number of `hbp-v2` in `sw.js` (e.g. `hbp-v3`).
