# Point 7 – Image Optimization & ALT Text Audit

## Overview

As part of my technical SEO audit, I evaluated all images on the website to determine whether they are optimized for search engines and accessibility. The main focus was verifying the implementation of the `alt` attribute, checking for proper use, and identifying potential improvements.

## Why ALT Text Matters

ALT (alternative) text serves several key purposes:

- **Accessibility**: It helps screen readers describe images to visually impaired users.
- **SEO context**: Google uses it to understand image content and associate it with relevant queries.
- **Fallback content**: Displays when an image fails to load.
- **Image search optimization**: Well-written ALT text can boost visibility in Google Images.

## What I Found

Using Screaming Frog, I scanned a total of **158 images** across the site. The results are summarized below:

| Issue Detected               | Count | % of Total |
|-----------------------------|-------|------------|
| Missing ALT text            | 36    | 22.78%     |
| Missing ALT attribute       | 10    | 6.33%      |
| Images over 100KB in size   | 25    | 15.82%     |
| Indexable images            | 158   | 100%       |

Additionally, most images are served from internal sources and are properly linked throughout the site. However, the lack of ALT text on nearly one-third of images is a concern.

## Issues Identified

- **Missing descriptive ALT text** for key images (including banners and product thumbnails).
- **No ALT attribute at all** on decorative elements, which can confuse screen readers.
- **File sizes** over 100KB detected – these could affect load speed and Core Web Vitals.

## Recommendations

I recommend the following actions to improve image SEO and accessibility:

1. **Add meaningful ALT text** to all content images:
   - Example:  
     Bad: `alt=""`  
     Good: `alt="Drumstick Ice Cream Cone with chocolate shell"`

2. **Use `alt=""` on purely decorative images** to inform screen readers to skip them.

3. **Avoid keyword stuffing** in ALT tags. Keep them natural and descriptive.

4. **Compress large images** over 100KB using WebP or optimized JPEG/PNG formats to reduce page load time.

5. **Audit ALT consistency across languages** if the site is multilingual (EN/FR hreflangs suggest this).

## Final Thoughts

While the majority of images are functioning correctly, the missing ALT text presents both an SEO opportunity and an accessibility issue. Implementing proper ALT tags will improve the site’s compliance with WCAG standards, enhance search performance, and offer a better user experience.

