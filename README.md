# desastre.app

Marketing site for **Desastre** — the AI config manager for Mac.
[App Store](https://apps.apple.com/app/desastre-ai-config-manager/id6778777399)

Static HTML/CSS, no build step. Served by GitHub Pages from the repo root at
the custom domain **desastre.app** (see `CNAME`).

## Structure

- `index.html` — landing page (hero, screenshots, how-it-works, guides, FAQ, CTA)
- `guides/` — 10 SEO guide pages, one per target keyword
- `assets/` — App Store icon + screenshots
- `style.css` — shared styles
- `sitemap.xml`, `robots.txt` — SEO
- `CNAME` — custom domain for GitHub Pages
- `.nojekyll` — serve files as-is, skip Jekyll processing

## Local preview

```sh
python3 -m http.server 8931
# then open http://localhost:8931
```

## Deploy

Push to `main`. GitHub Pages (Settings → Pages → Source: `main` / root) publishes automatically.
