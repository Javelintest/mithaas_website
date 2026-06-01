# Mithaas Exports — Embed Pages (v2)

A complete, multi-page export catalogue built from your Mithaas Export
Catalogue PDF. 8 pages, 83 SKUs, 92 photographs.

## What's inside

```
mithaas-export-page/
├── index.html                  ← main landing (74 SKUs, 8 category cards)
├── categories/                 ← detail page per category
│   ├── desi-ghee-sweets.html      (16 sweets)
│   ├── dry-fruit-sweets.html      (13 premium sweets)
│   ├── bengali-sweets.html        (6 chenna sweets)
│   ├── ready-gravies.html         (19 ready meals)
│   ├── indian-snacks.html         (12 fryables)
│   ├── indian-breads.html         (13 breads & parathas)
│   └── indian-dips.html           (4 chutneys)
├── images/
│   ├── hero-spread.jpg, gulab-jamun.jpg, kaju-katli.jpg, ...  (11 hero shots)
│   └── products/               ← per-item product photo (81 files)
└── README.md
```

## How users navigate

1. They land on `index.html` — the editorial export catalogue page.
2. The "The Catalogue" section now has **clickable category cards** —
   each one links to its detail page (e.g. clicking "Desi Ghee Sweets"
   opens `categories/desi-ghee-sweets.html`).
3. Each category page shows the full SKU list with **individual product
   photos, names, descriptions**, plus a how-to-serve strip, prev/next
   nav, and a "Back to all categories" CTA.
4. Breadcrumb at the top of every category page links back to the main
   export page.

## How to deploy

### Option A — Drop into your existing site
```
your-domain.com/store/mithaas/exports/             → index.html
your-domain.com/store/mithaas/exports/categories/* → category pages
```
Just upload the whole folder. Relative paths inside the HTML mean
everything Just Works™.

### Option B — Embed inside another page via iframe
```html
<iframe src="/path/to/mithaas-export-page/index.html"
        style="width:100%; height:100vh; border:0;"
        title="Mithaas Exports"></iframe>
```

### Option C — Inline into a CMS
The main `index.html` and category pages share the same style tokens
but each has its own `<style>` block. Copy each into your CMS's custom
page templates if needed.

## Editing content

All product data for category pages lives in **one place**:
`build_categories.py` (not included in the deliverable — kept in source).
If you want to:

- **Update a description**: open the relevant `categories/*.html` file
  and find the product `<h3>` / `<p>`. Edit and save.
- **Add a new SKU**: ask me to regenerate — I'll update the data file
  and re-emit all category pages with consistent styling.
- **Swap a product photo**: drop your replacement into
  `images/products/<filename>.jpg`. Keep the same filename — no other
  changes needed.

## Fonts

Loaded from Google Fonts via standard `<link>` tags. No local fonts to
manage. The brand stack:

- **Display**: Fraunces (300-500 weight, with optical-size axis)
- **Body**: Manrope (400-700)
- **Handwritten accents**: Caveat (500-600)
- **Cursive script accents**: Allura (regular)

## Brand consistency

Every page in the bundle uses the same:

- Colour palette (deep maroon, crimson, saffron, turmeric, cream)
- Typography (Fraunces + Manrope + Caveat + Allura)
- Component vocabulary (eyebrow labels, italic-accent display titles, pill tags, "100% Vegetarian" green-dot indicator)
- Reveal animations and hover behaviour
- Footer

## Notes on photography

- 11 hero shots were extracted from your PDF for the main page and category heroes.
- 81 individual product photos were generated from the PDF — for SKUs without a unique photo (e.g. multiple ladoos, paratha variants), thematically similar images are used with varied crops to avoid duplication.
- For the cleanest look at scale, consider commissioning a small product-photo shoot of the SKUs that share images. I can swap them in by filename.

## Contact details on every page

- Email: **export@themithaas.com**
- Phone: **+91 84484 92344**
- Head Office: **J-63, Sector 63, Noida, U.P. 201301**
- Certifications: **FSSC 22000 · USFDA · FSSAI · HACCP**

---

Designed with ❤️ for Mithaas · Making traditions trendy · Exported with love from India
