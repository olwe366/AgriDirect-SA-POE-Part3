# AgriDirect SA

A multi-page B2B marketplace concept connecting South African smallholder farmers with commercial buyers, built with plain HTML, CSS and JavaScript (no frameworks, no build step). This is the complete WEDE5020 Web Development submission, covering **Part 1** (semantic structure), **Part 2** (CSS styling & responsive layout) and **Part 3** (dynamic JavaScript & form validation).

> **Live site:** https://deft-kleicha-aa9f0d.netlify.app/
> **Repository:** https://github.com/olwe366/AgriDirect-SA-POE-Part3.git

---

## Table of Contents
1. [Features](#features)
2. [Pages](#pages)
3. [Tech Stack](#tech-stack)
4. [Project Structure](#project-structure)
5. [Getting Started](#getting-started)
6. [Deployment](#deployment)
7. [Known Limitations](#known-limitations)
8. [Documentation Files](#documentation-files)
9. [Author](#author)

---

## Features
- Produce catalogue of **15 listings** across Vegetables, Fruits and Herbs (5 each), filterable live by category and search term
- Every product card carries a `data-category` attribute, so the JS filter matches reliably instead of scanning visible text
- Enquiry and Contact forms with client-side validation (required fields, inline alerts)
- Two regional hubs on the Contact page — Durban and Cape Town — **each with its own embedded Google Map**
- Standardised footer across all five pages: brand blurb, quick links, contact emails
- Responsive, mobile-first layout: Flexbox/Grid, a 768px tablet/desktop breakpoint, and a dedicated sub-480px breakpoint for small phones
- JavaScript-driven collapsible navigation on mobile

## Pages
| Page | File | Purpose |
|---|---|---|
| Home | `Index.html` | Landing page, hero, 4 featured products |
| About | `About.html` | Mission, core pillars, call to action |
| Products | `Products.html` | Full 15-item catalogue with search/filter |
| Enquiry | `Enquiry.html` | Business enquiry form |
| Contact | `Contact.html` | Durban & Cape Town hubs, each with its own map, contact form |

## Tech Stack
- **HTML5** — semantic markup
- **CSS3** — custom properties, Flexbox, Grid, three-tier media queries (480px / 768px)
- **JavaScript (vanilla)** — DOM events, `data-category` filtering, form validation, mobile nav toggle
- **Git & GitHub** — version control, hosted on **GitHub Pages**

## Project Structure
agridirect/
├── Index.html
├── About.html
├── Products.html
├── Enquiry.html
├── Contact.html
├── CSS/
│ └── style.css
├── JS/
│ └── script.js
└── images/
├── tomatoes.jpg
├── spinach.jpg
└── 13 category SVG graphics (oranges, basil, butternut, red-onions,
potatoes, bananas, apples, watermelon, avocados, coriander,
mint, rosemary, thyme)


## Getting Started
No build step required.
- Open `agridirect/Index.html` directly in a browser, **or**
- Serve the folder locally for the most accurate preview: npx serve agridirect

    or right-click `Index.html` in VS Code and choose **Open with Live Server**.

## Deployment
Hosted on **GitHub Pages**, serving from the `main` branch root, so every page under `agridirect/` is reachable at:


## Known Limitations
This is an academic prototype, not a production marketplace.
- Forms validate client-side only — no backend, so no email is actually sent; the "submitted" confirmation is a JS `alert()`, not a persisted record.
- Only the Tomatoes and Spinach listings use real photography; the other 13 products use flat SVG placeholder graphics in the site's colour palette.
- No image compression pipeline — product photos are hand-sized.

## Documentation Files
| File | Contents |
|---|---|
| [`CHANGELOG.md`](CHANGELOG.md) | Part 1–3 milestones, grouped by date |
| [`robots.txt`](robots.txt) | Crawler access rules |

## Author
Olwethu Simphiwe Mkhize, ST10493769 — Web Development (WEDE5020), IIE Rosebank College (Durban Campus)
