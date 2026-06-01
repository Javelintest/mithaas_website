# Mithaas Website — Homepage + Export Catalogue

A complete, multi-page Mithaas site in one consistent editorial style.
Homepage + export landing + 7 category detail pages. All embed-friendly.

## File structure

```
mithaas-website/
├── index.html              ← HOMEPAGE (new) — embed content, no header/footer
├── export.html             ← Export catalogue landing (8 category cards)
├── categories/             ← Export category detail pages
│   ├── desi-ghee-sweets.html      (16 sweets)
│   ├── dry-fruit-sweets.html      (13 premium sweets)
│   ├── bengali-sweets.html        (6 chenna sweets)
│   ├── ready-gravies.html         (19 ready meals)
│   ├── indian-snacks.html         (12 fryables)
│   ├── indian-breads.html         (13 breads & parathas)
│   └── indian-dips.html           (4 chutneys)
├── images/
│   ├── brand/mithaas-logo.png     (your transparent logo)
│   ├── hero shots (gulab-jamun.jpg, kaju-katli.jpg, …)
│   └── products/                  (81 individual product photos)
└── README.md
```

## The homepage (index.html)

Built as **middle embed content** — no top nav bar, no footer (your existing
Mithaas site already provides those). Everything is wrapped in a single
`.mithaas-home` container so the styles never leak into your site chrome.

### Sections, in order
1. **Hero** — "Making *traditions* trendy, one bite at a time." + stats (2012 · 16+ stores · 100% veg · ₹450 for two)
2. **Our Story** — founded 2012, grown to 16+ NCR outlets, 100% vegetarian
3. **Explore Our Categories** — the "THE CATALOGUE" concept reworked into a 6-card bento grid: Sweets, Namkeen, Chaat, Restaurant, Festive Hampers, and Exports (links to export.html)
4. **Signature Sweets** — 12-photo gallery of bestsellers
5. **The Restaurant** — multi-cuisine vegetarian teaser (North Indian / South Indian / Indo-Chinese)
6. **Shop Online** — Swiggy + Zomato section, styled after your reference screenshot
7. **Bespoke Catering** — Weddings · Diwali Hampers · Baby Showers & Pujas
8. **Visit Us** — 16+ NCR store locations
9. **Testimonials** — customer love
10. **Closing CTA** — "Come, taste the Mithaas difference" + phone

## How to embed

### Option A — Standalone page
Upload the whole `mithaas-website/` folder. `index.html` works as-is.

### Option B — Inside your existing site (recommended)
The homepage is built as embed content. To drop it into a page that already
has your Mithaas header/footer:

1. Copy everything inside `<style>…</style>` (in the `<head>`) into your page.
2. Copy the `<div class="mithaas-home">…</div>` block (the whole body content)
   into your page body, between your header and footer.
3. Copy the `<script>` block at the bottom (scroll-reveal animations).
4. Upload the `images/` folder and keep the relative `images/...` paths,
   or update them to wherever you host the images.

The `.mithaas-home` wrapper scopes all CSS, so it won't clash with your
existing site styles.

## Content notes — please review before publishing

I built every section from the brand facts you shared, but a few items use
**representative placeholder content** that you should confirm or replace:

- **Store locations** — Paras Tierea (Noida 137) is from your Zomato link;
  the other 5 are illustrative NCR locations. Swap in your real outlets.
- **Testimonials** — 3 sample reviews. Replace with real customer quotes.
- **Swiggy / Zomato buttons** — currently link to `#`. Point them to your
  actual store URLs on each platform.
- **Category card links** — Sweets / Namkeen / Chaat / Restaurant / Catering
  link to `#` (placeholders). Exports links to `export.html` (working). Point
  the rest to your real menu/category pages when ready.
- **"Explore our menu" / phone CTAs** — phone is +91 84484 92344 from the
  export catalogue; confirm it's the right public number for the homepage.

## Design system (shared across all pages)

- **Display**: Fraunces (optical-size serif)
- **Body**: Manrope
- **Handwritten accents**: Caveat
- **Cursive script accents**: Allura
- **Palette**: deep maroon, crimson, saffron, turmeric, cream
- Fonts load from Google Fonts (standard `<link>`). No local font setup needed.
- Fully responsive (tested 390px mobile + 1440px desktop)

---

Designed with ❤️ for Mithaas · Making traditions trendy
