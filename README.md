# Atlas Cultural Initiative — Website

Independent cultural platform launching in Lebanon. Discover the world's cultures without traveling.

## Pages

- `index.html` — Home (with About folded in)
- `programs.html` — Five program formats
- `events.html` — Upcoming + past events
- `partners.html` — Sponsor (Colart) + partners (Hand in Hand, others)
- `contact.html` — Contact form / become a partner

## Brand

- **Wordmark:** ATLAS / CULTURAL INITIATIVE
- **Signature colors:** Red `#D63A2F` · Orange `#E89B2A` · Blue `#2E8FCF` · Green `#8FBE3F`
- **Type:** Inter (UI) + Cormorant Garamond (display/serif)
- **Voice:** Warm, confident, slightly literary — never touristy

## Stack

Pure HTML / CSS / JavaScript. No build step, no dependencies. Just push and host.

Animations include hero text rise, signature-bar stretch, scroll-reveal on sections, floating SVG world icons, hover lifts on cards, animated stat counter, and ambient color drifts on the CTA banner. Honors `prefers-reduced-motion`.

## Deploy

### Option A — GitHub Pages (free)

1. Create a new repo on GitHub (e.g. `atlas-cultural-initiative`)
2. Push these files to the `main` branch:
   ```bash
   git init
   git add .
   git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/atlas-cultural-initiative.git
   git push -u origin main
   ```
3. Go to **Settings → Pages**, set source to **Deploy from branch**, branch `main`, folder `/ (root)`. Save.
4. Site will be live at `https://YOUR-USERNAME.github.io/atlas-cultural-initiative/`

### Option B — Netlify or Vercel (recommended for clean URLs)

1. Push to GitHub as above
2. Connect the repo on [netlify.com](https://netlify.com) or [vercel.com](https://vercel.com)
3. Build command: *(none)* — Publish directory: `.`
4. Custom domain → point `atlasculturalinitiative.com` to it

> Netlify and Vercel both handle clean URLs automatically (`/programs` instead of `/programs.html`). On GitHub Pages, links use `.html` extensions which still work cleanly.

## Local preview

```bash
# Python
python3 -m http.server 8000

# Or Node
npx serve .
```

Then open `http://localhost:8000`.

## Structure

```
.
├── index.html
├── programs.html
├── events.html
├── partners.html
├── contact.html
├── README.md
└── assets/
    ├── css/style.css
    ├── js/main.js
    └── img/favicon.svg
```

## To customize

- **Events:** edit the `.event-card` blocks in `index.html` and `events.html`
- **Colors:** all four pillar colors are CSS variables in `assets/css/style.css` under `:root`
- **Contact form:** currently shows a confirmation message. To wire up real email delivery, integrate [Formspree](https://formspree.io), [Netlify Forms](https://docs.netlify.com/forms/setup/), or [Web3Forms](https://web3forms.com) — change the `<form>` action attribute to your endpoint
- **Social links:** placeholder hrefs in the footer of every page

---

© Atlas Cultural Initiative 2026
