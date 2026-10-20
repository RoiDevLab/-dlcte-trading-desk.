# DLCTE Trading Desk — PWA package

This package is ready to deploy as a static website. Once hosted on an HTTPS URL, it can be added to an iPhone Home Screen and supports offline app-shell loading after the first successful visit.

## Easiest route: GitHub Pages

1. Sign in to GitHub and create a new repository, e.g. `dlcte-trading-desk`.
2. Upload **all four files** from this folder (`index.html`, `manifest.webmanifest`, `sw.js`, `icon.svg`) to the repository root.
3. In the repository, open **Settings → Pages**.
4. Under build/deployment, choose **Deploy from a branch**, select the `main` branch and `/ (root)`, then Save.
5. Wait for GitHub Pages to publish the site. Open the published HTTPS URL on your iPhone in **Safari**.
6. In Safari, tap **Share → Add to Home Screen**. If shown, enable **Open as Web App**, then tap **Add**.

## Important data note

The watchlist and journal are stored in the browser's local storage on each device. They do **not** automatically sync between iPhone and laptop. Use Export backup / Import backup to transfer your data. Keep a backup before clearing website data.

## Updating the app

Upload the changed files to the same repository. The service worker caches the app shell for offline loading. After an update is published, close and reopen the app while online if the old version remains visible.
