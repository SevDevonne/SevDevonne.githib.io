# Sev Devonne — art + development website

A zero-build, static portfolio. No image files are required: all image areas are styled CSS placeholders.

## Deploy to the existing GitHub Pages repository

1. Copy `index.html`, `shop.html`, `stylesheet.css`, and `main.js` to the **repository root**.
2. Keep any other existing pages or directories you still use; these files do not require the existing `images/` folder.
3. Preview locally by opening `index.html`, or run `python -m http.server 8000` from the repository directory.
4. Commit and push the updated site.

## Replace a placeholder with a real image

For example, replace:

```html
<div class="media-placeholder media-tall" role="img" aria-label="Artwork image placeholder for Montagu Country Hotel">...</div>
```

with:

```html
<img class="artwork-image" src="images/artworks/montagu_hotel_car_web.webp" alt="Watercolour illustration of the Montagu Country Hotel" loading="lazy">
```

and add to `stylesheet.css`:

```css
.artwork-image { width: 100%; aspect-ratio: 4 / 4.85; object-fit: cover; display: block; }
```

Use web-optimized images rather than print-resolution originals. For hero images, you can replace the `.hero-visual` placeholder with an image and retain the surrounding visual style as needed.

## Customize

- `index.html`: sections, project descriptions, and contact details.
- `shop.html`: currently an honest preview with no checkout or order buttons.
- `stylesheet.css`: colors and responsive layout (`:root` variables at the top).
- `main.js`: mobile menu and copyright year only.

**Note:** Project links intentionally point to the GitHub profile rather than guessing individual repository URLs. Update each link to its exact project repository when ready.

This site imports Google Fonts for typography; it falls back to system fonts without network access.
