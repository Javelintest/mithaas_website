# Mithaas Exports — Embed Page

A self-contained, production-ready export landing page built from your
Mithaas Export Catalogue PDF.

## What's inside

```
mithaas-export-page/
├── index.html       ← the page (single file, ~47 KB)
└── images/          ← 11 product photos (~2.3 MB total, web-optimised)
    ├── hero-spread.jpg
    ├── frozen-food.jpg
    ├── gulab-jamun.jpg
    ├── kaju-katli.jpg
    ├── rasgulla.jpg
    ├── palak-paneer.jpg
    ├── samosa.jpg
    ├── kachori.jpg
    ├── paratha.jpg
    ├── chole-bhature.jpg
    └── chutney.jpg
```

## How to deploy

### Option A — Drop into your existing site
1. Copy the entire `mithaas-export-page/` folder to your web server.
2. Link to it from your navigation, e.g. `https://site.javelin.co.in/store/mithaas/exports/`.
3. Make sure your existing site header/nav doesn't conflict — the page
   currently runs standalone (no nav). If you want it embedded inside
   your existing Mithaas chrome (the maroon top bar with logo, cart,
   etc), let me know and I'll wire it in.

### Option B — Embed inside another page via iframe
```html
<iframe src="/path/to/mithaas-export-page/index.html"
        style="width:100%; height:100vh; border:0;"
        title="Mithaas Exports"></iframe>
```

### Option C — Inline into a CMS
Open `index.html`, copy the contents of the `<style>` block into your
CMS's custom CSS, and the contents of `<body>` into the page body.
Upload the `images/` folder and update the `src="images/..."` paths.

## Fonts

The page loads Fraunces, Manrope, Caveat and Allura from Google Fonts
via the `<link>` in the `<head>`. No additional setup needed — just
make sure your server allows outbound requests to `fonts.googleapis.com`
(it almost certainly does).

## Content

All product names, pack sizes, shelf lives, cooking instructions,
certifications, FAQ answers, and contact details come directly from
your Mithaas Export Catalogue PDF. No content was invented.

- **Hero**: tagline + 4 stats (16+ stores, 60+ SKUs, 12mo shelf life, 100% veg)
- **Our Story**: 2013 origin, 16-store NCR network
- **Process**: 5 steps — Sourcing, Sorting, Production, Packaging, Assurance
- **Catalogue**: 8 product cards covering all 7 categories (74+ SKUs total)
- **Specifications**: shelf life, pack sizes, certifications, vegetarian
- **Certifications**: FSSC 22000, USFDA, FSSAI, HACCP
- **FAQ**: 5 questions (3 from your catalogue + 2 export-specific)
- **CTA**: email export@themithaas.com · +91 84484 92344 · J-63, Sector 63, Noida

## Aesthetic

- **Display**: Fraunces (distinctive optical-size serif with character)
- **Body**: Manrope (clean modern sans)
- **Script accents**: Allura (flowing copperplate cursive) + Caveat (handwritten notes)
- **Palette**: deep maroon, crimson, saffron, turmeric, cream — built off your existing Mithaas brand
- Subtle paper-grain texture, scroll-reveal animations, hover-to-expand SKU lists
- Fully responsive (tested at 390px mobile and 1440px desktop)

## Tweaks you might want

- **Add your top nav bar**: page is currently chromeless. Ping me with
  your site header HTML/CSS and I'll wire it in.
- **Add more photos**: the current 11 images are pulled from the PDF.
  If you have higher-resolution studio shots, replace files in `images/`
  keeping the same filenames — no other changes needed.
- **Change copy**: open `index.html` and search for the section you want
  to edit. Content lives in clearly marked `<!-- ============ -->` blocks.
- **Add a "Download Catalogue" button**: easy to wire into the hero or CTA.

Designed with ❤️ for Mithaas · Making traditions trendy
