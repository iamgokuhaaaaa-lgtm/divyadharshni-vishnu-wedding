# Divyadharshni & Vishnu — Wedding Invitation Project Context

> **Purpose:** Persistent handoff/context file for ChatGPT, the owner, and collaborators. Keep this file updated whenever the website, hosting, design, assets, behavior, or sharing setup changes.

## 1. Project identity

- Project: **Divyadharshni & Vishnu — Wedding Invitation**
- Repository: `iamgokuhaaaaa-lgtm/divyadharshni-vishnu-wedding`
- Branch: `main`
- Hosting: **GitHub Pages**
- Live URL: `https://iamgokuhaaaaa-lgtm.github.io/divyadharshni-vishnu-wedding/`
- Main entry file: `index.html`

## 2. Current status

The invitation is live on GitHub Pages. The project is intentionally kept simple because the owner is a GitHub beginner.

Current working setup:

1. `index.html` is the live invitation.
2. GitHub Pages hosts the site at the stable public URL above.
3. `preview/DSC04255.JPG` is the currently selected WhatsApp/social preview image.
4. Background portrait lives in `background/` (active file: `background/background.jpg`).
5. Main couple photo lives in `photos/` (active file: `photos/couple.jpg`).
6. Background wash / panel blur strength is controlled by CSS variables at the top of `index.html` (`:root`).
7. `PROJECT_CONTEXT.md` is the persistent project memory and must be updated after meaningful changes.
8. GitHub Actions automation that was previously attempted and failed has been removed. Do not reintroduce automation unless explicitly requested.

## 3. Design direction

The invitation uses a premium Indian wedding aesthetic with:

- Ivory / warm cream background
- Plum / deep purple typography
- Lavender accents
- Muted gold accents
- Rose/pink accents
- Elegant serif and script typography
- Romantic couple portrait as the main visual

The existing design should be **preserved rather than replaced wholesale** unless the owner explicitly asks for a redesign.

## 4. Current invitation features / decisions

The current HTML contains:

- Wedding invitation hero section
- Couple names: **Divyadharshni & Vishnu**
- Wedding date: **Sunday, 30 August 2026**
- Venue: **Kallidaikurichi / Town Panchayat Marriage Hall**
- Google Maps/venue interaction
- Mobile-first layout
- Single-page invitation structure
- Couple photograph loaded from `photos/couple.jpg` (not embedded in the HTML)
- Background portrait loaded from `background/background.jpg` (not embedded in the HTML)
- Decorative wedding typography and styling

### Latest design changes deployed to `index.html`

The owner supplied one exact reference invitation image and explicitly said to use **that image only as the reference** for the requested visual treatment. No other generated artwork should be substituted.

Latest requested/deployed changes:

- Use the **Vinayakar/Ganesha artwork from the supplied reference image** as the top Vinayakar treatment.
- Remove the duplicate golden/orange date/muhurtham box.
- Keep one wedding date presentation and make the date static.
- Countdown is simplified to **DAYS · HOURS · MINUTES** only.
- Days, hours, and minutes are large and arranged together on one line where the viewport allows, with responsive behavior on small screens.
- Only the countdown values should pulse/update; the surrounding countdown container should remain still.
- **The heart is intentionally left alone** and should not be redesigned or replaced.
- Preserve the rest of the invitation and existing functionality.

The owner confirmed the edited `index.html` was manually replaced in GitHub after the updated file was prepared.

### Background translucency / blur knobs (22 August 2026)

There was no single variable before. The cream wash over the background photo and the frosted card blur are now adjustable in `index.html` inside `:root`.

Tweak these and refresh the page to compare looks:

- `--bg-veil` — main control for how milky the background photo is. `0` = photo fully visible, `1` = the previous look, higher than `1` = heavier cream wash.
- `--bg-veil-top`, `--bg-veil-mid`, `--bg-veil-deep`, `--bg-veil-bottom` — optional finer control of the gradient stops.
- `--panel-opacity` — how solid the frosted invitation cards are (was `0.62`).
- `--panel-blur` — blur amount on those cards (was `7px`).
- `--bg-photo-position` and `--bg-photo-saturate` — crop/saturation of the background photo.

Do not hunt through the rest of the CSS for overlay numbers; change `:root` only.

### Photo folders (22 August 2026)

The owner asked for separate folders so favorite photos can be uploaded and tried without rewriting the invitation layout.

- Background portrait folder: `background/`
- Active background file: `background/background.jpg`
- Main couple photo folder: `photos/`
- Active couple photo file: `photos/couple.jpg`

Two supported workflows:

1. **Same filename:** delete the old `background.jpg` or `couple.jpg`, upload a new image with that exact name. No `index.html` change needed (keep `.jpg` casing).
2. **Many favorites:** keep extra files in the same folder (`background/photo-a.jpg`, `photos/garden.jpg`, etc.) and change only the filename in `index.html`:
   - background: `--bg-photo: url("background/YOUR-FILE.jpg");`
   - couple photo: `<img src="photos/YOUR-FILE.jpg" ...>`

