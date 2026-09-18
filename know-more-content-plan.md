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

**Status:** `[ ] pending`

---

### Sub-Task 2 — Add Leadership Highlights section

**Intent:** Add the 8 leadership bullet points from the LinkedIn About section as styled highlight tags, consistent with the expertise tags on `index.html`.

**Expected Outcomes:**
- A new `<section>` with a section label "Leadership" and heading "Leadership Highlights" appears after the intro
- The 8 items are rendered as a `<ul class="tag-list">` (same pattern as the expertise tags on the homepage)

**Todo List:**
1. Add a `<section>` block with `class="expertise"` (reuses homepage tag-list styling)
2. Add `<p class="section-label">Leadership</p>` and `<h2>Leadership Highlights</h2>`
3. Render these 8 items as `<li>` inside `<ul class="tag-list">`:
   - Executive client engagement and strategic advisory
   - Enterprise architecture and digital transformation leadership
   - Delivery and execution of complex, mission-critical programs
   - Technology strategy, innovation, and modernization
   - Leadership of global multidisciplinary teams of 100+ professionals
   - Business development, revenue growth, and opportunity creation
   - Risk management, governance, and operational excellence
   - Cross-functional stakeholder alignment and executive communication

**Relevant Context:**
- File: `index.html` lines 50–71 — the `.expertise` / `.tag-list` pattern to mirror
- File: `about.html` — insert after the intro prose section
- Reuse existing classes: `expertise`, `section-label`, `tag-list`

**Status:** `[ ] pending`

---

### Sub-Task 3 — Add closing pull-quote / callout

**Intent:** Display the closing recognition statement as a styled pull-quote callout block, distinguishing it visually from regular prose.

**Expected Outcomes:**
- A `<blockquote>` element appears after the Leadership Highlights section
- Text: *"Recognized for bridging business strategy and technology execution, building high-performing teams, strengthening client partnerships, and delivering transformative solutions that accelerate growth and competitive advantage."*

**Todo List:**
1. Add a `<blockquote class="prose container">` (or a `<p>` with a pull-quote treatment inside the existing prose section) after the tag-list section
2. Use the existing `prose` and `container` classes — no new CSS needed

**Relevant Context:**
- File: `about.html` — insert after Sub-Task 2 section
- No new CSS classes required; `blockquote` is a standard HTML element already styled by the browser and any existing reset rules in `css/styles.css`

**Status:** `[ ] pending`

---

### Sub-Task 4 — Add Certifications section

**Intent:** List all five certifications from the LinkedIn profile.

**Expected Outcomes:**
- A new `<section>` labelled "Certifications" appears with all five certifications listed

**Todo List:**
1. Add a `<section class="container prose">` with `<p class="section-label">Certifications</p>` and `<h2>Licences & Certifications</h2>`
2. Render the following as a `<ul>`:
   - Claude Certified Architect — Foundations
   - AWS Certified Cloud Practitioner
   - The Python Bible™ | Everything You Need to Program in Python
   - watsonx.ai Generative AI Tools Technical Sales Intermediate
   - Introduction to Model Context Protocol

**Relevant Context:**
- Source: LinkedIn PDF lines 13–22
- File: `about.html` — insert after Sub-Task 3 block
- Reuse existing classes: `container`, `prose`, `section-label`

**Status:** `[ ] pending`

---

### Sub-Task 5 — Add Education section

**Intent:** Add the education entry from the LinkedIn profile.

**Expected Outcomes:**
- A new `<section>` labelled "Education" appears with the degree entry

**Todo List:**
1. Add a `<section class="container prose">` with `<p class="section-label">Education</p>` and `<h2>Academic Background</h2>`
2. Add the single entry: *Bachelor of Engineering, Information Technology — Jadavpur University, Kolkata (2001–2005)*

**Relevant Context:**
- Source: LinkedIn PDF lines 75–78
- File: `about.html` — insert after Sub-Task 4 block
- Reuse existing classes: `container`, `prose`, `section-label`

**Status:** `[ ] pending`

---

### Sub-Task 6 — Update page `<title>` and `<meta>` description

**Intent:** Align the browser tab title and meta description with the new professional content.

**Expected Outcomes:**
- `<title>` changes from `"About | rasidabdul.github.io"` to `"About Abdul Rasid | IBM Consulting Associate Partner"`
- `<meta name="description">` is added or updated to reflect the professional summary

**Todo List:**
1. Update `<title>` in `about.html` `<head>`
2. Add `<meta name="description" content="Professional profile of Abdul Rasid, Associate Partner — Solutions Architecture & Delivery, IBM Consulting Financial Services.">`

**Relevant Context:**
- File: `about.html` lines 1–8 (`<head>` block)

**Status:** `[ ] pending`
