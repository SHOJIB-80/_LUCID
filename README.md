# _LUCID

A static, single-page landing page template built with HTML, CSS and JavaScript — includes animated hero, testimonial carousel, pricing tables, contact form and visual effects (particles / ripples).

Preview: https://shojib-80.github.io/_LUCID/

---

## Overview

_LUCID_ is a lightweight, static landing page (one-page theme) intended as a ready-to-use HTML template for product or app landing pages. It demonstrates common landing page sections and client-side visual effects (particles background, ripple effects, scroll animations, carousel and counters). This repository contains the complete static site (HTML, CSS, JS and image assets).

Intended for: front-end developers, designers, or anyone who needs a simple static landing page template to customize.

---

## Features (implemented)

- Single-page landing layout (index.html) with header, hero, features, device/details, testimonials, pricing, contact, map and footer sections.
- Responsive styles (CSS files included).
- Particles background (particles.js).
- Water ripple effect (jQuery ripples) used in demo/testimonial area.
- Testimonial carousel (Owl Carousel).
- CSS / JavaScript animations (Animate.css, WOW.js and AOS).
- Animated counters (Counter-Up plugin).
- Back-to-top progress indicator (SVG progress circle + JS).
- Google Maps embed (iframe).
- Static contact form markup (no server-side endpoint).
- Included demo/third-party plugin folders (particles.js, Counter-Up, ripples).

Notes:
- Many buttons/CTAs in the template are placeholders (empty href attributes).
- Contact form has no action/handling — it is only the frontend markup.

---

## Tech stack (confirmed from repository)

- Languages: HTML5, CSS3, JavaScript (ES5)
- Frameworks / libraries:
  - Bootstrap (linked via CDN in index.html)
  - jQuery (linked via CDN)
  - Owl Carousel
  - particles.js
  - jQuery Ripples (ripples)
  - WOW.js
  - AOS (Animate On Scroll)
  - Counter-Up (jQuery plugin)
  - Font Awesome (kit referenced)
- Assets: images included in `/images`
- No build tools, package manager files (npm / yarn / package.json) or backend code present — this is a static site.

---

## Project structure

Top-level (important files and folders):

```
_LUCID/
├─ index.html                 # Main landing page
├─ css/
│  ├─ style.css
│  ├─ media.css
│  ├─ animate.css
│  ├─ owl.carousel.min.css
│  └─ owl.theme.default.min.css
├─ js/
│  ├─ particles.min.js
│  ├─ particle.js
│  ├─ jquery.ripples.js / jquery.ripples-min.js
│  ├─ owl.carousel.min.js
│  ├─ wow.min.js
│  ├─ jquery.counterup.min.js
│  └─ scroll-up-bar.js
├─ images/                    # Visual assets used by the template
├─ Counter-Up-master/         # Included third-party plugin (contains its own LICENSE)
├─ jQuery-Plugin-For-Water-Ripple-Animation-ripples/  # ripples demo and files
├─ particles.js-master/       # particles demo files
└─ README.md
```

Purpose of notable files:
- index.html — the complete template to open or serve.
- css/style.css — main site styles.
- js/* — client-side scripts for effects, carousel, counters etc.
- images/ — images used in hero, clients, banners and icons.
- Counter-Up-master/ and particles.js-master/ — third-party plugin source/demo folders included in repo.

---

## Requirements / Prerequisites

- Any modern web browser (Chrome, Firefox, Edge, Safari).
- No build step required.
- Recommended (for local preview): Python 3 (for a simple HTTP server) or Node.js `live-server` (optional).

Confirmed external CDN dependencies (loaded in index.html):
- Bootstrap CSS / JS (CDN)
- jQuery (CDN)
- Font Awesome kit
- AOS (CDN)
- Waypoints (CDN)

---

## Installation / Local preview

You can preview the site simply by opening index.html in a browser, or serve it locally to avoid cross-origin issues with some plugins.

1. Clone the repository:
   - git clone https://github.com/SHOJIB-80/_LUCID.git
   - cd _LUCID

2. Quick preview (open file)
   - Open index.html in your browser (double-click or use your editor's Live Preview).

3. Recommended: run a local static server

- Python 3:
  - python -m http.server 8000
  - Open http://localhost:8000 in your browser

- Node (if you have `live-server`):
  - npx live-server .        # or live-server if installed globally

This will ensure features such as particles or plugins that rely on HTTP work as expected.

---

## Configuration

- No environment variables or server configuration are required — this is a static template.
- The contact form in index.html uses a plain `<form action="">` and therefore does not submit to a server. To make it functional, integrate it with a backend endpoint or a form service and update the form `action` attribute and method.
- Font Awesome is referenced via a kit token in index.html. Replace the kit token or include Font Awesome another way if necessary.
- If you use any included third-party libraries in production, review their licenses (Counter-Up includes a LICENSE file inside its folder).

TODO:
- Add a root-level LICENSE for this repository (none was found).
- Replace placeholder CTA links and contact form action with real endpoints if needed.

---

## Running / Usage

- After cloning and serving the project (see above), use the site as a static landing page template.
- Edit content directly in index.html to customize text, images and links.
- Modify styles in css/style.css and responsive rules in css/media.css.
- Replace or remove third-party assets in `js/` and `css/` as desired.

Important usage notes:
- Buttons such as "Download Now" and "View Features" in the template are placeholders (empty href) and need to be wired to real destinations.
- The Google Maps iframe is embedded with a public URL inside index.html — update it if you want a different location.

---

## API / Database

- This project contains no server-side API or database. All functionality is client-side only.

---

## Testing

- No automated tests or test framework are included in this repository.

---

## Deployment

- This is a static site. You can deploy it with any static hosting solution:
  - GitHub Pages (repository root as source) — the README header includes a preview URL: https://shojib-80.github.io/_LUCID/
  - Netlify / Vercel / Surge / S3 + CloudFront etc.

If using GitHub Pages, set the repository Pages source to the main branch (root) in repository Settings -> Pages.

---

## Security

- No backend is included. Sensitive operations (forms, API keys) are not implemented.
- Font Awesome kit token appears in index.html — if that is a private kit token, consider moving to a safer configuration. (If this is a public demo kit, no action required.)
- Review and comply with third-party licenses for included libraries before commercial use.

---

## Known limitations

- Contact form is non-functional (no server endpoint).
- Several CTA links are placeholders (empty href values).
- No package.json / build pipeline — everything is manual/static.
- No root LICENSE was found for the repository (Counter-Up subfolder contains its own license).

---

## Contributing

Contributions are welcome. A simple workflow:

1. Fork the repository.
2. Create a feature branch: git checkout -b feature/my-change
3. Make changes and test locally.
4. Commit and push your branch.
5. Open a pull request with a clear description.

(There are no contribution guidelines or CODE_OF_CONDUCT files in this repo — consider adding them if you intend to accept external contributions.)

---

## License

- No repository-level license file was found. Confirm and add a LICENSE at the project root if you plan to make this project public and reusable under a specific license.
- Note: some included third-party components (e.g., Counter-Up) include their own LICENSE inside their folder — review those files before reuse.

---

## Author

- Repository owner: SHOJIB-80 (GitHub user)

---

## Acknowledgements

This template includes and integrates several third-party front-end libraries and demos:
- particles.js
- jQuery Ripples
- Owl Carousel
- WOW.js / Animate.css
- Counter-Up (Counter-Up-master folder)

Please review each project's license if you reuse their code.

---