Vinayakar/Ganesha artwork remains embedded in `index.html` and should still not be substituted.

WhatsApp preview is still independent and remains `preview/DSC04255.JPG`.

## 5. WhatsApp sharing / preview

The owner wants the invitation shared as one stable link through WhatsApp with a rich preview card containing image, title, and description.

This is currently working.

Current preview image:

`preview/DSC04255.JPG`

Current public image URL:

`https://iamgokuhaaaaa-lgtm.github.io/divyadharshni-vishnu-wedding/preview/DSC04255.JPG`

The owner successfully tested that WhatsApp displays the image + title + description preview.

### Preview folder convention

The owner wants a dedicated `preview/` folder so preview images can be experimented with independently of the main invitation.

Current file:

`preview/DSC04255.JPG`

For future experiments, the safest simple workflow is:

1. Keep the active preview at the stable filename/path `preview/DSC04255.JPG`.
2. Delete the old image when replacing it.
3. Upload the new image using the same filename `DSC04255.JPG`.
4. Do not rename the extension or change case (`.JPG` vs `.jpg`) unless the HTML is also updated.
5. Avoid making the HTML dynamically guess which image is inside the folder; GitHub Pages is static, so a fixed filename is more reliable.

WhatsApp may cache an older preview. A website image changing does not guarantee instant refresh of a preview already cached by WhatsApp.

## 6. Open Graph / social metadata

The desired metadata remains:

- Title: **Divyadharshni & Vishnu — Wedding Invitation**
- Description: invitation/wedding date text
- Type: website
- URL: stable GitHub Pages URL
- Image: current `preview/DSC04255.JPG`
- Image target: approximately 1200 × 630 for social sharing
- Twitter card: `summary_large_image`

Important: the active preview path is now `preview/DSC04255.JPG`, not the older `preview.jpg` proposal.

## 7. Image/reference rules

The owner supplied a specific reference image showing the complete invitation artwork, including:

- the Vinayakar/Ganesha line-art treatment
- lavender/purple floral decoration
- cream/plum/gold wedding palette
- couple portrait treatment
- elegant typography
- countdown styling
- date/muhurtham styling

The owner explicitly said: **“this image is good enough dont use anything else.”**

Therefore, when refining the Vinayakar or visual direction, use only that supplied reference image as the design reference. Do not substitute another generated Vinayakar or unrelated artwork.

The owner also explicitly requested that the **heart be left alone** in the latest countdown redesign.

## 8. Hosting / GitHub history

- GitHub repository was created for the invitation.
- GitHub Pages was enabled.
- The original file was renamed to `index.html`.
- GitHub Pages became the public host.
- Live URL established:
  `https://iamgokuhaaaaa-lgtm.github.io/divyadharshni-vishnu-wedding/`
- The owner has connected GitHub to ChatGPT and granted repository access.
- ChatGPT can read and write repository text files through the GitHub connection.

## 9. Collaboration goal

The owner wants a friend to be able to help edit the invitation.

Preferred setup:

- Add friend as a collaborator on this repository.
- Friend can edit/commit changes.
- GitHub Pages automatically republishes the same URL.
- Do not create separate websites for different collaborators.

The friend does not need access to the owner's ChatGPT account.

## 10. Owner's GitHub skill level

The owner is a **GitHub beginner**. Instructions should therefore be extremely simple and click-by-click. Avoid unnecessary Git commands, branches, terminal commands, or complex Git concepts unless they become necessary.

## 11. Automation history

A GitHub Actions approach was previously attempted to automate countdown/preview changes. It produced failed jobs and was ultimately cleaned up.

The failed workflow files were removed. The project should currently remain simple and should **not rely on GitHub Actions** for routine preview or invitation edits.

## 12. Change log

### Hosting setup

- Created GitHub repository: `iamgokuhaaaaa-lgtm/divyadharshni-vishnu-wedding`.
- Uploaded the invitation.
- Renamed `wedding-invitation.html` → `index.html`.
- GitHub Pages became the public host.
- Live URL established and kept stable.

### WhatsApp preview work

- Owner requested a rich WhatsApp link preview.
- Owner supplied the couple image to use as the preview visual.
- A 1200 × 630 social-preview concept was prepared.
- Open Graph/Twitter metadata was added and successfully tested in WhatsApp.
- The active preview is now `preview/DSC04255.JPG`.
- Owner confirmed that WhatsApp displays the preview image, title, and description successfully.

### Countdown redesign

- The original flip-clock countdown was abandoned because it was unreliable/stuck.
- Countdown was redesigned to show **days, hours, and minutes only**.
- Days, hours, and minutes are large and grouped together.
- Countdown values are intended to remain visibly alive through subtle pulsing/updating.
- Static wedding date remains separate from the countdown.
- The duplicate golden/orange date/muhurtham card was removed.
- The heart was explicitly left unchanged.

