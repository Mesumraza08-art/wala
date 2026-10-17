# Furniture Wala — website

Static site (plain HTML + JSON data + media). No build step.

## Deploy to Hostinger

**Option A — Git deploy (recommended)**
1. hPanel → Websites → Manage → **Advanced → Git**.
2. Repository: `https://github.com/Mesumraza08-art/wala.git`, branch `main`, install path empty (deploys to `public_html`).
3. Click **Create**, then **Deploy**. Enable *Auto Deployment* to redeploy on every push.

**Option B — File Manager / FTP**
Upload `index.html`, `.htaccess`, `data/` and `media/` into `public_html/`.

After deploying, enable SSL in hPanel → Security → SSL (the `.htaccess` redirects HTTP → HTTPS).

## Local preview
```
python3 -m http.server 8000
```
Then open http://localhost:8000 (opening `index.html` directly won't load the JSON data).
