# Top Navigation & Header Plan

## Overview
Add a consistent, responsive top navigation header and aligned footer to [`index.html`](index.html), and update navigation menus across all site pages ([`index.html`](index.html), [`about.html`](about.html), and [`contact.html`](contact.html)).

The navigation menus will feature:
1. **Brand**: `Abdul Rasid` linking to `index.html`
2. **Know More**: Linking to `about.html`
3. **ContactMe**: Linking to `contact.html`
4. **My Github Repositories**: Linking to `https://github.com/rasidabdul` opening with `target="_blank"` and `rel="noopener noreferrer"`

---

## Sub-Tasks

### Sub-Task 1: Add Site Header and Footer CSS Styles
- **Intent**: Provide responsive styling for `.site-header`, `.header-inner`, `.brand`, `.nav`, `.nav a`, and `.site-footer` in `css/styles.css` so that the navigation and footer render cleanly across desktop and mobile devices without breaking existing `.page-shell` or hero layouts.
- **Expected Outcomes**:
  - CSS includes styles for sticky or top-level `.site-header` matching the existing palette (`--ink`, `--paper`, `--accent`, `--line`).
  - Active link state `.nav a.active` and hover effects are properly styled.
  - Mobile responsiveness adjusts navigation spacing cleanly on screens &le; 680px.
- **Todo List**:
  1. Add `.site-header`, `.header-inner`, `.brand`, and `.nav` styles into [`css/styles.css`](css/styles.css).
  2. Add `.site-footer` styles and responsive adjustments for mobile in [`css/styles.css`](css/styles.css).
- **Relevant Context**: [`css/styles.css`](css/styles.css)
- **Status**: `[x] done`

---

### Sub-Task 2: Update `index.html` with Navigation Header & Footer
- **Intent**: Add the `<header class="site-header">` with the new navigation menu items (`Know More`, `ContactMe`, `My Github Repositories`) and the standard `<footer class="site-footer">` to the home page.
- **Expected Outcomes**:
  - `index.html` contains the top `<header>` element above `<main>`.
  - Header contains brand link and nav links:
    - "Know More" -> `about.html`
    - "ContactMe" -> `contact.html`
    - "My Github Repositories" -> `https://github.com/rasidabdul` (`target="_blank"`)
  - A consistent `<footer class="site-footer">` with dynamic copyright year is rendered at the bottom.
- **Todo List**:
  1. Insert `<header class="site-header">` structure before `<main>` in [`index.html`](index.html).
  2. Insert `<footer class="site-footer">` and year script before `</body>` in [`index.html`](index.html).
- **Relevant Context**: [`index.html`](index.html)
- **Status**: `[x] done`

---

### Sub-Task 3: Synchronize Navigation Header across `about.html` and `contact.html`
- **Intent**: Ensure navigation menu labels, links, and structure are uniform across all pages (`about.html`, `contact.html`).
- **Expected Outcomes**:
  - `about.html` header reflects:
    - Brand / Home -> `index.html`
    - "Know More" -> `about.html` (with `.active` class)
    - "ContactMe" -> `contact.html`
    - "My Github Repositories" -> `https://github.com/rasidabdul` (`target="_blank"`)
  - `contact.html` header reflects:
    - Brand / Home -> `index.html`
    - "Know More" -> `about.html`
    - "ContactMe" -> `contact.html` (with `.active` class)
    - "My Github Repositories" -> `https://github.com/rasidabdul` (`target="_blank"`)
- **Todo List**:
  1. Update `<nav class="nav">` in [`about.html`](about.html).
  2. Update `<nav class="nav">` in [`contact.html`](contact.html).
- **Relevant Context**: [`about.html`](about.html), [`contact.html`](contact.html)
- **Status**: `[x] done`

---

### Sub-Task 4: Validation & Preview Check
- **Intent**: Verify HTML markup validity, active link states, external link attributes (`rel="noopener noreferrer"`), and layout appearance across pages.
- **Expected Outcomes**:
  - All navigation links work correctly.
  - Layout is clean and responsive on mobile and desktop viewports.
- **Todo List**:
  1. Inspect modified HTML files and CSS rules.
  2. Verify links and styling consistency.
- **Relevant Context**: [`index.html`](index.html), [`about.html`](about.html), [`contact.html`](contact.html), [`css/styles.css`](css/styles.css)
- **Status**: `[x] done`
