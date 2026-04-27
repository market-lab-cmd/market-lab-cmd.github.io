# Root SEO Topic Pages Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Expand the root GitHub Pages repository from a single directory page into a crawlable senior-player review hub with topic pages, a local cover image, a 404 page, and split sitemaps.

**Architecture:** Keep the site static and dependency-free at runtime. Reuse `assets/css/index.css` across the root homepage and new topic pages, keep all public HTML in the repo root, and keep Markdown source notes under `content/`.

**Tech Stack:** Static HTML, CSS, small JavaScript for GA, XML sitemaps, GitHub Pages.

---

### Task 1: Add Root Topic Pages

**Files:**
- Create: `ludo-strategy-notes.html`
- Create: `teen-patti-review-notes.html`
- Create: `callbreak-strategy-review.html`
- Create: `indian-card-game-patterns.html`
- Create: `skill-game-decision-making.html`
- Modify: `assets/css/index.css`

- [ ] Create five static topic pages with unique title, description, canonical, JSON-LD, and senior-player review copy.
- [ ] Add shared article page CSS for readable long-form layout, breadcrumbs, article cards, and next-step links.

### Task 2: Add Content Source Notes

**Files:**
- Create: `content/002-ludo-strategy-notes.md`
- Create: `content/003-teen-patti-review-notes.md`
- Create: `content/004-callbreak-strategy-review.md`
- Create: `content/005-indian-card-game-patterns.md`
- Create: `content/006-skill-game-decision-making.md`
- Modify: `README.md`

- [ ] Add Markdown source notes that mirror the new root topic pages.
- [ ] Update README content list with ordered links.

### Task 3: Add Root Cover Image and Metadata

**Files:**
- Create: `assets/images/game-strategy-notes-hub.png`
- Modify: `index.html`

- [ ] Generate a local root cover image for the hub.
- [ ] Point root Open Graph and Twitter images to the local image.
- [ ] Add the topic pages to homepage navigation and homepage internal links.

### Task 4: Add 404 Page

**Files:**
- Create: `404.html`

- [ ] Create a helpful GitHub Pages 404 page that links back to root notes and topic pages.

### Task 5: Split and Verify Sitemaps

**Files:**
- Modify: `sitemap.xml`
- Create: `sitemaps/root-pages.xml`
- Create: `sitemaps/collections.xml`
- Modify: `robots.txt`

- [ ] Convert `sitemap.xml` into a sitemap index.
- [ ] Put root pages in `sitemaps/root-pages.xml`.
- [ ] Put existing collection URLs in `sitemaps/collections.xml`.
- [ ] Keep `robots.txt` pointing at `https://market-lab-cmd.github.io/sitemap.xml`.

### Verification

- [ ] Parse every XML sitemap.
- [ ] Parse JSON-LD from all root HTML pages.
- [ ] Confirm one H1 per public HTML page.
- [ ] Confirm all local CSS, JS, and image references exist.
- [ ] Confirm all sitemap URLs map to local files in the workspace.
