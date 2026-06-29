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
  - Homepage: `Organization` + `WebSite`
  - Each app: `SoftwareApplication` + `FAQPage` + `BreadcrumbList`
- [x] **FAQ sections** targeting "People also ask" queries for each app
- [x] **Open Graph + Twitter Card** tags on every page, including 1200×630 share images
- [x] **`robots.txt`** (allow all) + **`sitemap.xml`** (all 5 pages)
- [x] **Custom-domain canonicalization** — canonical URLs, `og:url`, JSON-LD URLs,
  `robots.txt`, and `sitemap.xml` all use `https://appcraftdigital.co.in`
- [x] **Clean schema** — removed placeholder ratings and invalid site-search markup
- [x] **Internal linking** — every page links to every other page
- [x] **Keyword-rich body copy** (no stuffing), mobile-responsive, fast (no JS frameworks)
- [x] `<html lang="en">`, descriptive link text, `rel="noopener"` on external links

## Part B — Off-page / account actions (TODO, owner only)

These have a **much bigger ranking impact** than any code change. Do them in order.

### 1. Google Search Console (highest priority)
1. Go to https://search.google.com/search-console
2. Add a property for `https://appcraftdigital.co.in`.
3. Verify ownership (GitHub Pages sites can be verified via the HTML tag method —
   paste the meta tag into each page's `<head>`, or use the Google Analytics method).
4. Submit the sitemap: `https://appcraftdigital.co.in/sitemap.xml`
5. Use **URL Inspection → Request Indexing** for each of the 5 pages.

### 2. GitHub Pages domain settings
- In Settings → Pages, confirm the custom domain is `appcraftdigital.co.in`.
- Enable **Enforce HTTPS** once GitHub allows it.
- Keep the repo `CNAME` file set to `appcraftdigital.co.in`.

### 3. Backlinks (the main ranking currency)
- Link to the site **from each app's Play Store listing** (Developer website field +
  app description footer).
- Add the site URL to your **GitHub profile**, README files, and bio links.
- Write on Reddit (r/androidapps, r/privacy), X, Product Hunt, and app-review blogs.
- Reach out to "best app locker 2026" / "Cam Scanner alternative" listicle authors.

### 4. Keep content fresh
- Update `<lastmod>` in `sitemap.xml` whenever you change a page.
- Add real app screenshots once available, especially on the app detail pages.
- Add `aggregateRating` only after you have real public Play Store ratings.

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
