# Technical SEO Audit – Point 1

## ✅ Overview

As part of my application for the SEO Search Analyst position at Nestlé, I performed a full technical SEO audit of [https://www.madewithnestle.ca](https://www.madewithnestle.ca) using Screaming Frog.

This document presents my findings and SEO recommendations based on the crawl and review of key technical elements across the site.

---

## 1. 404 and 403 Errors

During the crawl, I identified:
- 3 URLs returning a **404 (Not Found)** error
- 1 URL returning a **403 (Forbidden)** error

Some of these broken pages were still being linked internally over 100 times, which could negatively affect crawl efficiency and user experience.

**Recommendation:** I suggest removing or redirecting these URLs to relevant live pages and updating internal links accordingly.

---

## 2. Redirects

I found:
- 22 permanent (301) redirects
- 1 permanent (308) redirect

There were no redirect chains or loops, which is a good sign.

**Recommendation:** I recommend keeping redirect types consistent (using 301s) and replacing redirected internal links with their final destination to streamline crawling.

---

## 3. Canonical Tags

All scanned pages had self-referencing canonical tags.

**Observation:** This implementation prevents duplicate content issues and signals the correct version of each page to search engines.

---

## 4. Meta Tags

From the audit, I observed the following issues with meta descriptions:

- 6 indexable pages are missing a meta description
- 56 pages have descriptions exceeding 155 characters
- 44 pages have descriptions shorter than 70 characters
- No duplicate meta descriptions were found, which is positive

**Recommendation:** I recommend writing clear, concise, and keyword-optimized meta descriptions for all pages. Descriptions should ideally be between 140–155 characters to ensure proper display in search results. Pages without descriptions should be prioritized for optimization to improve click-through rates (CTR).

## 5. Indexability

Out of all crawled URLs, **27 were marked as “Not Indexable”**, with the following breakdown:
- 16 were **redirects**, which is expected behavior
- 8 were **canonicalized** to clean or main versions of their content
- 3 returned **4xx errors** (403/404), which should be corrected

There were no pages blocked by `robots.txt`, and no use of the `noindex` directive.

**Observation:** All canonical tags were reviewed and found to be pointing to valid, appropriate destination URLs. The non-indexable status of these pages is justified and correctly configured. Only the 3 error pages require fixing.

## 6. Sitemap.xml

The sitemap includes only 9 URLs, most related to a specific section (Nature’s Heart). Also:
- Some URLs have outdated last modified dates
- A few URLs (e.g., `/node/10269`) use non-SEO-friendly structures

**Recommendation:** I suggest updating the sitemap to include all important site pages, with clean URLs and accurate modification dates.

## 7. Hreflang Usage

In the HTML source, I found that most pages include `hreflang="en"`. However:
- There is no connection to French versions (`hreflang="fr"`)
- The attribute `x-default` is also missing

**Recommendation:** I recommend implementing full hreflang mapping between English and French versions, and adding `x-default` to improve SEO for multilingual users.

## 8. HTTPS

All scanned URLs used HTTPS, and there were no HTTP versions detected.

**Observation:** HTTPS is well-implemented across the site and contributes positively to SEO and user trust.

## 9. SEO-Friendly URLs

While most URLs are clean, I found the following issues:
- 5 URLs contain non-ASCII characters
- 8 use underscores `_` instead of hyphens `-`
- 3 contain uppercase letters
- 8 include dynamic parameters
- 1 URL is longer than 115 characters

**Recommendation:** I suggest standardizing URLs to lowercase, using hyphens, avoiding special characters and excessive length, and reducing query parameters where possible.

## 10. Structured Data

Using Google’s Rich Results Test, I confirmed that:
- The homepage and recipe pages have **no structured data implemented**

**Recommendation:** I recommend implementing structured data using JSON-LD for entities like `Organization`, `Product`, and `Recipe`, to increase visibility through enhanced search listings (rich results).

## ✉️ About Me

Prepared by: **Gisselle**  
Candidate – SEO Search Analyst at Nestlé  
Audit completed: **June 2025**