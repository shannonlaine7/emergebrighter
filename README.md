# Emerge Brighter Website

Simple static landing page for EmergeBrighter.com, hosted free with GitHub + Cloudflare Workers Static Assets.

## Structure

- `public/` — the only directory Cloudflare publishes
  - `index.html`
  - `404.html`
  - `favicon.svg`
  - `robots.txt`
  - `sitemap.xml`
  - `_headers`
  - `assets/workbook.webp`
- `wrangler.jsonc` — Cloudflare Worker configuration
- `README.md` — repository documentation

## Cloudflare deployment

The repository is connected to Cloudflare Workers.

- Build command: leave blank
- Deploy command: `npx wrangler deploy`
- Production branch: `main`

The `wrangler.jsonc` configuration intentionally points Cloudflare only to `./public`, which prevents Git metadata and deployment files from being published as website assets.

## Workbook purchase

The site links to the Emerge Brighter workbook on Amazon.
