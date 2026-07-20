# Push to GitHub & deploy — free

## Step 0: Add your photo first
Save your portrait as `om.jpg` in this folder (next to `index.html`). Any color photo works — the B&W + lime look is applied by CSS.

---

## Push to GitHub

### Easiest — no command line (recommended)
1. Go to https://github.com/new and create a repo, e.g. `portfolio` (Public). Don't add a README.
2. On the new repo page, click **uploading an existing file**.
3. Drag in everything from this folder: `index.html`, `om.jpg`, `README.md`, `.gitignore`, `DEPLOY.md`.
4. Click **Commit changes**. Done — your code is on GitHub.

### Or with the command line
Run these in this folder (needs Git installed and a GitHub account):
```
git init
git add .
git commit -m "Initial commit: portfolio"
git branch -M main
git remote add origin https://github.com/om-1021/portfolio.git
git push -u origin main
```
(Replace the URL with your actual repo. GitHub will prompt for login / a Personal Access Token.)

---

## Go live (pick one)

### GitHub Pages (free, uses the repo you just made)
1. In the repo: **Settings → Pages**.
2. Under "Build and deployment", Source = **Deploy from a branch**.
3. Branch = **main**, folder = **/ (root)**. Save.
4. Wait ~1 min → your site is at `https://om-1021.github.io/portfolio/`.

### Netlify (drag & drop, ~1 min)
1. Go to https://app.netlify.com/drop
2. Drag this whole folder onto the page.
3. You get a live URL instantly. Rename it under Site settings → Domain management.

### Vercel
1. https://vercel.com → "Add New Project" → import your GitHub repo → Deploy.

---

## Custom domain (optional, later)
All three let you add a custom domain free; you only pay ~$10/yr for the domain itself. Add it under the project's domain settings and follow the DNS steps.
