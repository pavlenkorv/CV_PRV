# Ruslan Pavlenko — CV

Interactive CV web app with position & language switching.

🌐 **Live:** https://pavlenkorv.github.io/CV_PRV

---

## Features

- **2 positions:** Project Manager | CEO / COO
- **3 languages:** 🇬🇧 English · 🇩🇪 Deutsch · 🇺🇦 Українська
- **Print to PDF** directly from browser
- Auto-deployed to GitHub Pages on every push

## Structure

```
├── index.html                  # Main CV web app
├── src/
│   ├── metadata/
│   │   └── metadata.js         # All CV content (edit this)
│   └── assets/
│       └── images/
│           └── photo.jpg       # Profile photo
├── .github/
│   └── workflows/
│       └── deploy.yml          # Auto-deploy to GitHub Pages
└── README.md
```

## Setup & Deployment

### One-time GitHub Pages setup

1. Go to your repo → **Settings → Pages**
2. Under **Source** select **GitHub Actions**
3. Push to `main` — the workflow deploys automatically

### Local preview

```bash
npx serve . -p 3000
# Open http://localhost:3000
```

### Update CV content

Edit `src/metadata/metadata.js` — all 6 CV versions are in one file.
Commit and push → GitHub Actions redeploys in ~30 seconds.

## URL parameters

Link directly to a specific version:

| URL | Opens |
|-----|-------|
| `index.html?pos=pm&lang=en` | Project Manager · English |
| `index.html?pos=coo&lang=de` | CEO/COO · Deutsch |
| `index.html?pos=pm&lang=ua` | PM · Українська |

---

*Last updated: February 2026*
