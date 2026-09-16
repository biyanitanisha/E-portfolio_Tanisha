# Tanisha Biyani — Geoinformatics Portfolio

A e-portfolio built with plain HTML, CSS, and a little JavaScript, hosted on GitHub Pages.

**Live site:** `https://biyanitanisha.github.io/<repo-name>/` — replace `<repo-name>` with this repository's actual name once published.

## Overview

This site introduces my work as an M.Sc. Geoinformatics student, covering:

- **Hero** — background video, name, and a one-line intro
- **About & education** — academic background and timeline
- **Skills & tools** — software, programming, analysis, and field data collection
- **Projects** — tabbed by category (Dashboards & Web GIS / Remote Sensing & Mapping), each card linking to the live project
- **Field research & surveys** — an interactive satellite map pinpointing field sites (Pashan Lake, Mayureshwar Supe, Mulshi), plus a socio-economic survey write-up
- **Contact** — email, GitHub, and LinkedIn

## Tech stack

- HTML5 / CSS3 (no build step, no frameworks)
- [Leaflet.js](https://leafletjs.com/) for the interactive field-work map
- Esri World Imagery tiles for the satellite basemap
- Google Fonts: Space Grotesk, IBM Plex Sans, IBM Plex Mono

## File structure

```
.
├── index.html      # entire site — markup, styles, and scripts in one file
├── profile.jpeg    # profile photo shown in the About section
└── README.md
```

## Adding project images

A few project cards currently show a small dashed **ADD IMAGE** placeholder because no screenshot was available yet. To add one:

1. Drop the image file into this repo (root, or a folder like `images/`).
2. In `index.html`, find the card's `<div class="placeholder-slot">ADD IMAGE</div>` and replace it with:
   ```html
   <img src="your-image-file.jpg" alt="Short description of the project">
   ```

## Updating content

Everything lives in `index.html`:
- Project cards are grouped under `<div class="tabpanel" id="tab-dash">` (Dashboards & Web GIS) and `id="tab-rs">` (Remote Sensing & Mapping).
- Field site coordinates are set in the `locations` object near the bottom of the file.
- Skills are listed under `<div class="skills-grid">`.

## Deploying updates

Push changes to the `main` branch (or whichever branch GitHub Pages is configured to serve) — the live site updates automatically within a minute or two.

## Contact

- Email: biyanitanisha9@gmail.com
- GitHub: [github.com/biyanitanisha](https://github.com/biyanitanisha)
- LinkedIn: [linkedin.com/in/tanisha-biyani](https://www.linkedin.com/in/tanisha-biyani-782a16312)
