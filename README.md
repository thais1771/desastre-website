# Desastre website

Marketing site for **Desastre** — the AI config manager for Mac.
[App Store](https://apps.apple.com/app/desastre-ai-config-manager/id6778777399)

Static HTML/CSS, no build step. Hosted free on GitHub Pages at
**https://thais1771.github.io/desastre-website/**

## Structure

- `index.html` — landing page (hero, screenshots, how-it-works, guides, FAQ, CTA)
- `guides/` — 10 SEO guide pages, one per target keyword
- `assets/` — App Store icon + screenshots
- `style.css` — shared styles
- `sitemap.xml`, `robots.txt` — SEO
- `.nojekyll` — serve files as-is, skip Jekyll processing

## Local preview

```sh
python3 -m http.server 8931
# then open http://localhost:8931
```

## Deploy

Push to `main`. GitHub Pages (Settings → Pages → Source: `main` / root) publishes automatically.

To move to a custom domain later: add a `CNAME` file with the domain, point DNS at
GitHub's Pages IPs, and update the absolute URLs in `index.html`, `guides/*.html`,
`sitemap.xml` and `robots.txt` from the github.io base to the new domain.
