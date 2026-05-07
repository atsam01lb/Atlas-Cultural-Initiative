# Atlas Cultural Initiative — Home

Full home page for Atlas, light theme, ready for GitHub.

---

## 📸 Where to add your photos

You can add images in **3 places** on the home page. All optional — the page works without them.

Drop image files into the **`assets/img/`** folder using these exact filenames, and they'll appear automatically. Recommended formats: `.jpg` or `.webp`.

### 1. Hero background — `assets/img/hero-bg.jpg`

Sits behind the headline at the very top.
- **Recommended:** subtle, light, travel/world themed (e.g. a faded map, distant landscape, soft cultural texture)
- **Size:** at least 1600×900 px
- The CSS automatically fades it to 18% opacity so the text stays readable on white.

### 2. About section background — `assets/img/about-bg.jpg`

(Optional — currently inactive in CSS. Leave blank or tell me to enable it.)

### 3. CTA banner background — `assets/img/cta-bg.jpg`

Sits behind the "Host culture in your space" dark section near the bottom.
- **Recommended:** atmospheric, evening-mood, hospitality/venue/world theme
- **Size:** at least 1600×600 px
- The CSS darkens it automatically.

### Bonus — replace the colored event covers with real photos

Right now the upcoming events show colored blocks with text (日本, Hola, VR). To use real photos:

1. Save photos as `assets/img/event-japan.jpg`, `assets/img/event-spanish.jpg`, `assets/img/event-vr.jpg`
2. In `index.html`, find the event cards and change:
   ```html
   <div class="event-cover" style="background:#D63A2F">
   ```
   to:
   ```html
   <div class="event-cover" style="background-image: url('assets/img/event-japan.jpg')">
   ```

---

## Files

```
.
├── index.html
├── README.md
├── .gitignore
└── assets/
    ├── css/style.css
    ├── js/main.js
    └── img/
        ├── atlas-logo.png        ← your logo (used in header + footer)
        ├── favicon.ico
        ├── favicon-16.png
        ├── favicon-32.png
        ├── favicon.png
        ├── apple-touch-icon.png
        ├── hero-bg.jpg           ← ADD THIS (optional)
        └── cta-bg.jpg            ← ADD THIS (optional)
```

---

## Push to GitHub

⚠️ **Important:** upload the **contents** of this folder to your repo, not the folder itself. The `index.html` must be at the **root** of your repo for GitHub Pages to find it.

1. Open this folder
2. Select all files inside (`index.html`, `README.md`, `.gitignore`, `assets/`)
3. On GitHub: **Add file → Upload files** → drag the selection in
4. Commit
5. **Settings → Pages → Source: main branch / root → Save**
6. Visit `https://YOUR-USERNAME.github.io/YOUR-REPO/`

For clean URLs (no `.html` in the address bar), deploy on **Netlify** (drag the folder onto netlify.com/drop) or **Vercel**. Both are free and faster than GitHub Pages.

---

## Animations included

- Logo bars rotate slightly on hover
- Hero headline rises in line by line
- Eyebrow / lede / buttons fade up in sequence
- Hero background performs slow Ken-Burns zoom (when image present)
- Floating world-icon SVGs
- Spinning globe icons
- Four signature bars stretch in across the bottom of the hero
- Cards lift on hover with soft shadows
- Reveal-on-scroll for all sections
- Ambient color drifts on the dark CTA banner
- Header fades in when scrolling
- Honors `prefers-reduced-motion`

---

© Atlas Cultural Initiative 2026
