# Hewad Market, version 4: Apple-style sections after the film

Open `index.html` from a local web server (in this folder run `npx http-server`, then open the address it prints). Video scrubbing needs a server; Safari may refuse it from a double-clicked file. On a phone, watch `preview-phone.mp4`. On a laptop, watch `preview-desktop.mp4`.

## What changed from v3
- **The walk-in film is untouched.** Same two video files, same HTML, CSS and scroll logic (checked line by line against v3).
- **Everything after the film was rebuilt** in the style of the Apple Intelligence screenshots, with ideas from Stellar and Stillform:

| Section | Modelled on | What it does |
|---|---|---|
| Nav | Apple global bar + pill sub-nav | Translucent bar with the gold wordmark, Directions and Call. Below it, a row of pills (Walk in, Aisles, Brands, Prices, Visit). The active pill follows your scroll with a spring. The bar turns light over the light sections. |
| Statement | Stellar's "From historic blocks [photo]…" | One sentence with small photos set inline. The words light up one by one as you scroll. |
| Take a walk around the shop | Apple's big autoplay carousel (dots + pause) | 5 real aisle photos. Autoplays every 6 s, with a pause button. You can swipe or drag it: it follows your finger 1:1, rubber-bands at the ends and throws to the next slide with momentum. |
| Six kitchens. One shop. | Apple "And so much more" grid + Stellar key figures | 6 regions × 20+ brands, from hewadmarket.fi. Numbers count up when they come into view. |
| Real prices. Off real labels. | Apple light section | The real jam-shelf photo with tappable pins. Tap a jar or label and a frosted price tag appears. The list beside it highlights the matching pin. |
| Visit | Apple Maps Flyover card + privacy panel | The high-res shopfront photo with a frosted "maps" bar and directions button, an hours card with live Open/Closed status (Finnish time), and a "Looking for something?" panel with phone, email, TikTok and Facebook. |
| Footer | Apple fine print | Notes, breadcrumb, 4 small columns, copyright. |

Fonts: SF Pro on Apple devices (system font, like apple.com), Inter everywhere else. Young Serif only for the wordmark and inside the film.

Accessibility: reduced motion turns off autoplay, counters and scroll effects. Reduced transparency makes the glass surfaces solid. The carousel works with arrow keys.

## Media
| File | Source |
|---|---|
| `walk-16x9.mp4`, `walk-9x16.mp4`, posters | Unchanged v3 film |
| `rice-aisle.jpg`, `storefront.jpg`, `main-aisle.jpg` | New: the shop's own photos from hewadmarket.fi, at higher resolution |
| `aisle-*.jpg`, `jams-wide.jpg`, `freezers.jpg`, `door-winter.jpg` | Your photos from earlier versions |

## Check with the owner before showing this to them
1. **Opening hours conflict.** hewadmarket.fi says Mon–Fri 9–21, Sat 9–21, Sun 10–20 (Google also says 21). The door notice in your photo says Mon–Fri 9–20, Sat–Sun 10–20. The Visit section uses the website hours. The film still shows the door-notice hours in its "MA–PE 9–20 · LA–SU 10–20" caption, because the film was kept exactly as it was. One of the two needs to change.
2. **Halal meat.** The website says they sell fresh halal meat. None of the photos show a meat counter. A photo of it would make a strong extra slide.
3. **"Over 120 brands"** is 6 regions × "20+" from their website, not a number the owner gave.
4. **Prices** were copied from one shelf photo and will go out of date. In Shopify they should come from the product catalogue.
5. **Email** `almasharakat@gmail.com` is the one listed on hewadmarket.fi. Check that it's the one they want public.
6. "Mango from Yemen" and "cassava" are still in the film captions from v3 (unverified).
7. Copy is English only. A Finnish version is needed.

## Not done yet
- A Shopify theme. Each section maps to one Liquid section.
- The two film files are 7 MB each, which is heavy on mobile data. Re-encode before launch.
