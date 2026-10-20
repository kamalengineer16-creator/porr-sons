# P. Orr & Sons — Watch Storefront POC

A responsive, static storefront concept inspired by P. Orr & Sons' heritage. Built as a demo only; this is not an official website or an affiliated commerce integration.

## Demo features
- Responsive watch catalogue with brand, category, search, and price sorting
- Product cards show sample price and stock status
- Add-to-bag, quantity controls, subtotal, and demo checkout enquiry
- **Stock Desk** lets you edit sample inventory quantities and prices; the catalogue updates immediately
- Inventory and cart persist in the current browser via `localStorage`
- No build step, framework, backend, API keys, or install required

## Run locally
Open `index.html` in a modern browser. An internet connection is needed for Google Fonts and remote product photography.

## Deploy on GitHub Pages
1. Create a new public GitHub repository, for example `orr-sons-store-poc`.
2. Upload `index.html` and `README.md` to the repository root and commit to `main`.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/(root)`, then Save.
5. Wait for the deployment and open the Pages URL shown in Settings → Pages.

GitHub Pages serves static files; it does not provide a database, server-side stock control, authentication, payment processing, or order management. This POC's stock edits are local to one browser and are not shared across customers.

## Before a production launch
- Confirm brand permission, product imagery, product catalogue, and brand assets.
- Replace demo data with an authenticated backend and inventory/POS integration.
- Implement customer accounts if needed, order management, shipping/tax, returns, and customer support flows.
- Integrate a payment provider; never store card details in this frontend.
- Add role-based staff login, audit trail, server-side stock reservation, and concurrency protection.
- Add privacy policy, terms, shipping/returns, accessibility and security reviews.

## Project structure
- `index.html` — complete storefront and demo inventory UI
- `README.md` — setup, deployment, and production notes
