# ASOKE'S COLLECTIONS — storefront starter

A static, mobile-first scarf storefront for free static hosting on Cloudflare Pages. No database, paid checkout, or build command required.

## Before launch

1. Open `script.js` and replace `STORE.whatsappNumber` with the seller's WhatsApp number in international format, digits only. For Nigeria, use `234` plus the number without its leading `0`.
2. Product images are editorial placeholder images from Unsplash and are not verified photos of actual stock. Replace each product's `image` URL in `script.js` with the seller's own photos when available.
3. Review product names and prices before launch.

## Included

- Nine scarf products and supplied prices in NGN
- Product search and price/name sorting
- Add-to-bag, quantity adjustment, remove, clear, and subtotal
- WhatsApp order message built from cart contents (no payment is taken on the site)
- Responsive layout and favicon

## Deploy to Cloudflare Pages (free plan)

1. In Cloudflare Dashboard, open **Workers & Pages → Create → Pages → Connect to Git** and select `Phyn-Creative/asokes-collections`.
2. Use **Framework preset: None**, leave the build command blank, and set the build output directory to `/` or the repository root (often shown as `.`).
3. Deploy. Cloudflare will provide a `*.pages.dev` address.

This is a front-end storefront. The cart lives in the browser session and WhatsApp is the order handoff; there is no online payment processor, inventory database, or order dashboard in this first version.