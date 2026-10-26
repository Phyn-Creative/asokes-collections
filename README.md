# ASOKE'S COLLECTIONS — boutique storefront

A responsive, static storefront for Asoke's Collections, designed for free hosting through the existing GitHub and Cloudflare setup. No build command or paid storefront platform is required.

## Current storefront

- Boutique-style homepage and responsive mobile navigation
- Category browsing for scarves, crafts, beauty and apparel
- Nine scarf styles with supplied prices in NGN
- Search and sorting for listed scarf products
- Add-to-bag, quantity adjustment, remove, clear and subtotal
- WhatsApp order handoff with order details prefilled
- Direct WhatsApp contact link
- Responsive layout and SVG favicon

## Product information

The supplied scarf catalogue is listed in `script.js`:

- Normal Thrifted Scarves — ₦1,200
- Premium Thick Thrifted Scarves — ₦1,500
- Vintage Scarves — ₦1,800
- Jersey Scarves — ₦2,000
- Crinkle Scarves — ₦2,500
- Ball Chiffon Scarves — ₦3,000
- Plain Chiffon Scarves — ₦3,500
- Rainbow Chiffon Scarves — ₦3,500
- Medium Jersey Scarves — ₦4,000

Crafts, beauty and apparel categories are present in the storefront navigation, but they are not populated with product listings yet because their actual products, prices and details have not been supplied. Selecting one directs customers to a WhatsApp enquiry rather than showing invented stock.

## Before launch

1. Confirm the WhatsApp number in `script.js` and in the direct WhatsApp links in `index.html`. Use international digits only (Nigeria: `234` followed by the number without the leading `0`).
2. Replace editorial Unsplash imagery with the seller's actual product and category photos when available. Current product images are visual placeholders and are not verified photos of actual stock.
3. Confirm the displayed prices, product availability, colours and delivery arrangements with the seller.
4. Test the contact link and a complete cart-to-WhatsApp checkout on the deployed website.

## Deployment

The project is a static HTML/CSS/JavaScript site. Keep using the existing Cloudflare deployment and GitHub repository `Phyn-Creative/asokes-collections`. If Cloudflare is connected to the repository, commits to the configured branch should trigger its deployment workflow; otherwise deploy the latest repository contents using the existing Cloudflare setup.

This front end does not take online payments and does not have a stock database, persistent cart, customer accounts or an order-management dashboard. The cart is held in the current browser session and WhatsApp is the order handoff.
