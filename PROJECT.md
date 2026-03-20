# Apple Shop Checkout — Project Documentation

## Project Summary

A pixel-perfect, Apple-inspired **checkout page** built using pure HTML, CSS, and a minimal Node.js server. Designed for simplicity, visual polish, and zero external dependencies.

---

## Tech Stack

| Layer | Technology |
|---|---|
| Markup | HTML5 (semantic) |
| Styling | Vanilla CSS3 (Grid, Flexbox, animations) |
| Typography | Inter (Google Fonts) |
| Icons | Inline SVG |
| Server | Node.js `http` module |
| Port | `8080` |

---

## File Reference

### `index.html`
The single-page application entry point.

- `<main class="checkout-container">` — outer container with frosted-glass effect
- `<section class="summary-section">` — product list, coupon field, and price totals
- `<section class="form-section">` — contact form (name, email, country dropdown)
- Inline SVG icons for iPhone, Apple Watch, and iMac

### `style.css`
All visual styles and animations.

- `:root` CSS variables for colors, border-radius, shadow
- `.background-overlay` — dual radial-gradient dark background
- `.checkout-layout` — 2-column CSS Grid (`1.5fr 1fr`)
- `.product-item` — Flexbox row with staggered `fadeIn` animation
- Responsive breakpoints at `850px` and `480px`

### `server.js`
Lightweight static file server.

- Uses Node.js built-in `http` and `fs` modules
- Resolves correct MIME types for all static assets
- Listens on port `8080`

---

## Design System

### Color Palette

| Token | Value | Usage |
|---|---|---|
| `--primary-bg` | `#f5f5f7` | Page/input background |
| `--container-bg` | `#ffffff` | Card background |
| `--text-primary` | `#1d1d1f` | Headings, prices |
| `--text-secondary` | `#86868b` | Labels, subtitles |
| `--accent-color` | `#0071e3` | Focus rings (Apple blue) |
| Body background | `#0b0c10` | Dark backdrop |

### Typography
- Font: **Inter** (weights: 300, 400, 500, 600, 700)
- Fallback stack: `-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica, Arial`

### Animations
- `fadeIn` keyframe: `opacity: 0 → 1`, `translateY(10px → 0)`
- Product items stagger with `0.1s`, `0.2s`, `0.3s` delays
- Product icon scales to `1.1x` on hover
- Remove button transitions to `#ef4444` on hover

---

## Cart Data

| Product | Variant | Qty | Price |
|---|---|---|---|
| iPhone 12 Pro | Golden | 1 | $999.00 |
| Apple Watch | Blue | 1 | $399.00 |
| iMac | Green | 1 | $1,199.00 |
| **Subtotal** | | | **$2,597.00** |
| **Tax (24%)** | | | **$623.28** |
| **Total** | | | **$3,220.28** |

---

## Running Locally

```bash
node server.js
# → Server running at http://localhost:8080/
```

**Requirements:** Node.js installed (no npm packages needed).

---

## Future Improvements

- [ ] Add JavaScript to dynamically calculate totals
- [ ] Implement working coupon code validation
- [ ] Add item quantity controls (increment/decrement)
- [ ] Connect to a payment gateway (Stripe)
- [ ] Add success/confirmation screen after checkout
- [ ] Persist cart state using `localStorage`
