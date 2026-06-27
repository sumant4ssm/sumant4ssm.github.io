# SEO Follow-up Actions

This file lists the **on-page work that is already done** in the code, plus the
**off-page / account actions that only the site owner can do**. On-page SEO gets
the site indexed and understood, but ranking for competitive terms ("app lock",
"pdf scanner", "internet speed test") also depends on the items in Part B.

## Part A — On-page SEO (DONE in this repo)

- [x] **Multi-page hub & spoke structure** — homepage + one focused page per app
- [x] **Keyword-targeted titles & meta descriptions** (≤60 / ≤155 chars) on every page
- [x] **Canonical URLs** (`<link rel="canonical">`) on every page
- [x] **Semantic HTML5** — `header`, `main`, `section`, `article`, `nav`, `aside`, one `<h1>` per page
- [x] **Breadcrumb navigation** + `BreadcrumbList` structured data on app pages
- [x] **Structured data (JSON-LD)**
  - Homepage: `Organization` + `WebSite` (with `SearchAction`)
  - Each app: `SoftwareApplication` + `FAQPage` + `BreadcrumbList`
- [x] **FAQ sections** targeting "People also ask" queries for each app
- [x] **Open Graph + Twitter Card** tags on every page
- [x] **`robots.txt`** (allow all) + **`sitemap.xml`** (all 5 pages)
- [x] **Internal linking** — every page links to every other page
- [x] **Keyword-rich body copy** (no stuffing), mobile-responsive, fast (no JS frameworks)
- [x] `<html lang="en">`, descriptive link text, `rel="noopener"` on external links

## Part B — Off-page / account actions (TODO, owner only)

These have a **much bigger ranking impact** than any code change. Do them in order.

### 1. Google Search Console (highest priority)
1. Go to https://search.google.com/search-console
2. Add a property for `https://sumant4ssm.github.io` (URL prefix) **or** the
   custom domain from Part C.
3. Verify ownership (GitHub Pages sites can be verified via the HTML tag method —
   paste the meta tag into each page's `<head>`, or use the Google Analytics method).
4. Submit the sitemap: `https://sumant4ssm.github.io/sitemap.xml`
5. Use **URL Inspection → Request Indexing** for each of the 5 pages.

### 2. Get a custom domain (biggest single SEO boost)
A `*.github.io` subdomain has low authority. Buying `appcraft.digital` (or similar)
and pointing it at GitHub Pages:
- Adds a permanent, brandable identity.
- Lets you build **domain authority** over time that transfers across pages.
- In Settings → Pages → Custom domain, add the domain and check **Enforce HTTPS**.
- Then update every `canonical`, `og:url`, and the `sitemap.xml`/`robots.txt` URLs
  in this repo from `sumant4ssm.github.io` to the new domain, and resubmit.

### 3. Backlinks (the main ranking currency)
- Link to the site **from each app's Play Store listing** (Developer website field +
  app description footer).
- Add the site URL to your **GitHub profile**, README files, and bio links.
- Write on Reddit (r/androidapps, r/privacy), X, Product Hunt, and app-review blogs.
- Reach out to "best app locker 2026" / "Cam Scanner alternative" listicle authors.

### 4. Keep content fresh
- Update `<lastmod>` in `sitemap.xml` whenever you change a page.
- Add real screenshots and an icon image once available (OG image + `og:image` tag).
- Replace the placeholder `aggregateRating` values on AppLock Ultra with **real**
  Play Store ratings once you have them — fake/stale ratings can be flagged.

### 5. Monitor
- Check Search Console weekly for indexing errors, queries, and CTR.
- Use the **Rich Results Test** (https://search.google.com/test/rich-results) on
  each page to confirm the FAQ and SoftwareApplication data is valid.

---

## Honest expectation

Ranking #1 for "app lock", "internet speed test", or "pdf scanner" is **not**
possible through code alone — those terms are owned by Google Play, Ookla, Adobe,
etc. with massive authority. Realistic wins:

- **Branded searches** (AppLock Ultra, Internet Velocity, AppCraft Digital)
- **Long-tail queries** ("offline pdf scanner without ads", "app locker intruder selfie",
  "encrypt photos on-device", "wifi speed meter per app data")
- **"People also ask"** FAQ snippets, once indexed

Combine the on-page work here with Part B (Search Console + custom domain +
backlinks) for the best results over the coming months.
