# Point 6 – HTML Structure Analysis (Headings)

As part of the technical audit, I analyzed the HTML heading structure of both the homepage and a product/recipe page to assess whether the pages follow a semantic, accessible, and SEO-friendly structure. Proper use of heading tags is important for both user experience and search engine crawlers to understand the hierarchy and context of content.

## Pages Analyzed

- Home Page: `https://www.madewithnestle.ca/`
- Product/Recipe Page: `https://www.madewithnestle.ca/recipes/original-smarties-cookies-recipe`

---

## Home Page

### Observations

- The homepage contains **two `<h1>` tags**, both reading:  
  `Essentia® Ionized alkaline water pH 9.5 (or higher)`
- This heading is related to a product and not reflective of the overall site content or purpose.
- There are no visible `<h2>`, `<h3>`, or lower-level heading tags present in the structure.

### Issues Identified

- Using more than one `<h1>` tag breaks semantic HTML practices and may confuse crawlers.
- The `<h1>` content is promotional rather than descriptive of the site.
- The lack of heading hierarchy (no `<h2>`, `<h3>`, etc.) makes the structure flat and non-informative.

### Recommendations

- Ensure the homepage has only one `<h1>` tag.
- Rewrite the `<h1>` to reflect the main purpose of the website.  
  **Recommended `<h1>`:**  
  `Made With Nestlé Canada – Recipes, Brands & Products You Love`
- Introduce a structured heading hierarchy:
  - `<h2>` tags for key content blocks like "Featured Products", "Our Recipes", "Sustainability"
  - `<h3>` tags for subsections if applicable within each content block
- Review all homepage banners and ensure that decorative headings are not mistakenly marked as `<h1>`.

---

## Product/Recipe Page: SMARTIES Cookies

### Observations

- The page contains **one `<h1>` tag**:  
  `Canadian SMARTIES Cookies`
- There are **two `<h2>` tags**, both with the same text:  
  `What you need`

### Issues Identified

- Having the same `<h2>` repeated does not provide additional value or clarity.
- There is no use of `<h3>` or deeper heading levels to organize the rest of the content such as preparation steps or notes.
- Headings are possibly being reused for styling purposes rather than for structure.

### Recommendations

- Keep the `<h1>` tag as it is — it clearly identifies the content of the page.
- Modify the `<h2>` tags to avoid duplication and improve semantic clarity.  
  **Suggested alternatives:**
  - First `<h2>`: `What You Need to Bake`
  - Second: `Ingredients for SMARTIES Cookies`
- Use `<h3>` tags for sub-sections, such as preparation steps, storage tips, or variations.
- Make sure future product or recipe pages use consistent structure:
  - One unique `<h1>` per page
  - `<h2>` for main content blocks (Ingredients, Instructions, Tips)
  - `<h3>` for any sub-sections

---

## Final Evaluation

The homepage currently lacks proper semantic structure due to multiple `<h1>` tags and missing secondary headings. The product page performs better in terms of heading use but could still benefit from improved hierarchy and non-repetitive heading content.

By applying a clear and logical heading hierarchy, both user experience and SEO performance can be significantly improved across the site.
