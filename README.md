# wedding-2.0

Static site, no build step — just plain HTML/CSS/JS served directly.

## Layout

- `index.html` — root landing page, password-gated, links out to the sections below.
- `thecelebration/` (the single-day event) and `theweekend/` (the two-day event) — each has its own `mobile.html` and `web.html` (intentionally different designs, not responsive variants of one file), an `images/` folder, and an `index.html` that checks `window.innerWidth` on load and redirects to `web.html` (≥1024px) or `mobile.html` (<1024px). `/thecelebration/` and `/theweekend/` stay the shareable URLs — deliberately not named as obvious siblings so the two events' links don't look related.
- `games/` — wedding games page (`index.html`) and its `images/` assets.

Each section is self-contained.
