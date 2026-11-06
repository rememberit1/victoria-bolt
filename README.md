# Victoria (Bolt variant)

## Overview

Same **Victoria** coming-soon book microsite as `victoria-site`, packaged in a lighter “Bolt” layout: photos are embedded as base64 in `photos.js` instead of separate image files under `assets/`.

## Purpose

Drop-in single-folder variant of the Victoria storytelling page for hosts or builders that prefer inlined assets (fewer files to upload).

## Features

Identical UX to `victoria-site`:

- 3D heart WebGL background
- Flip-book hero, iMessage mock, gallery, reviews, debt gag, notify CTA
- GSAP scroll animations

Differences:

- `photos.js` supplies `window.VPHOTOS` data-URLs
- No separate photo assets directory or vendored Three/GSAP copies in this slim tree (script tags / imports follow this variant’s `index.html` / `main.js`)

## Tech stack

- Static HTML/CSS/JS + Three.js / GSAP (as referenced by this variant)
- Inlined JPEG data-URLs for photos

## Run / deploy

```bash
python3 -m http.server 8080
# open http://localhost:8080/
```

Static host only. Prefer `victoria-site` if you want discrete asset files and the fuller vendor/shot folders.

## Notes

Creative joke site; not a commercial product page.
