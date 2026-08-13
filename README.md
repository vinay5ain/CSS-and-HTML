# Portfolio — HTML & CSS Template

A clean, responsive static portfolio template built with plain HTML and CSS. Intended as a beginner-friendly personal website/portfolio demonstrating layout, responsive design, and asset organization.

## Overview
This repository contains a single-page static portfolio website (index.html) with accompanying CSS and image assets. It was built as a learning project to practice HTML structure, CSS layout (Flexbox, CSS variables, simple grid), and responsive design. The site includes sections commonly found on personal portfolios: hero, about, services, works, blog, reviews, contact and a downloadable CV.

## Features
- Responsive single-page portfolio layout (desktop and mobile styles).
- Sections: Header / Hero, About, Services (placeholder content), Works, Blog (static), Reviews (markup for a slider), Contact (static form markup).
- Downloadable resume (VINAY_MAIN_RESUME.pdf) linked from the header and hero.
- Organized asset folder at repository root (images and icons are included).
- Lightweight CSS-only implementation (no build tools required).

## Tech Stack
- Frontend: HTML, CSS
- Fonts: Google Fonts (Poppins, Lato)
- Libraries (CSS only): slick-carousel CSS is linked in the HTML but no JS is provided in this repo
- Tools: Any static web server or GitHub Pages can serve the site

## How it works
- index.html is a static document that references style.css and utilities.css for styling.
- The site layout uses CSS variables, Flexbox and a small responsive media query to adapt to smaller screens.
- The contact form and review slider are present as HTML markup only; there is no backend or client-side JavaScript to handle submissions or activate the slider.

## Architecture
This is a static site (no backend). Runtime shape:
- Client (browser) loads index.html -> CSS files -> assets (images, fonts)
- All behavior is presentational; no JavaScript or server-side code is required to view the site

## Project structure
Important files and folders at repository root:

- index.html            — main page (entry point)
- style.css             — main stylesheet (imports utilities.css)
- utilities.css         — small set of utility/flex/button classes
- VINAY_MAIN_RESUME.pdf — PDF resume linked from the site
- images / icons        — several PNG/JPG/SVG files used by the site (stored at repo root)

Files not listed above are primarily image assets used by the template.

## Installation / Preview locally
Clone the repository and open the site locally. No build steps or package manager is required.

Commands:

git clone https://github.com/vinay5ain/CSS-and-HTML.git
cd CSS-and-HTML

# open directly in browser (file://) or run a simple static server
# Python 3 built-in HTTP server (recommended for testing relative links):
python -m http.server 8000
# then open http://localhost:8000 in your browser

Or use the Live Server extension in VS Code to preview the page.

## Environment variables
This project is a static front-end. There are no required environment variables.

## API documentation
There are no APIs or backend endpoints in this repository. The contact form in index.html is static (no action attribute). To enable form submission you would need to add a backend endpoint or form service.

## Screenshots / Demo
No deployment URL is included in the repository. Use the local preview instructions above to view the site. Screenshots and image assets used by the page are included in the repository (e.g., `vinaay.jpg`, `ph-1.png`, `article-ph-1.png`).

## Challenges & Learning
This project demonstrates:
- HTML semantic structure for a single-page portfolio
- CSS layout with Flexbox, CSS variables, media queries and simple grid
- Organizing static assets and linking downloadable files (resume.pdf)
- Designing responsive components without frameworks — useful practice for front-end fundamentals

## Future improvements (realistic)
- Add JavaScript to enable the client slider (slick-carousel requires the JS file) and enhance interactivity
- Activate and validate the contact form by adding a backend endpoint (Node/Express or serverless form service)
- Improve accessibility (semantic landmarks, ARIA attributes, form labels)
- Add unit/end-to-end tests for build pipeline if a build step is introduced
- Move images into an `/assets` or `/images` directory for clearer structure
- Deploy to GitHub Pages and add a demo URL

## What this project demonstrates
- Foundational front-end skills: responsive HTML/CSS, layout, and asset management
- Attention to visual design and prototype-style portfolio structure
- Ability to organize a small project for quick previews and demonstrations

## Author
Vinay Kumar Sain — GitHub: @vinay5ain
