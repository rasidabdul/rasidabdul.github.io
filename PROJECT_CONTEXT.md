# Project Context: rasidabdul.github.io

## Overview
- **Type**: Personal Portfolio / Professional Biography Website
- **Owner**: Abdul Rasid (Associate Partner, Solutions Architecture & Delivery, IBM Consulting Financial Services)
- **Deployment Platform**: GitHub Pages (`https://rasidabdul.github.io/`)
- **Hosting Method**: Deployed from branch `main`, root `/` directory.

## Architecture & Tech Stack
- **Languages**: HTML5, CSS3, Minimal Vanilla JavaScript (for dynamic footer year rendering)
- **Dependencies / Frameworks**: Zero external dependencies or build tools; pure static site
- **Styling**: [`css/styles.css`](css/styles.css) using CSS variables, flexbox, grid, and Google Fonts (`DM Sans`, `Playfair Display`)
- **Configuration**: [`_config.yml`](_config.yml) (basic Jekyll metadata config for GitHub Pages)

## Project Structure
- [`index.html`](index.html): Main landing page presenting professional summary, expertise badges, and career timeline.
- [`about.html`](about.html): Overview of site architecture and design goals.
- [`contact.html`](contact.html): Contact points and links (GitHub repo, LinkedIn, live site).
- [`css/styles.css`](css/styles.css): Shared responsive stylesheet.
- [`_config.yml`](_config.yml): Jekyll configuration for GitHub Pages exclusions and metadata.
- [`README.md`](README.md): Repository documentation and local preview instructions.

## Development & Local Preview
To preview locally:
```sh
python3 -m http.server 8000
```
Then visit `http://localhost:8000`.

## Guidelines for Modifications
- Maintain zero-build-step simplicity (pure HTML/CSS/minimal JS).
- Ensure mobile responsiveness and cross-browser compatibility.
- Adhere to the established CSS variable palette and typography rules defined in [`css/styles.css`](css/styles.css).
