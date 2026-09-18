# Know More Page — Content Rewrite Plan

## Overview

The "Know More" nav link points to `about.html`, which currently describes the site repository (build approach, file structure, design goals). This plan replaces that content entirely with Abdul Rasid's professional biography drawn from his LinkedIn profile PDF.

**Goal:** Transform `about.html` into a professional profile page that reflects the full LinkedIn About section, leadership highlights, experience, education, and certifications.  
**Scope:** `about.html` only. No changes to `index.html`, `contact.html`, `css/styles.css`, or any other file.  
**Non-goals:** No layout/design changes, no new CSS classes (reuse existing ones), no new pages.

---

## Sub-Tasks

---

### Sub-Task 1 — Replace page header and intro

**Intent:** Remove the "About this site" heading and repository description. Replace with the professional headline and executive summary from the LinkedIn About section.

**Expected Outcomes:**
- `<h1>` reads: `About Abdul Rasid`
- Subheading (lede) reads the LinkedIn headline: *Associate Partner @ IBM Consulting — Financial Services | Solutions Architecture & Delivery | Banking Transformation | Agentic AI Systems*
- Opening prose paragraph contains the executive summary: *"Executive technology leader with 21+ years of experience…"*

**Todo List:**
1. Change `<h1>` from `"About this site"` to `"About Abdul Rasid"`
2. Change the `<p class="lede">` to the LinkedIn headline text
3. Replace the repository description paragraph with the executive summary paragraph from the LinkedIn About section

**Relevant Context:**
- File: `about.html` lines 22–31 (current `<section class="page-header container">` and first `<section class="container prose">` paragraph)
- Reuse existing classes: `page-header`, `container`, `prose`, `lede`

**Status:** `[x] done`

---

### Sub-Task 2 — Add Leadership Highlights section

**Intent:** Add the 8 leadership bullet points from the LinkedIn About section as styled highlight tags, consistent with the expertise tags on `index.html`.

**Expected Outcomes:**
- A new `<section>` with a section label "Leadership" and heading "Leadership Highlights" appears after the intro
- The 8 items are rendered as a `<ul class="tag-list">` (same pattern as the expertise tags on the homepage)

**Todo List:**
1. Add a `<section class="container prose">` block (reuses prose layout for alignment)
2. Add `<p class="section-label">Leadership</p>` and `<h2>Leadership Highlights</h2>`
3. Render 8 items as `<li>` inside `<ul class="tag-list">`

**Relevant Context:**
- File: `about.html` — insert after the intro prose section
- Reuse existing classes: `container`, `prose`, `section-label`, `tag-list`

**Status:** `[x] done`

---

### Sub-Task 3 — Add closing pull-quote / callout

**Intent:** Display the closing recognition statement as a styled pull-quote callout block.

**Expected Outcomes:**
- A `<blockquote>` element appears after the Leadership Highlights section

**Status:** `[x] done`

---

### Sub-Task 4 — Add Certifications section

**Intent:** List all five certifications from the LinkedIn profile.

**Status:** `[x] done`

---

### Sub-Task 5 — Add Education section

**Intent:** Add the education entry from the LinkedIn profile.

**Status:** `[x] done`

---

### Sub-Task 6 — Update page title and meta description

**Intent:** Align the browser tab title and meta description with the new professional content.

**Status:** `[x] done`
