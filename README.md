# ShiftFill website

Static landing page (plain HTML/CSS/JS, no build step) ready for GitHub Pages.

```
shiftfill-site/
├── index.html
├── .nojekyll                   # tells GitHub Pages to serve files as-is
├── css/styles.css
├── js/main.js
└── assets/
    ├── img/favicon.svg
    └── video/
        └── shiftfill-demo.mp4  # ← put your video here
```

## Adding the video

1. Rename your file to `shiftfill-demo.mp4` (lowercase, no spaces).
2. Put it in `assets/video/`.
3. Commit and push it with the rest of the site.

To use a different file name, change this line in `index.html`:

```html
<source src="assets/video/shiftfill-demo.mp4" type="video/mp4">
```

Tips:
- Keep it under ~25 MB. GitHub rejects files over 100 MB and warns above 50 MB.
- Export as H.264 (MP4) with AAC audio so it plays in every browser.
- Optional poster image: add `poster="assets/img/video-poster.jpg"` to the `<video>` tag.

## Before you publish

Search `index.html` for `you@example.com` and `(000) 000-0000` and replace them with your real contact details.

## Deploying to GitHub Pages

1. Create a new repository on GitHub, for example `shiftfill`.
2. Upload the **contents** of this folder so `index.html` is at the root of the repo.
3. Go to **Settings → Pages**, set **Source** to *Deploy from a branch*, then pick branch `main` and folder `/ (root)`. Click Save.
4. After about a minute the site is live at `https://<your-username>.github.io/shiftfill/`.

To use your own domain, add it under **Settings → Pages → Custom domain**.
