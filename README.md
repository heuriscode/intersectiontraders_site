# Intersection Traders — website

Single-file static site for intersectiontraders.com.au, served via GitHub Pages.

## Update workflow
1. Edit `index.html` locally.
2. Test locally: just open `index.html` in a browser (double-click), or run `python3 -m http.server` in this folder and visit http://localhost:8000
3. Commit and push to `main`. GitHub Pages redeploys automatically in ~1 minute.

## One-time setup (already described in chat)
- Repo Settings → Pages → Source: Deploy from a branch → `main` / `/ (root)`
- Custom domain: `www.intersectiontraders.com.au` → tick "Enforce HTTPS" once the certificate is issued
- DNS at cheaperdomains.com.au: `www` CNAME → `<your-github-username>.github.io`; apex A records → 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153

`.nojekyll` disables Jekyll processing (keeps deploys fast and literal). `CNAME` holds the custom domain for Pages.
