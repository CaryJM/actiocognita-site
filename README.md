# actiocognita-site

Static one-page site for ActioCognita LLC.

- `index.html` — the entire site (markup + styles, no build step, no dependencies).

## Deploy

Cloudflare Pages: connect this repository, leave the build command empty, and set
the build output directory to `/` (repository root).

## Local preview

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000
