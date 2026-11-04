# LUMIÈRE — Luxury Cosmetics Website

A luxury, dark-themed e-commerce storefront for a cosmetics brand, built as a single self-contained HTML file with vanilla HTML, CSS and JavaScript. No build step, no dependencies.

## Features

**Shopping**
- Product grid with category tabs, search, sorting, concern and price filters
- Product pop-ups with shade swatches or sizes, how-to-use tips, stock status and reviews
- Shopping bag with discount codes and a free-delivery progress bar
- Wishlist, recently viewed strip and side-by-side product comparison (up to 3)
- Curated gift sets with optional gift messages
- M-Pesa-style checkout form with delivery fees by county (demo, see below)

**Discovery**
- Shade finder quiz and a skincare routine builder (oily, dry, combination, sensitive)
- Before/after slider, customer reviews, FAQ and brand story

**Experience**
- Light and dark theme toggle
- Announcement bar, sale countdown, cookie notice, Privacy Policy and Terms pop-ups
- Floating WhatsApp button and a contact form that opens WhatsApp
- Responsive layout, sticky mobile add-to-bag, accessibility improvements (skip link, focus styles, keyboard support, reduced motion)
- SEO meta tags, structured data for products, and PWA files (`manifest.json`, `sw.js`, `icon.svg`)

## Getting started

```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
# open index.html in your browser, or serve it locally:
npx serve .
```

## Before going live

This is a frontend template. Replace or connect the following:

| Item | Where |
|---|---|
| Brand name, logo, colours | `index.html` (CSS variables at the top of `<style>`) |
| Products, prices, shades, stock | `P`, `SWT`, `ST`, `CON` arrays in the script |
| WhatsApp number | Search for `254700000000` |
| Contact details, address, hours | Contact section |
| Discount codes | `WELCOME10`, `LUMIERE15` in the `ap` click handler |
| Sale end date | `SALE_END` in the script |
| Privacy Policy and Terms | `LG` object in the script (generic templates, have them reviewed) |
| Before/after images | The slider is an illustration, replace with real client photos |
| PWA icons | Add `icon-192.png` and `icon-512.png` |

## Roadmap

- [ ] Node.js / Express / MongoDB backend (products, orders, users, stock)
- [ ] Real M-Pesa payments via the Safaricom Daraja STK Push API
- [ ] Admin dashboard for products and orders
- [ ] Customer accounts, order tracking and loyalty points
- [ ] Order confirmation emails and SMS
- [ ] Swahili language switch
- [ ] Real product photography

## Notes

- Checkout is a **demo**. It validates the M-Pesa number and calculates totals but does not take payment.
- Reviews, stock levels and the notify-me form are not stored anywhere yet; they need the backend.
- Wishlist and cookie choice are saved in the browser's local storage.

## Tech

HTML5 · CSS3 (custom properties, grid, flexbox) · Vanilla JavaScript · Google Fonts (Cormorant Garamond, Inter)

## License

MIT. Add a `LICENSE` file if you publish this.
