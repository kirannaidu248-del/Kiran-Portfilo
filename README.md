# Kiran R — Portfolio

> Digital Marketing Specialist & SEO Analyst portfolio. A single-page, zero-dependency static site built for fast load, full accessibility, and easy customization.

🌐 **Live:** *deploy to Vercel — instructions below*
📍 **Bangalore, India** &nbsp;·&nbsp; ✉️ kirannaidu248@gmail.com &nbsp;·&nbsp; 🔗 [LinkedIn](https://www.linkedin.com/in/kiranraghupathi/)

---

## ✨ Features

- 🎨 **10 color palettes** — Aurora, Sunset, Ocean, Forest, Crimson, Mono, Gold, Lavender, Cyber, Coral
- 🌗 **Light + Dark theme** with system-preference detection, persists via `localStorage`
- 📱 **Fully responsive** — breakpoints at 900 / 600 / 380px, touch-friendly, reduced-motion aware
- 🧱 **Bento grid layout** — the dominant 2026 portfolio pattern
- ⚡ **Zero build step** — single HTML file, no bundler, no framework
- ⌨️ **Press `T`** anywhere to toggle theme
- 📊 **Animated stat counters** (count-up on scroll-into-view)
- 📏 **Reading progress bar**, active nav highlight, back-to-top
- 🍔 **Mobile hamburger menu** with full-screen serif overlay
- 📥 **Resume PDF download** + working contact form (mailto)
- 🚀 **SEO + AEO ready** — meta tags, Open Graph, sitemap, robots.txt with AI crawler allow-list

---

## 🎨 Color Palettes

| # | Name     | Vibe                                |
| - | -------- | ----------------------------------- |
| 1 | Aurora   | Violet → Blue → Cyan (AI-era cool)  |
| 2 | Sunset   | Orange → Pink → Yellow (warm)       |
| 3 | Ocean    | Cyan → Blue → Teal (calm)           |
| 4 | Forest   | Emerald → Lime → Olive (organic)    |
| 5 | Crimson  | Red → Rose → Pink (bold)            |
| 6 | Mono     | Neutral grays (editorial)           |
| 7 | Gold     | Amber → Orange → Bronze (luxe)      |
| 8 | Lavender | Violet → Indigo (premium)           |
| 9 | Cyber    | Cyan → Lime (futuristic)            |
| 10 | Coral   | Coral → Peach → Amber (friendly)    |

Open the floating ⚙ button (bottom-right) on the live site to switch between them.

---

## 🛠 Tech Stack

- **HTML5** — semantic, accessible markup
- **CSS3** — custom properties, `color-mix()` for theme-aware tinting, modern grid
- **Vanilla JS** — IntersectionObserver, no dependencies
- **Fonts** — Inter (sans), Instrument Serif (display italic), JetBrains Mono (UI)

---

## 🚀 Deploy to Vercel

This repo is **Vercel-ready** out of the box.

### Option 1 — One-click (recommended)

1. Push your fork to GitHub (already done if you're reading this on GitHub)
2. Go to [vercel.com/new](https://vercel.com/new)
3. Import this repository
4. Click **Deploy** — Vercel auto-detects it as a static site
5. Done. Your site is live at `https://kiran-portfilo.vercel.app/` (or your custom domain)

### Option 2 — Vercel CLI

```bash
npm i -g vercel
vercel
```

### What's included for Vercel

| File | Purpose |
| ---- | ------- |
| `vercel.json` | Clean URLs, security headers, cache control, custom redirects (`/resume`, `/cv`, `/linkedin`) |
| `404.html` | Custom not-found page matching the site theme |
| `robots.txt` | Crawler rules + AI bot allow-list (GPTBot, ClaudeBot, PerplexityBot, Google-Extended) |
| `sitemap.xml` | URL discovery for search engines |
| `favicon.svg` | Scalable gradient "K" mark |

### After deploying

1. **Update absolute URLs** in `sitemap.xml`, `robots.txt`, and the `<link rel="canonical">` in `index.html` if you use a custom domain instead of the default Vercel URL.
2. **Add your custom domain** via the Vercel dashboard → Project Settings → Domains.
3. **Submit your sitemap** to [Google Search Console](https://search.google.com/search-console) for indexing.

---

## 💻 Run Locally

No build step. Just open `index.html` in any modern browser.

For a local server (avoids `file://` quirks with the resume download):

```bash
# Python 3
python -m http.server 8000

# or Node
npx serve

# then open http://localhost:8000
```

---

## 🎯 Customize

All theming lives at the top of the `<style>` block in `index.html`.

### Change colors

Edit the `[data-palette="..."]` blocks (around line 35–44):

```css
[data-palette="aurora"] {
  --accent:       #a855f7;  /* primary */
  --accent-2:     #3b82f6;  /* secondary */
  --accent-3:     #22d3ee;  /* tertiary / success */
  --accent-light: #c084fc;  /* badges & soft text */
}
```

### Add your own palette

1. Add a new `[data-palette="yourname"]` block in CSS
2. Add a matching `.swatch-yourname` gradient
3. Add a `<button data-palette-btn="yourname">` to the settings panel

### Change content

All copy lives directly in the HTML — search for the section headings (Hero, About, Skills, etc.) and edit in place.

---

## 📁 Project Structure

```
.
├── index.html        # Single-page portfolio
├── 404.html          # Custom not-found page
├── favicon.svg       # Gradient "K" mark
├── vercel.json       # Vercel config (headers, redirects, clean URLs)
├── robots.txt        # Crawler + AI bot rules
├── sitemap.xml       # SEO sitemap
├── R_KIRAN_...pdf    # Downloadable resume
└── README.md
```

---

## 📬 Contact

**Kiran R** — Digital Marketing Specialist & SEO Analyst

- ✉️ kirannaidu248@gmail.com
- 📞 +91 7022392407
- 🔗 [linkedin.com/in/kiranraghupathi](https://www.linkedin.com/in/kiranraghupathi/)

---

<sub>Built with intent &amp; SEO in mind · © 2026</sub>
