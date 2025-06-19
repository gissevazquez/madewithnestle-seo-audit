# Point 9 – Page Speed Analysis & Recommendations

As part of the technical SEO audit, I evaluated the page speed performance of **madewithnestle.ca** using **Google PageSpeed Insights** for both mobile and desktop. The evaluation focuses on Core Web Vitals, performance metrics, and diagnostic recommendations to improve the overall user experience and SEO.

---

## Pagespeed Summary

| Metric                    | Mobile         | Desktop        | Threshold (Good)  |
|---------------------------|----------------|----------------|-------------------|
| Largest Contentful Paint  | 22.2 s         | 3.4 s          | < 2.5 s           |
| First Contentful Paint    | 5.2 s          | 0.7 s          | < 1.8 s           |
| Time to First Byte (TTFB) | 0.9 s          | 0.6 s          | < 0.6 s           |
| Total Blocking Time       | 1,130 ms       | 840 ms         | < 200 ms          |
| Speed Index               | 9.6 s          | 2.7 s          | < 4.3 s           |
| Cumulative Layout Shift   | 0              | 0.001          | < 0.1             |
| Overall Performance Score | 34             | 47             | 90–100            |

---

## Key Issues Identified

### Mobile

- Very high **LCP** (22.2 s) and **FCP** (5.2 s).
- Heavy **JavaScript execution time** (2.3 s).
- **Third-party scripts** blocking main thread (1,140 ms).
- Unoptimized, non-modern image formats.
- Several unused CSS and JavaScript files loading.
- Excessive **DOM size** (1,397 elements).
- Poor **Speed Index** and **Total Blocking Time**.

### Desktop

- Better but still problematic LCP (3.4 s).
- High **TBT** and several **unused resources**.
- **JavaScript blocking time** of 2.4 s.
- Render-blocking resources and unnecessary third-party code.

---

## Recommendations

### 1. Optimize Images

- Convert images to modern formats like **WebP**.
- Implement **lazy loading** for offscreen images.
- **Compress and resize** large images for mobile.

### 2. Minimize JavaScript & CSS

- Remove **unused JavaScript** (1.7 MB potential saving).
- **Defer** or **async load** non-critical JS.
- Minify and combine CSS files.
- Enable Drupal’s **CSS aggregation** and **JS compression**.

### 3. Improve Rendering Efficiency

- Eliminate **render-blocking resources** (inline critical CSS).
- Reduce **DOM size** and complexity (avoid 1,300+ elements).
- Audit and clean up **third-party tags** (GTM, Gigya, AddToAny).

### 4. Address Core Web Vitals

- Focus on reducing **LCP** by prioritizing the hero image.
- Optimize TTFB by enhancing server response times.
- Improve **TBT** by deferring heavy JavaScript modules.

---

## Final Thoughts

The site currently fails the **Core Web Vitals assessment**, especially on mobile devices. Page speed is a direct ranking factor and essential for user retention. Prioritizing image optimization, reducing script execution, and minimizing unused resources will significantly improve both UX and SEO rankings.

---

**Prepared by:** Gisselle  
**Role:** SEO Search Analyst – Technical Assessment  
**Audit Date:** June 2025
