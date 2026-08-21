# WhatsApp / Social Preview

This folder is the single source of truth for the invitation's WhatsApp/social preview image.

## How to change the preview later

1. Keep **one** image in this folder (`.png`, `.jpg`, `.jpeg`, or `.webp`).
2. Delete the old preview image.
3. Upload the new image into this same `preview/` folder.
4. The GitHub Action will automatically find the image and update `og:image` and `twitter:image` in `index.html`.
5. Keep only one image here so there is no ambiguity.

You do **not** need to edit `index.html` when changing the preview image.

The automation is in `.github/workflows/replace-countdown.yml`.