### Vinayakar/reference redesign

- Owner supplied an exact reference image and requested that it be the sole visual reference.
- Vinayakar/Ganesha treatment was changed to use the supplied reference artwork as the basis for the top treatment.
- Do not substitute unrelated/generated Vinayakar artwork in future edits.

### Repository cleanup

- Failed GitHub Actions workflows from the experimental automation approach were removed.
- Routine edits should now be made directly and deliberately rather than through broken automation.

### 22 August 2026 — Background translucency variables

- The background cream wash and frosted-card blur had hardcoded RGBA/blur values and no knob to retune them.
- Added `:root` variables: `--bg-veil` (main), `--bg-veil-top/mid/deep/bottom`, `--panel-opacity`, `--panel-blur`, plus `--bg-photo-position` and `--bg-photo-saturate`.
- Default values match the previous look (`--bg-veil: 1`, panel opacity `0.62`, blur `7px`).

### 22 August 2026 — Separate photo folders

- Extracted the embedded background portrait to `background/background.jpg`.
- Extracted the embedded couple photograph to `photos/couple.jpg`.
- `index.html` now points at those files by name so the owner can replace a file in-place or keep several favorites and change only the filename.
- Vinayakar artwork and WhatsApp `preview/` image were left as they were.
- `index.html` is much smaller now that those two photographs are no longer inline.

### Context persistence

- This file exists specifically so future ChatGPT sessions and collaborators can recover project state, decisions, pending work, and important constraints.
- Update this file after every meaningful design, hosting, preview, or behavior change.

### 22 August 2026 — Top-level image variables (editable)

- A small script was added to `index.html` that exposes three top-level JavaScript variables making image filenames easy to change without hunting through the markup or CSS:
  - `IMG_DIR` — directory prefixes (`preview/`, `background/`, `photos/`).
  - `IMG_FILE` — filenames for the active images (e.g. `preview: 'DSC04255.JPG'`, `background: 'background.jpg'`, `couple: 'couple.jpg'`).
  - `IMAGE_PATHS` — derived full paths (`preview`, `background`, `couple`) built from the two objects above.

- What the script does:
  - Sets the CSS variable `--bg-photo` to `url("background/<filename>")` so the background can be changed by editing `IMG_FILE.background`.
  - Updates the Open Graph (`meta[property="og:image"]`) and Twitter (`meta[name="twitter:image"]`) `content` to the `preview` image path so social previews reflect the chosen file.
  - Updates the couple photo `<img>` `src` to the `photos/` image path.

- How to change an image quickly:
  1. Open `index.html` and find the `IMG_FILE` object near the top of the file.
  2. Change only the filename value for `preview`, `background`, or `couple` (for example, replace `'couple.jpg'` with `'garden.jpg'`).
  3. Save and refresh the site. (Because GitHub Pages is static, commit & push to the repository to publish changes.)

- Notes and best practices:
  - Keep the directory names as-is (`preview/`, `background/`, `photos/`) unless you also update the `IMG_DIR` object.
  - Use the exact filename and extension case (`.JPG` vs `.jpg`) you uploaded to the repo.
  - The script runs on page load and will update meta tags/`--bg-photo` dynamically for testing; however, for production sharing (social preview caches), replace the preview file at the same path or use the same filename when updating the preview image to reduce caching issues.
  - The CSS `:root` variables for veil/blur remain the canonical place for visual tuning; do not mix image filename edits with veil/blur changes.

## 13. Pending / future work

1. Continue visual polish only when the owner requests it.
2. Potential future enhancement: additional photos/slideshow.
3. Potential future enhancement: further invitation sections.
4. If changing the WhatsApp preview, replace `preview/DSC04255.JPG` with another image using the same exact filename/path.
5. If changing `index.html`, preserve the current working WhatsApp metadata, mobile behavior, countdown behavior, and the `photos/` + `background/` file references.
6. To try a different background or couple photo, add the file to the matching folder and either reuse the active filename or change only that filename in `index.html`.

## 14. Editing rules for future work

- Preserve the existing invitation's overall visual language unless the owner requests a redesign.
- Use the owner's supplied reference image as the sole visual reference for the current Vinayakar/design treatment.
- Do not change the heart unless explicitly requested.
- Do not remove working mobile fixes without testing the result.
- Keep the public URL stable.
- Prefer simple files and simple deployment.
- Keep important decisions in this file.
- Whenever changing a feature, append a short dated entry to the change log.
- Never assume an asset exists: verify the repository path before putting it into HTML.
- Couple and background photos must live in `photos/` and `background/` respectively; do not re-embed those photographs as base64 in `index.html`.
- Before changing `index.html`, preserve existing functionality and test the resulting live page on mobile.
- Do not reintroduce the failed GitHub Actions automation unless the owner explicitly asks for automation.
