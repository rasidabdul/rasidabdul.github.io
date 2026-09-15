# Project Context: rasidabdul.github.io

## Overview
- **Type**: Personal Portfolio / Professional Biography Website
- **Owner**: Abdul Rasid (Associate Partner, Solutions Architecture & Delivery, IBM Consulting Financial Services)
- **Deployment Platform**: GitHub Pages (`https://rasidabdul.github.io/`)
- **Hosting Method**: Deployed from branch `main`, root `/` directory.

## Architecture & Tech Stack
- **Languages**: HTML5, CSS3, Minimal Vanilla JavaScript (for dynamic footer year rendering)
- **Dependencies / Frameworks**: Zero external dependencies or build tools; pure static site
- **Styling**: `css/styles.css` using CSS variables, CSS grid/flexbox, and Google Fonts (`DM Sans`, `Playfair Display`)
- **Configuration**: `_config.yml` (Jekyll metadata & exclusions for GitHub Pages)

## Project Structure
- `index.html`: Main landing page with hero summary, expertise tags, overview cards, and career timeline.
- `about.html`: Explains repository purpose, design philosophy, and architecture.
- `contact.html`: Contact channels and external repository links.
- `css/styles.css`: Shared responsive stylesheet.
- `_config.yml`: GitHub Pages configuration and file exclusion rules.
- `README.md`: Project overview and local development instructions.

## Development & Local Preview
To preview locally:
```sh
python3 -m http.server 8000
```
Then open `http://localhost:8000`.

## Guidelines & Conventions
- **No Build Steps**: Keep all HTML, CSS, and JS plain and native without bundlers or frameworks.
- **Responsiveness**: Ensure layout adaptations work across mobile and desktop breakpoints.
- **Theme Consistency**: Reuse the CSS variables in `css/styles.css` (`--ink`, `--paper`, `--accent`, `--accent-soft`, `--muted`, `--line`).
