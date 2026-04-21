# 🍽️ The Hearthstone Kitchen & Bar — Restaurant Landing Page

A production-ready, single-page restaurant/café website built with **pure HTML, CSS, and vanilla JavaScript** — no frameworks, no build tools, no dependencies. Focused heavily on **on-page SEO** and **local search optimization**.

![Status](https://img.shields.io/badge/status-production--ready-brightgreen) ![HTML](https://img.shields.io/badge/HTML5-semantic-orange) ![CSS](https://img.shields.io/badge/CSS3-responsive-blue) ![SEO](https://img.shields.io/badge/SEO-optimized-success)

---

## 🚀 Quick Start

1. Clone or download this repository
2. Open `index.html` in any browser
3. That's it — zero setup, no build step, no `npm install`

```bash
# Or serve locally
npx serve .
```

---

## 📸 Sections

| Section | Description |
|---------|------------|
| **Hero** | Full-screen cinematic banner with restaurant name (H1), tagline, and dual CTA buttons |
| **About** | Restaurant story with animated highlight badges (Est. 2010, Farm to Table, Open Daily) |
| **Menu** | Tabbed/categorized layout — Starters, Mains, Desserts, Drinks — with 20 items |
| **Gallery** | Grid layout with hover zoom effects, food and ambiance photography |
| **Testimonials** | 3 customer reviews with star ratings and Schema.org Review markup |
| **Contact** | Address, phone (click-to-call), email, hours, Google Maps placeholder, Get Directions CTA |
| **Footer** | Logo, nav links, social media icons, copyright |

---

## 🔍 SEO Features (The Main Focus)

This project is built as a **reference implementation** of restaurant SEO best practices. Every SEO technique is documented in detail in [`SEO-GUIDE.md`](SEO-GUIDE.md).

### Meta Tags
- ✅ Keyword-rich `<title>` tag (under 60 characters)
- ✅ `<meta description>` at 150-160 characters with location + cuisine keywords
- ✅ `<meta keywords>` for secondary search engines
- ✅ `<link rel="canonical">` to prevent duplicate content issues

### Social Media (OG + Twitter)
- ✅ Open Graph tags: `og:title`, `og:description`, `og:image`, `og:url`, `og:type`, `og:locale`, `og:site_name`
- ✅ Twitter Card tags: `twitter:card` (summary_large_image), title, description, image

### Schema.org Structured Data (JSON-LD)
- ✅ `@type: Restaurant` with full business info
- ✅ `PostalAddress` with street, city, state, zip, country
- ✅ `GeoCoordinates` with latitude/longitude
- ✅ `OpeningHoursSpecification` for each day of the week
- ✅ `AggregateRating` (4.8 stars, 342 reviews) — triggers Rich Snippets in Google
- ✅ 3 individual `Review` entries with author, date, rating, and review body
- ✅ `servesCuisine`, `priceRange`, `acceptsReservations`, `menu` URL

### Semantic HTML5
- ✅ `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`
- ✅ `<nav>` with `aria-label` for accessibility
- ✅ Single `<h1>` with logical H2/H3 heading hierarchy
- ✅ Clean section anchor IDs: `#about`, `#menu`, `#gallery`, `#testimonials`, `#contact`

### Image SEO
- ✅ Descriptive, keyword-rich `alt` text on all images
- ✅ `loading="lazy"` on below-the-fold images
- ✅ `width` and `height` attributes to prevent CLS (Cumulative Layout Shift)

### Technical SEO
- ✅ Inline CSS — no render-blocking external stylesheets
- ✅ JavaScript at end of `<body>` — non-render-blocking
- ✅ `preconnect` for Google Fonts
- ✅ `display=swap` on fonts — prevents invisible text
- ✅ Mobile-first responsive design (Google's Mobile-First Indexing)
- ✅ `<meta name="viewport">` for mobile rendering
- ✅ Smooth scroll behavior

### Local SEO
- ✅ Geo meta tags (`geo.region`, `geo.placename`)
- ✅ `tel:` click-to-call links on all phone numbers
- ✅ NAP (Name, Address, Phone) consistency across page + schema
- ✅ Google Maps iframe placeholder
- ✅ "Get Directions" link (Google Maps deep link)

---

## 🎨 Design

| Property | Value |
|----------|-------|
| **Background** | Warm off-white `#FAFAF8` |
| **Text** | Deep charcoal `#1A1A1A` |
| **Accent** | Earthy terracotta `#C4622D` |
| **Secondary** | Sage green `#5C7A5E` |
| **Display Font** | Cormorant Garamond (serif) |
| **Body Font** | DM Sans (sans-serif) |
| **Style** | Editorial food magazine aesthetic |

### Design Features
- 🎯 Sticky navbar with transparent → solid scroll transition
- ✨ Fade-in scroll animations (Intersection Observer API)
- 📱 Fully responsive — desktop, tablet, mobile
- 🍔 Mobile hamburger menu with slide-in panel
- 🔝 Back-to-top floating button
- 📋 Reservation modal with call/email options
- 🖼️ Gallery hover zoom effects

---

## 📁 Project Structure

```
Jaidev Project/
├── index.html          # Complete single-page website (HTML + CSS + JS)
├── README.md           # This file
├── SEO-GUIDE.md        # Detailed SEO explanation document
└── images/
    ├── hero-banner.png     # Hero section background photo
    ├── food-pasta.png      # Gallery: pasta dish photo
    └── cafe-ambiance.png   # Gallery: café interior photo
```

---

## ⚙️ Customization

Search for `<!-- REPLACE WITH YOUR: ... -->` comments in `index.html` to customize:

| What to Replace | How Many Places |
|-----------------|:-:|
| Restaurant/café name | 10+ |
| Phone number | 6 |
| Email address | 3 |
| Street address | 3 |
| City / State | 5 |
| Opening hours | 3 |
| Website URL (canonical, OG, Schema) | 6 |
| Hero image + OG image URL | 4 |
| Google Maps embed `src` | 1 |
| Social media URLs | 3 |
| Menu items & prices | 20 items |
| Customer reviews | 3 reviews |
| GPS coordinates | 1 |

---

## 🚢 Deployment

This is a **static site** — deploy anywhere:

| Platform | Command / Steps |
|----------|----------------|
| **GitHub Pages** | Push to repo → Settings → Pages → Deploy from branch |
| **Netlify** | Drag & drop the folder on [netlify.com/drop](https://app.netlify.com/drop) |
| **Vercel** | `npx vercel` |
| **cPanel** | Upload via File Manager to `public_html/` |
| **Cloudflare Pages** | Connect repo → automatic deploy |
| **Local** | `npx serve .` or just double-click `index.html` |

---

## 🧪 Testing & Validation

After deploying, test your SEO implementation with these free tools:

| Tool | URL | What It Checks |
|------|-----|----------------|
| Google Rich Results Test | [search.google.com/test/rich-results](https://search.google.com/test/rich-results) | Schema.org structured data validity |
| Google PageSpeed Insights | [pagespeed.web.dev](https://pagespeed.web.dev/) | Performance, Accessibility, SEO scores |
| Open Graph Debugger (Facebook) | [developers.facebook.com/tools/debug](https://developers.facebook.com/tools/debug/) | OG tag preview |
| Twitter Card Validator | [cards-dev.twitter.com/validator](https://cards-dev.twitter.com/validator) | Twitter card preview |
| Schema.org Validator | [validator.schema.org](https://validator.schema.org/) | Full Schema.org validation |
| Mobile-Friendly Test | [search.google.com/test/mobile-friendly](https://search.google.com/test/mobile-friendly) | Mobile usability |

---

## 📄 Tech Stack

- **HTML5** — Semantic structure
- **CSS3** — Custom properties, Grid, Flexbox, animations, media queries
- **Vanilla JavaScript** — Intersection Observer, event listeners, DOM manipulation
- **Google Fonts** — Cormorant Garamond + DM Sans
- **No frameworks** — No React, no Vue, no Tailwind, no jQuery
- **No build tools** — No Webpack, no Vite, no npm scripts
- **No external JS libraries** — everything is hand-written

---

## 📝 License

This project is free to use for personal and commercial purposes. Attribution is appreciated but not required.

---

## 👤 Author

Built as a restaurant landing page project with integrated SEO best practices.

---

*For a detailed explanation of every SEO technique used, see [`SEO-GUIDE.md`](SEO-GUIDE.md).*
