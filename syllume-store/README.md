# Syllume candle store — GitHub Pages starter

A polished static-storefront starter built with HTML, CSS and vanilla JavaScript. It includes a responsive home page, five sample catalogue entries, product detail page, filter/search, local cart, rule-based candle finder, checkout demo and supporting policy/contact pages.

## Important: this is a storefront demo, not live ecommerce

- Product names, prices, sizes, descriptions and stock are examples. Edit `products.js` to match real inventory.
- Product images use remote Unsplash URLs. Replace them with original product photos or images you have permission to use.
- `localStorage` only saves a cart in the current browser; it is not a database or order system.
- Checkout is intentionally demo-only. It does not place orders or take payment.
- Contact and newsletter forms show a demo message; they do not transmit data.
- The candle finder is a local rule-based recommendation quiz, not a connected AI service.
- Shipping, returns and privacy are starter templates that must be completed and checked before launch.
- Do not put secret API keys, payment credentials, card data, CVVs or UPI PINs in frontend files or a public repository.

## Project files

- `index.html` — home, catalogue, filter/search, finder and cart drawer
- `style.css` — responsive styling and design system
- `products.js` — editable catalogue data
- `app.js` — cart, filters, product page, finder and demo checkout logic
- `product.html` — product details
- `checkout.html` — demo checkout page
- `about.html`, `contact.html`, `shipping.html`, `returns.html`, `privacy.html` — supporting pages
- `assets/favicon.svg` — tab icon

## Preview on your laptop

1. Download and extract the project ZIP.
2. Open the `syllume-store` folder in VS Code, or open `index.html` directly in a modern browser.
3. Try searching/filtering, adding products, changing cart quantities, opening product details, using the candle finder and testing the checkout demo.

## Publish on GitHub Pages

1. Create a repository, e.g. `syllume-store`.
2. Upload all files and the `assets` folder into the repository root; preserve names and folder structure.
3. Commit to your `main` branch.
4. Open **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select branch `main` and folder `/ (root)`, then save.
7. Open the published URL shown in Pages settings, usually `https://YOUR-USERNAME.github.io/syllume-store/`.
8. Check pages, mobile layout, images, browser console and every navigation link on the published URL.

All internal links are relative and should work under a repository subdirectory.

## Edit products

Open `products.js`. Update `name`, `subtitle`, `category`, `price`, `stock`, `size`, `notes`, `description`, `image`, and `alt`. Keep IDs unique. Replace sample values with verified facts before taking orders. Frontend stock is for display only and cannot prevent overselling in a real store.

## Real payments — safe architecture

GitHub Pages serves static files; it cannot securely hold payment secrets or verify payment. To accept real payments:

1. Choose a payment provider and confirm the merchant account is eligible and approved.
2. Use a secure server-side backend or provider-approved hosted checkout integration.
3. The backend—not browser JavaScript—must validate product IDs, prices, quantities, stock, delivery charges and order totals.
4. Create checkout sessions/orders using server-side credentials; redirect customers to the provider-hosted checkout.
5. Verify payment status/signatures and webhooks on the server before marking any order paid.
6. Store orders in a proper database and send confirmations only after verified payment.
7. Keep all secret keys off GitHub and out of frontend code. Test failures, cancellations, duplicate callbacks and refunds.

Eligibility and age requirements vary by provider. If the account holder is under 18, use a legally eligible adult for accounts that require it; do not enter false identity details.

## Launch checklist

- [ ] Replace sample prices, photos, notes, sizes, stock and descriptions.
- [ ] Verify candle ingredients, care instructions and safety claims for your actual products.
- [ ] Add a business contact method that does not reveal a private home address.
- [ ] Complete shipping, refunds/returns and privacy policy.
- [ ] Connect contact/newsletter forms to a service or backend.
- [ ] Set up real order storage and payment verification before taking money.
- [ ] Test desktop/mobile layouts, keyboard navigation, all links and the browser console.
- [ ] Verify image usage rights and actual published URL.
