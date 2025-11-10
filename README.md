# Irfan Ullah — GitHub Pages site

Static site contents:
- `index.html` (Tailwind via CDN)
- `prof.png`
- `404.html`
- `.nojekyll`

## Quick publish (user/organization site)
1) Create a new public repo named exactly: `<your-github-username>.github.io`
2) Put these files in the repo root (index.html at the root path).
3) Commit and push to the `main` branch.
4) Visit: `https://<your-github-username>.github.io/`

## Project site (subpath) alternative
1) Create a new public repo with any name (e.g., `portfolio`).
2) Put these files at the repo root and push to `main`.
3) In repo Settings → Pages:
   - Source: `Deploy from a branch`
   - Branch: `main` / root (`/`)
4) Your site will be at: `https://<your-github-username>.github.io/<repo-name>/`

Notes:
- `.nojekyll` disables Jekyll processing so Tailwind CDN and folder names like `_*` won’t be blocked.
- `404.html` gives a friendly not‑found page.
- For a custom domain, add a `CNAME` file with your domain and configure DNS (A/ALIAS/ANAME or CNAME to `<username>.github.io`).

## Local preview
Open `index.html` directly in your browser or serve locally:

```bash
# Python
python3 -m http.server 5500
# then visit http://localhost:5500
```


