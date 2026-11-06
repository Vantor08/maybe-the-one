# Vallore SuperBalance — Shopify theme

Custom theme converted from the Vallore landing page. The homepage is the full
custom design; product / collection / cart / customer templates are minimal,
working stubs you can build out later.

## Connect to Shopify via GitHub
1. Create a GitHub repo and put the CONTENTS of this folder at the repo root
   (so `assets/`, `config/`, `layout/`, `sections/`, `templates/` are at the top level).
2. Shopify admin → Online Store → Themes → Add theme → Connect from GitHub.
3. Pick the repo/branch. Shopify imports it. Preview, then Publish.

## Videos (optional — section is hidden until you add them)
The "See Vallore in action" video section stays completely hidden until you add
video URLs, so the site looks finished without any videos.
To add them later: upload each video to Shopify (Content > Files), copy its URL,
and paste it between the quotes at the top of `sections/main-page.liquid`
(`assign ritual_video_1 = "https://cdn.shopify.com/..."` through _5). The section
appears automatically once at least one URL is set. Use your OWN Vallore videos
only — not another brand's footage.

## Notes
- All images live in `assets/` and are referenced with `{{ 'name.jpg' | asset_url }}`.
- Styles: `assets/theme.css`  ·  Scripts: `assets/theme.js`
- The buy box / cart drawer are front-end demo logic. To take real orders, wire
  them to real Shopify products & the `/cart` form (the `product.liquid` stub shows the pattern).
