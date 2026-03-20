# 🍎 Apple Shop Checkout

A sleek, Apple-inspired **checkout page** built with pure HTML, CSS, and a minimal Node.js static server — no frameworks, no npm packages.

![Apple Shop Checkout](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white)

---

## ✨ Features

- **Apple-style UI** — frosted glass card, dark backdrop with radial gradients
- **2-column layout** — order summary on the left, contact form on the right
- **Staggered animations** — product items fade in with smooth delays
- **Responsive design** — adapts to tablet and mobile breakpoints
- **Zero dependencies** — runs with just Node.js installed
- **SVG product icons** — inline icons for iPhone, Apple Watch, and iMac

---

## 📁 Project Structure

```
applestore/
├── index.html    # Checkout page — layout, products, form
├── style.css     # Styling, animations, responsive rules
├── server.js     # Node.js static file server (port 8080)
├── PROJECT.md    # Detailed project documentation
└── README.md     # This file
```

---

## 🚀 Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) (any recent version)

### Run Locally

```bash
# Clone the repo or navigate to the project folder
cd "apple-shop-checkout/applestore"

# Start the server (no npm install needed)
node server.js

# Open your browser at:
# http://localhost:8080
```

---

## 🛒 Cart Summary

| Product | Variant | Price |
|---|---|---|
| iPhone 12 Pro | Golden | $999.00 |
| Apple Watch | Blue | $399.00 |
| iMac | Green | $1,199.00 |
| **Total** | | **$3,220.28** |

---

## 🎨 Design Highlights

- **Font**: Inter (Google Fonts) — matches Apple's system font feel
- **Colors**: `#0b0c10` dark bg · `#0071e3` Apple blue focus ring · `#1d1d1f` text
- **Animations**: CSS `@keyframes fadeIn` with staggered `animation-delay`
- **Glassmorphism**: `backdrop-filter: blur(10px)` + semi-transparent white card

---

## 📄 License

This project is for educational/portfolio purposes. Apple product names and trademarks belong to Apple Inc.