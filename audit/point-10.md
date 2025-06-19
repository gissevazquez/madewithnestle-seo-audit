# Point 10 – Structured Data Markup Analysis

As part of the technical SEO audit, I examined the presence of structured data (schema markup) on both the homepage and a product/recipe page of **madewithnestle.ca** to determine whether the site is leveraging this important feature to enhance its search visibility.

---

## What is Structured Data?

Structured data is a standardized format used to annotate the content of web pages, helping search engines better understand the context and meaning of the information. Google, Bing, and other engines use structured data to enable **rich results**, such as:

- Review stars
- FAQs
- Recipe instructions
- Images and video previews
- Product availability and price

The most commonly used vocabulary is [Schema.org](https://schema.org), and the recommended implementation is using `JSON-LD` inside a `<script type="application/ld+json">` tag in the HTML of the page.

---

## Pages Tested

1. **Homepage** – https://www.madewithnestle.ca/
2. **Recipe Page** – https://www.madewithnestle.ca/recipes/original-smarties-cookies-recipe

Tests were conducted using both:
- [Google’s Rich Results Test](https://search.google.com/test/rich-results)
- [Schema Markup Validator (schema.org)](https://validator.schema.org/)

---

## Audit Findings

| Page              | Structured Data Found | Rich Results Eligibility | Notes                                       |
|-------------------|------------------------|--------------------------|---------------------------------------------|
| Homepage          | No                     | No                       | No schema types like Organization, WebPage, Breadcrumb detected |
| Recipe Page       | No                     | No                       | Missing Recipe schema, despite being a recipe |

> Additional inspection via Chrome DevTools confirmed that there is no `<script type="application/ld+json">` on either page. The only `application/json` found is Drupal's internal settings configuration (not SEO-relevant).

---

## Recommendations

### 1. Add Organization Schema to Homepage
```json
{
  "@context": "https://schema.org",
  "@type": "Organization",
  "name": "Made With Nestlé Canada",
  "url": "https://www.madewithnestle.ca/",
  "logo": "https://www.madewithnestle.ca/path-to-logo.png",
  "sameAs": [
    "https://www.facebook.com/nestleca",
    "https://www.instagram.com/nestlecanada/",
    "https://www.youtube.com/user/nestlecanada"
  ]
}
{
  "@context": "https://schema.org",
  "@type": "Recipe",
  "name": "Original SMARTIES Cookie Recipe",
  "author": {
    "@type": "Organization",
    "name": "Nestlé Canada"
  },
  "image": "https://www.madewithnestle.ca/path-to-cookie-image.jpg",
  "recipeIngredient": [
    "1 cup flour",
    "1/2 cup sugar",
    "1/2 cup butter",
    "1 pack SMARTIES"
  ],
  "recipeInstructions": [
    "Preheat oven to 350°F.",
    "Mix all ingredients.",
    "Bake for 10–12 minutes."
  ],
  "cookTime": "PT12M",
  "prepTime": "PT10M",
  "totalTime": "PT22M",
  "recipeYield": "12 cookies",
  "description": "A fun and colorful SMARTIES cookie recipe perfect for kids."
}
