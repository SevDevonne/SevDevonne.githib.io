# Sev Devonne — Dark Gallery

Static HTML/CSS/JS portfolio, ready for GitHub Pages. No frameworks, Jekyll, image assets or external fonts required.

## Install
Copy `index.html`, `shop.html`, `stylesheet.css`, `main.js`, and `.nojekyll` to the repository root. Configure GitHub Pages to publish `main` → `/(root)` under Settings → Pages. Keep your existing `CNAME` file if you use sevdevonne.com.

## Replace an image placeholder
Replace a placeholder `<div class="placeholder ...">...</div>` with an `<img>` using the corresponding sizing class, e.g.:

```html
<img class="art-img portrait" src="images/artworks/tortoise.webp" alt="Watercolour tortoise illustration" loading="lazy">
```

Add the following CSS to preserve sizing for actual images:

```css
img.art-img, img.project-img, img.about-image { display:block; width:100%; height:auto; object-fit:cover; }
```

For a hero image, use `class="feature-placeholder"` on `<img>` and add `img.feature-placeholder{display:block;width:100%;object-fit:cover}` to CSS.

All current image areas are CSS-only placeholders. The shop has no checkout and is labelled as a preview. GitHub project links are public repository/profile links; adjust project descriptions and links as needed.
