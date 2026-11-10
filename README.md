# MP3 Cover Tool

Add cover art to MP3 files, right in the browser. Works on iPhone, Android and desktop.
Nothing is uploaded: all processing happens on your device.

## Put it on GitHub and get a web link

1. Create a GitHub account and a **new public repository** (e.g. `mp3-covers`).
2. Upload all files from this folder to the repository root
   (`index.html`, `sw.js`, `manifest.webmanifest`, `icon-*.png`, `README.md`).
   Use **Add file -> Upload files** on the repository page.
3. Go to **Settings -> Pages**. Under *Build and deployment* choose
   **Deploy from a branch**, branch **main**, folder **/ (root)**, then **Save**.
4. After a minute the app is live at `https://YOUR-USERNAME.github.io/mp3-covers/`.

## Install on iPhone

1. Open the link in **Safari**.
2. Tap **Share -> Add to Home Screen**.
3. It now opens like an app and also works offline.

## Using it

1. Choose your MP3s (select several at once).
2. Choose one image (used for every file) or several images named like the songs
   (`song.mp3` gets `song.jpg`).
3. Tap **Embed covers**, then **Save / Share...** and pick **Save to Files**.
   On a computer use **Download ZIP**.

Your original files are never changed; you get new copies.

## Notes

- Existing tags (title, artist, album...) are kept. Any old cover is replaced.
- HEIC/WebP/etc. images are converted to JPEG automatically. The default max cover size is 800 px.
- Folders can't be selected on iPhone, so pick files directly. Do very large batches in groups.
- Old ID3v2.2 tags are replaced by a new ID3v2.3 tag (text tags in those rare files are lost).
- After you edit files in the repo, bump `VERSION` in `sw.js` so installed copies update.
