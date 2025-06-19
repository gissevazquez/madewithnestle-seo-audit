# Point 3 – Broken Links & Technical Errors

As part of the crawl analysis, I reviewed the internal structure of madewithnestle.ca to detect broken links and technical SEO issues. Below are the findings and my professional recommendations.

---

## 1. Broken Links (4xx Errors)

### ✅ Findings:
- **3 internal 404 Not Found errors**:
  - `/easy-to-prepare-breakfast-recipes-for-busy-mornings`
  - `/coffee`
  - One external image from YouTube (thumbnail)
- **1 internal 403 Forbidden error**:
  - `/world-flavours-contest` – likely restricted or unpublished

These URLs are non-indexable and classified as client errors, which is accurate. However, they are still being linked internally.

---

## 2. Redirects (3xx Status)

- **22 internal URLs return a 301 Moved Permanently status**
- **1 internal URL returns a 308 Permanent Redirect**
- Many of these have a high number of internal links pointing to the redirected URL
  - Example: one redirect receives 150 internal links

This weakens internal link equity and creates unnecessary redirect hops.

---

## 3. Other Technical Observations

- **Redirect chains and unnecessary internal redirects** reduce crawl efficiency
- **Broken image links** (e.g., YouTube thumbnails) negatively impact both user experience and SEO
- **No 5xx server errors** were found, which is positive

---

## Recommendations

1. **Fix or remove all 404 URLs:**
   - Redirect them to the most relevant working pages
   - Or remove internal links that point to them

2. **Investigate the 403 page:**
   - If it's meant to be public, ensure proper access
   - If restricted, remove internal references

3. **Update internal links that point to redirected URLs:**
   - Link directly to the final destination instead of going through 301 or 308 redirects

4. **Fix or replace broken images:**
   - Especially external sources like embedded thumbnails

5. **Continue monitoring for changes:**
   - These issues can recur as the site evolves

---

Overall, madewithnestle.ca shows a technically solid structure with isolated issues. Resolving these will strengthen crawl efficiency and preserve link equity.

---

Prepared by: **Gisselle**  
Position: SEO Search Analyst – Technical Assessment  
Audit Date: June 2025
