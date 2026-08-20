# Emerge Brighter Website

A simple static landing page for **EmergeBrighter.com**, configured for free hosting with **GitHub + Cloudflare Workers Static Assets**.

## Files

- `index.html` — complete responsive landing page
- `assets/workbook.webp` — workbook image
- `favicon.svg` — browser icon
- `404.html` — custom not-found page
- `robots.txt` — search-engine instructions
- `sitemap.xml` — one-page sitemap
- `_headers` — Cloudflare security/cache headers
- `wrangler.jsonc` — Cloudflare Workers configuration
- `.assetsignore` — keeps deployment-only files out of the public site

## GitHub

Upload all files and the `assets` folder to the repository root and commit the changes.

## Cloudflare Workers settings

Connect the GitHub repository from **Workers & Pages → Create application → Continue with GitHub**.

- Project name: `emergebrighter`
- Production branch: `main`
- Build command: leave blank
- Deploy command: use Cloudflare's default `npx wrangler deploy`
- Static assets directory: configured automatically in `wrangler.jsonc`

Cloudflare will first deploy the site to a free `workers.dev` preview address. After the site is verified, add `emergebrighter.com` to Cloudflare and connect it as the custom domain.

## Workbook purchase link

The purchase buttons point to:

`https://www.amazon.com/dp/1733083723`
