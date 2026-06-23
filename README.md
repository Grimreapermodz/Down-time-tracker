# Line Downtime Tracker — PWA

A fully offline-capable Progressive Web App for tracking production line downtime.

---

## Files

```
index.html    ← The app (all logic self-contained)
sw.js         ← Service worker (enables offline use)
manifest.json ← PWA install metadata
icon-192.svg  ← App icon (home screen)
icon-512.svg  ← App icon (splash screen)
```

---

## Deploy to GitHub Pages (one-time setup)

1. Go to [github.com](https://github.com) and sign in (or create a free account)
2. Click **+** → **New repository**
3. Name it `line-tracker` (or anything you like), set it to **Public**, click **Create repository**
4. Click **uploading an existing file**, drag in all 5 files above, click **Commit changes**
5. Go to **Settings** → **Pages** → under *Branch* select `main` → click **Save**
6. After ~1 minute your app is live at:
   `https://YOUR-USERNAME.github.io/line-tracker/`

---

## Install to Android home screen

1. Open the URL above in **Chrome** on your Android phone
2. Tap the **⋮ menu** → **Add to Home screen**
3. Tap **Add** — it installs like a real app
4. Open it once with Wi-Fi to cache everything, then it works **100% offline**

---

## Updating the app

When changes are made to `index.html`:

1. Download the new `index.html`
2. Go to your GitHub repo → click `index.html` → click the **pencil ✏️ edit icon**
3. Delete all the old content, paste in the new content → click **Commit changes**
4. The next time you open the app on your phone, a blue **"Update available"** banner
   will appear at the bottom — tap it to apply instantly. No reinstall needed.

---

## Log persistence

Entries are saved to your device's local storage automatically.
They survive closing the app and rebooting your phone.
Tapping **Clear** in the log permanently removes them.
