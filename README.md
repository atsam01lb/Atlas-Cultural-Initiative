# Atlas Cultural Initiative — Hero

This is the standalone hero page for Atlas, ready to push to GitHub.

## Drop your background here

The hero looks for a background image at:

```
assets/img/hero-bg.jpg
```

Once you upload your two images, save the chosen hero background as `hero-bg.jpg` (or `.png` / `.webp` — just update the path in `assets/css/style.css` line ~226 if you use a different extension).

A dark gradient overlay sits on top of the image so the white headline stays readable. You can adjust the overlay strength in `style.css` under `.hero-overlay`.

## Files

```
.
├── index.html
├── README.md
└── assets/
    ├── css/style.css
    ├── js/main.js
    └── img/
        ├── atlas-logo.png        ← your logo, used in the header
        ├── favicon.ico           ← multi-size browser tab icon
        ├── favicon-16.png
        ├── favicon-32.png
        ├── favicon.png           ← 256×256
        ├── apple-touch-icon.png  ← 180×180 for iOS
        └── hero-bg.jpg           ← ADD THIS — your hero background
```

## Push to GitHub

```bash
git init
git add .
git commit -m "Atlas hero"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/atlas-cultural-initiative.git
git push -u origin main
```

For clean URLs (no `.html`), deploy on **Netlify** (drag-drop the folder at netlify.com/drop) or **Vercel**. Both are free.

## Local preview

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Animations included

- Logo bars rotate slightly on hover
- Hero headline rises in line by line
- Eyebrow, lede, and buttons fade up in sequence
- Background image performs a slow Ken-Burns zoom
- Floating world-icon SVGs drift up and down
- Globe icons spin slowly
- Four signature bars stretch in across the bottom
- Scroll hint pulses at the bottom center
- Header fades to a blurred dark bar when you scroll
- All animations honor `prefers-reduced-motion`

---

© Atlas Cultural Initiative 2026
