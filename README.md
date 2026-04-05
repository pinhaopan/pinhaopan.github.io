# pinhaopan.github.io

Personal portfolio for Johnny Pan. Deployed as a static site on GitHub Pages.

**Live URL:** https://pinhaopan.github.io

---

## Deployment Steps

### 1. Create the repository on GitHub

1. Go to https://github.com/new
2. Set **Repository name** to exactly: `pinhaopan.github.io`
3. Set **Visibility** to **Public** (required for free GitHub Pages)
4. Leave all other options unchecked
5. Click **Create repository**

### 2. Clone and add your files

```bash
# Clone the empty repo to your local machine
git clone https://github.com/pinhaopan/pinhaopan.github.io.git
cd pinhaopan.github.io

# Copy index.html (and README.md) into this folder
# Then stage and commit:
git add index.html README.md
git commit -m "Initial portfolio deploy"
git push origin main
```

If you already have the files locally and just need to push:

```bash
cd path/to/pinhaopan.github.io

git init
git remote add origin https://github.com/pinhaopan/pinhaopan.github.io.git
git add index.html README.md
git commit -m "Initial portfolio deploy"
git branch -M main
git push -u origin main
```

### 3. Enable GitHub Pages

1. Open the repository on GitHub
2. Click **Settings** (top menu)
3. In the left sidebar, click **Pages** (under "Code and automation")
4. Under **Source**, select **Deploy from a branch**
5. Set branch to `main`, folder to `/ (root)`
6. Click **Save**

Your site will be live at **https://pinhaopan.github.io** within 1-3 minutes.

---

## Customization Checklist

Before going live, update the following inside `index.html`:

| Item | Location | What to change |
|------|----------|---------------|
| Email address | Contact section + `mailto:` href | Replace `hello@johnnypan.com` with your real address |
| LinkedIn URL | Contact section | Update `linkedin.com/in/pinhaopan` if your handle differs |
| Counter numbers | Hero `data-target` attributes | Adjust 47K+, 6, 3, 2 to reflect your real stats |
| Project descriptions | Projects section | Add specific impact numbers and correct GitHub repo links |

---

## Tech Notes

- Pure HTML, CSS, and vanilla JavaScript
- No build tools, no frameworks, no local dependencies
- Fonts loaded via Google Fonts CDN (DM Serif Display + IBM Plex Mono)
- All other CSS and JS is inline in `index.html`
- Works on any static file host, not just GitHub Pages
