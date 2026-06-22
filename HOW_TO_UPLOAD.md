# Upload guide — x402cli GitHub repository

Upload **everything inside** `github/` to your repo root. **No website HTML/CSS/JS.**

---

## File tree (full)

```
github/
├── logo.png                          ← Repo logo + README header
├── assets/logo.png                   ← Same logo (assets folder)
├── README.md                         ← Main repo page
├── LICENSE
├── CHANGELOG.md
├── STATUS.md
├── SOCIAL.md                         ← X / @x402cli follow page
├── CONTRIBUTING.md
├── SECURITY.md
├── HOW_TO_UPLOAD.md
├── .gitignore
├── docs/
│   ├── INTRODUCTION.md
│   ├── COMMANDS.md
│   ├── API.md
│   ├── ARCHITECTURE.md
│   ├── ROADMAP.md
│   ├── FAQ.md
│   └── DISCLAIMER.md
└── .github/
    ├── PULL_REQUEST_TEMPLATE.md
    └── ISSUE_TEMPLATE/
        ├── bug_report.md
        ├── feature_request.md
        └── registry_interest.md
```

**Total: ~20 files — all markdown, logo, templates. Zero website source.**

---

## Step 1 — Create repo

1. [github.com/new](https://github.com/new)
2. Name: `x402cli`
3. Public
4. **Do NOT** add README / license / gitignore
5. Create repository

---

## Step 2 — Upload

### Drag & drop (easiest)

1. Open empty repo → **Add file → Upload files**
2. Drag **entire contents** of `d:\x402cli\github\`
3. Commit: `Initial commit — x402 CLI project hub`

### Git CLI

```powershell
cd d:\x402cli\github
git init
git add .
git commit -m "Initial commit — x402 CLI project hub"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/x402cli.git
git push -u origin main
```

---

## Step 3 — Repo settings

**About (gear icon):**
- Website: `https://x402cli.xyz`
- Topics: `x402`, `base`, `usdc`, `developer-tools`, `cli`, `http-402`

**X updates:** README and SOCIAL.md link to **https://x.com/x402cli** — users follow here for progress.

**Social preview:** Settings → General → upload `logo.png`

**Edit README.md:** replace `YOUR_USERNAME` if any placeholder remains.

---

## What stays OFF GitHub

| Keep private (cPanel only) | In this repo |
|----------------------------|--------------|
| index.html, docs.html, etc. | docs/*.md (text only) |
| style.css, main.js | — |
| api/*.php | docs/API.md (reference) |
| .htaccess | docs/ARCHITECTURE.md |

---

## FAQ

**Why so many files if no website code?**  
Professional repos have docs, changelog, contributing guide, issue templates, and status — without exposing deployable source.

**Can people still copy my site?**  
Anyone can visit x402cli.xyz and view source in browser. Keeping HTML off GitHub prevents one-click repo clone of your full deploy bundle.
