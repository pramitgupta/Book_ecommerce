# Leaf & Ledger — Static Book E‑Commerce (Demo)

A fully static, client‑side book store you can host on GitHub Pages. Includes:

- Home, product list, product detail, cart, checkout
- Sign up / log in using localStorage + SHA‑256 (demo only)
- Automatically generated book covers (SVG) based on title/author
- INR currency formatting and simple search/filter

> ⚠️ Security note: This is **not** production-ready auth or checkout. No backend is used. Do **not** use real passwords or personal data.

## Quick start

1. Serve locally (any static server) or push this folder to a GitHub repo and enable **Settings → Pages**.
2. Ensure `index.html` is at the repo root (it is).
3. Visit `/products.html` to browse; click a book to view details. Add to cart and try the demo checkout.
4. Create an account at `/signup.html` (stored only in your browser).

## Structure

```
.
├── index.html          # Home
├── products.html       # Catalog grid + search/filter
├── product.html        # Detail page (uses ?id=...)
├── cart.html           # Cart view
├── checkout.html       # Requires login
├── signup.html, login.html, account.html
├── styles.css
├── js/
│   ├── books.js        # Sample book data
│   ├── covers.js       # SVG cover generator
│   ├── auth.js         # Demo auth (localStorage + SHA-256)
│   └── app.js          # UI + cart logic
└── assets/
    └── favicon.svg
```

## Customising

- Add or edit books in `js/books.js`.
- Tweak styles in `styles.css`.
- The cover generator in `js/covers.js` can be adjusted for different palettes or shapes.
