# rasidabdul.github.io

Personal GitHub Pages site for **Abdul Rasid** — Associate Partner, Solutions Architecture & Delivery, IBM Consulting Financial Services.

- **Repository:** https://github.com/rasidabdul/rasidabdul.github.io
- **Published site:** https://rasidabdul.github.io/
- **Default branch:** `main`
- **Visibility:** Public

## Purpose

This repository hosts a polished, responsive personal biography site published with GitHub Pages. It is plain static HTML and CSS — no build step, no framework, no external dependencies.

## Status

| Stage | Status |
|---|---|
| Repository created (public, `main` default branch) | Done |
| README and baseline configuration | Done |
| Site content (biography, about, contact pages) | Done |
| GitHub Pages build/deploy configured | Done — Deploy from branch `main`, `/ (root)` |
| Published site verified | https://rasidabdul.github.io/ |

## Repository layout

```text
.
├── README.md          # This file
├── .gitignore         # Editor, OS, and static-site build artifacts
├── _config.yml        # Jekyll/Pages site metadata
├── index.html         # Biography landing page
├── about.html         # About this site
├── contact.html       # Contact / links page
└── css/
    └── styles.css     # Shared responsive stylesheet
```

## Publishing with GitHub Pages

GitHub Pages is enabled for this repository:

1. **Settings → Pages** → **Build and deployment**
2. **Source:** Deploy from a branch
3. **Branch:** `main` / `/ (root)`

The site is available at `https://rasidabdul.github.io/`.

## Local preview

This is plain static HTML/CSS — serve the repository root and open it in a browser:

```sh
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.
