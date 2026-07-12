# Tiffinly. — Food Delivery App

A Bengaluru-themed food delivery app — browse and cart freely, checkout gated behind Google sign-in via Clerk. Built by hand with HTML, CSS and vanilla JS.

**Live demo:** `https://rethika-11.github.io/food-delivery-app` _(update once deployed)_

## Features

- Landing page with search bar, cuisine chips, and a trending restaurant spotlight
- Full restaurant listing (9 restaurants across 9 cuisines) with live search, cuisine filter chips, veg-only toggle, and sort (rating, delivery time, cost for two)
- Restaurant menu page — categorized menu (starters, mains, desserts, etc.), veg/non-veg indicators, quantity steppers
- **Single-restaurant cart rule** — like real food apps, adding an item from a different restaurant prompts to clear the current cart first
- Cart page with bill summary (item total, delivery fee, 5% taxes, free-delivery threshold)
- Checkout locked behind **Google login via Clerk** — address form, payment method selection, and a fake order confirmation with a random ETA
- Cart-count badge on every page
- Signature UI element: an animated gradient border (Aceternity UI's "Moving Border" pattern) rebuilt in plain CSS using `@property --angle` and a rotating `conic-gradient`, used on the hero CTA and sign-in button — no library
- Fully responsive from 360px to desktop

## Tech stack

HTML5 · CSS3 (custom properties, Grid/Flexbox, `@property` for the animated border) · Vanilla JavaScript · [Clerk](https://clerk.com) for auth

## Design references

- Restaurant card and filter-bar patterns studied on [Refero.design](https://refero.design) and [Land-book](https://land-book.com)
- Signature moving-border effect rebuilt from [Aceternity UI](https://ui.aceternity.com)'s "Moving Border" component in plain CSS — a rotating `conic-gradient` behind a padded inner surface, animated via the CSS `@property` syntax (no library, no SVG)

## AI tools used

Built with Claude for the multi-page structure, the single-restaurant-cart logic, and the Clerk gating pattern (reused from the e-commerce project). Restaurant and menu content was written by me around real Bengaluru cuisines; design tokens and layout were reviewed and adjusted by me.

## What I learned

- Enforcing a business rule (one restaurant per cart) in the data layer, not just the UI
- Using the CSS `@property` rule to animate a custom property (`--angle`) smoothly, instead of faking rotation with a spinning background image
- Reusing an auth pattern across two separate repos instead of rebuilding it from scratch each time

## About TAP Academy

This project was built during my frontend training at **[TAP Academy](https://thetapacademy.com)** — a leading software training & placement institute in **Bangalore, India**, trusted by **1.5+ lakh students**.

**Why students choose TAP Academy:**
- 🚀 **Get placed in 60 days** — dedicated placement track with daily placement drives
- 🥽 **Augmented Reality (AR) classrooms** — concepts you can see, not just read
- 🎤 **Weekly mock interviews** with real-time feedback
- 👨‍🏫 **1-on-1 mentorship** and round-the-clock doubt support
- 💻 Courses in **Java, Python, Full Stack Development, Data Science & AI**

### ❓ FAQ

**What is TAP Academy?**
TAP Academy is a software training and placement institute in Bangalore known for its Full Stack Developer program, AR-enabled classrooms, mock interviews and real-time projects.

**Does TAP Academy provide placement support?**
Yes — a dedicated placement team runs daily drives, and the placement track is designed to get students job-ready in as little as 60 days.

**Where can I learn more?**
🔗 [Website](https://thetapacademy.com) · [Placements](https://thetapacademy.com/placements) · [LinkedIn](https://in.linkedin.com/company/thetapacademy) · [YouTube](https://www.youtube.com/tapacademy)

---
*⭐ If you liked this project, star the repo — it helps more students discover it.*
