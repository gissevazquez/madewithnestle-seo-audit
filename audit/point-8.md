# Point 8 – SEO-Friendly URLs Audit

As part of my technical audit, I evaluated 10 key URLs from the website to assess whether they follow SEO best practices for clean, readable, and indexable URL structures.

## Why SEO-Friendly URLs Matter

URLs are not just technical paths — they also communicate content meaning to users and search engines. A well-structured URL helps:

- Improve click-through rates from search results
- Enhance crawlability for search engines
- Provide a better user experience

## SEO Criteria Used

The following best practices were used to evaluate each URL:

| Criterion | Best Practice |
|----------|----------------|
| HTTPS | Secure protocol preferred for all URLs |
| Readable structure | Human-friendly, meaningful words (no symbols, gibberish) |
| No dynamic parameters | Avoid query strings unless necessary |
| No uppercase or special characters | Should be lowercase, avoid accents |
| Use of hyphens `-` | Separate words clearly with hyphens, not underscores |
| Concise | Shorter is better, without keyword stuffing |

## URLs Reviewed

| URL 	            | HTTPS | Readable | Parameters | Hyphens Used | Issues |
|-----|-------------|-------|----------|------------|--------------|--------|
| `/` 	            | Yes   | Yes      | No         | No           | None |
| `/about-us`       | Yes   | Yes      | No         | Yes          | None |
| `/aero`           | Yes   | Yes      | No         | No           | None |
| `/articles`       | Yes   | Yes      | No         | No           | None |
| `/big-turk`       | Yes   | Yes      | No         | Yes          | None |
| `/nido`           | Yes   | Yes      | No         | No           | None |
| `/nescafe`        | Yes   | Yes      | No         | No           | None |
| `/nesfruta`       | Yes   | Yes      | No         | No           | None |
| `/nesquik`        | Yes   | Yes      | No         | No           | None |
| `/nestlé-materna` | Yes   | Yes      | No         | Yes          | Uses accented character `é` (not recommended) |

## Recommendations

- Avoid using accented characters in URLs. Although `/nestlé-materna` is technically valid, characters like `é` can lead to encoding issues and negatively impact indexing. Replacing it with `/nestle-materna` is recommended.
- Maintain the current clean structure for other URLs. All are short, readable, and free from dynamic parameters.
- Continue applying these best practices in all new content to preserve consistency and avoid crawl issues or duplicate paths.

## Tools Used

- Screaming Frog SEO Spider
- Manual URL inspection in browser

_Last reviewed on: June 2025_
