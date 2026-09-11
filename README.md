# actiocognita-site

Static one-page site for ActioCognita LLC.

- `public/index.html` — the entire site (markup + styles, no build step, no dependencies).
- `wrangler.jsonc` — Cloudflare Workers config; serves `public/` as static assets.

## Deploy

Deployed on Cloudflare Workers (Static Assets), connected to this repository —
every push to `main` deploys.

Dashboard settings for the Git connection: no build command, and the assets
directory comes from `wrangler.jsonc`.

To deploy by hand instead:

```bash
npx wrangler deploy
```

## Local preview

```bash
python3 -m http.server 8080 --bind 0.0.0.0 --directory public
```

Reachable from other devices on the tailnet at http://mac-studio:8080
