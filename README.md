# wedding-2.0

Static site, no build step — just plain HTML/CSS/JS served directly.

## Layout

- `index.html` — root landing page, password-gated, links out to the sections below.
- `one-day/` and `two-day/` — each has its own `mobile.html` and `web.html` (intentionally different designs, not responsive variants of one file), an `images/` folder, and an `index.html` that checks `window.innerWidth` on load and redirects to `web.html` (≥1024px) or `mobile.html` (<1024px). `/one-day/` and `/two-day/` stay the shareable URLs.
- `games/` — wedding games page (`index.html`) and its `images/` assets.

Each section is self-contained.
