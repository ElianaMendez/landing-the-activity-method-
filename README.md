# The Activity Method™ — Landing Page

This repository contains the sales landing page files for The Activity Method™.

## Files Included
1. `SYSTEMEIO_LANDING.html`: The ONLY file you need for Systeme.io. **Do not use `index.html` in Systeme.io.** This file is an HTML fragment without standard document tags (`<html>`, `<head>`, `<body>`, etc.), complying with Systeme.io's "Raw HTML" element requirements.
2. `index.html`: A local preview wrapper file. 
3. `README.md`: These instructions.

## 1. How to preview locally
To preview the design in your browser, you must open `index.html` using a local web server to avoid CORS issues when fetching the fragment. 
- If using VS Code, use the **Live Server** extension.
- Alternatively, run a python local server in this directory: `python -m http.server` and navigate to `http://localhost:8000`.

## 2. Which file should be copied into Systeme.io
You must copy the ENTIRE contents of **`SYSTEMEIO_LANDING.html`**. 
Paste it into the **Raw HTML (Código HTML)** element inside your Systeme.io drag-and-drop builder.

It is confirmed that this file **DOES NOT** contain `<html>`, `<head>`, `<body>`, or `<footer>` tags. It only contains a `<style>` block and scoped HTML markup.

## 3. Where the checkout URL is defined
The checkout URL is defined on every primary Call to Action (CTA) button in the `SYSTEMEIO_LANDING.html` file. 
Search for the following URL in the file:
`https://activity-method.systeme.io/checkout`

All CTA links strictly point to this checkout URL.

## 4. Where future image URLs should be inserted
In the `SYSTEMEIO_LANDING.html` file, there are 3 clear placeholders to insert your final actual product screenshots or graphics when ready. They are marked with HTML comments:

1. `<!-- SYSTEME_IMAGE_01: PRODUCT_SELECTOR_SCREENSHOT -->`
2. `<!-- SYSTEME_IMAGE_02: THREE_MATCHES_SCREENSHOT -->`
3. `<!-- SYSTEME_IMAGE_03: ACTIVITY_DETAIL_SCREENSHOT -->`

Currently, these sections contain HTML/CSS mockups representing the product experience for presentation purposes. You can replace the `<div class="tam-mockup">...</div>` elements immediately below those comments with `<img src="..." alt="...">` tags once your visual assets are uploaded.

## Quality Control Checklist
- [x] NO "Raíces Vivas" branding, images, or copy used.
- [x] All CTA buttons link strictly to `https://activity-method.systeme.io/checkout`.
- [x] No references to 1,395 activities or fake bonuses.
- [x] Tone is professional, practical, and non-medical.
- [x] $35 one-time offer and 7-day refund policy are clearly specified.
- [x] Pure HTML/CSS (No React, Vue, npm build tools, or external UI frameworks).
- [x] No fake scarcity, count down timers, or fake testimonials.
