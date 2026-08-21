# Divyadharshni & Vishnu — Wedding Invitation Project Context

> **Purpose:** Persistent handoff/context file for ChatGPT, the owner, and collaborators. Keep this file updated whenever the website, hosting, design, assets, behavior, or sharing setup changes.

## 1. Project identity

- Project: **Divyadharshni & Vishnu — Wedding Invitation**
- Repository: `iamgokuhaaaaa-lgtm/divyadharshni-vishnu-wedding`
- Branch: `main`
- Hosting: **GitHub Pages**
- Live URL: `https://iamgokuhaaaaa-lgtm.github.io/divyadharshni-vishnu-wedding/`
- Main entry file: `index.html`
- Current date of this context update: **2026-08-21**

## 2. Current status

The invitation is live on GitHub Pages and opens successfully for the owner. The site was originally a self-contained HTML invitation and was renamed from `wedding-invitation.html` to `index.html` so GitHub Pages could serve it as the homepage.

The owner is a GitHub beginner. The intended workflow is therefore:

1. Keep the project in one simple GitHub repository.
2. Keep the public URL stable.
3. Make changes directly in the repository when possible.
4. Keep this markdown file as persistent context so future sessions can understand the project without reconstructing the history.
5. Allow the owner's friend to be added as a GitHub collaborator later so they can edit the same repository.

## 3. Design direction

The invitation uses a premium Indian wedding aesthetic with:

- Ivory / warm cream background
- Plum / deep purple typography
- Lavender accents
- Muted gold accents
- Rose/pink accents
- Elegant serif typography
- Cormorant Garamond, Playfair Display, Cinzel/Cinzel Decorative, and Alex Brush fonts
- A romantic couple portrait used as the main visual/background treatment

The existing design should be **preserved rather than replaced wholesale** unless the owner explicitly asks for a redesign.

## 4. Existing website features / decisions

The current HTML contains:

- Wedding invitation hero section
- Couple names: **Divyadharshni & Vishnu**
- Wedding date: **Sunday, 30 August 2026**
- Venue: **Kallidaikurichi**
- Google Maps/venue interaction
- Countdown / flip-clock style date countdown
- Mobile-first layout
- Single-page invitation structure
- Existing couple photograph embedded in the self-contained HTML
- Decorative wedding typography and styling

### Important previous fixes

Previous testing identified mobile rendering issues with the flip clock and contrast. Those fixes should not be casually removed when editing the site.

The project plan also identified future work such as additional photos/slideshow and further invitation sections. Those are future enhancements unless the owner explicitly changes priority.

## 5. WhatsApp sharing goal

The owner wants the invitation to be shared as **one common link** through WhatsApp, with an attractive preview card similar to Google Maps, Spotify, Amazon, etc.

The desired behavior is:

- Send only the website URL in WhatsApp.
- WhatsApp should automatically generate a rich link preview.
- Preview should use the couple image supplied by the owner.
- Preview title should be: **Divyadharshni & Vishnu — Wedding Invitation**.
- Preview description should mention the wedding invitation and date.
- Target preview dimensions: **1200 × 630**.

The intended Open Graph metadata is:

```html
<meta property="og:title" content="Divyadharshni &amp; Vishnu — Wedding Invitation">
<meta property="og:description" content="You're invited to celebrate our special day. Sunday, 30 August 2026.">
<meta property="og:type" content="website">
<meta property="og:url" content="https://iamgokuhaaaaa-lgtm.github.io/divyadharshni-vishnu-wedding/">
<meta property="og:image" content="https://iamgokuhaaaaa-lgtm.github.io/divyadharshni-vishnu-wedding/preview.jpg">
<meta property="og:image:secure_url" content="https://iamgokuhaaaaa-lgtm.github.io/divyadharshni-vishnu-wedding/preview.jpg">
<meta property="og:image:type" content="image/jpeg">
<meta property="og:image:width" content="1200">
<meta property="og:image:height" content="630">
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="Divyadharshni &amp; Vishnu — Wedding Invitation">
<meta name="twitter:description" content="You're invited to celebrate our special day.">
<meta name="twitter:image" content="https://iamgokuhaaaaa-lgtm.github.io/divyadharshni-vishnu-wedding/preview.jpg">
```

**Important:** As of this context update, the exact `preview.jpg` path has NOT been confirmed in the repository. The repository currently contains two PNG image assets uploaded by the owner, but no file named `preview.jpg`. Before finalizing the Open Graph image URL, verify the actual preview image filename/path in GitHub.

## 6. Current image assets in repository

The repository currently contains these uploaded PNG files:

- `ChatGPT Image Aug 21, 2026, 05_15_52 PM.png`
- `ChatGPT Image Aug 21, 2026, 05_27_19 PM.png`

Do not delete or rename these without checking whether they are used by the invitation.

## 7. Social preview image supplied by owner

The owner supplied a portrait couple image and asked for it to be used as the image people see when the invitation link is shared.

The requested sharing preview format is **1200 × 630**. The visual should remain elegant and recognizable at small WhatsApp preview sizes.

If a new preview image is generated or uploaded, give it a simple stable filename such as:

`preview.jpg`

or, if PNG is required:

`preview.png`

Then update the Open Graph tags to match the actual deployed filename.

## 8. Hosting / GitHub history

- GitHub repository was created for the invitation.
- GitHub Pages was enabled.
- The original file was renamed to `index.html`.
- The live public URL is stable and should remain unchanged while iterating.
- The owner has connected GitHub to ChatGPT and granted repository access.
- ChatGPT can now read and write repository text files through the GitHub connection.

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

## 11. Change log

### Initial project / v4 context

- Single self-contained HTML invitation was established.
- Main wedding visual and invitation styling were established.
- Mobile flip-clock/countdown behavior was tested and fixed.
- Mobile contrast/readability issues were identified and fixed.
- Venue/Google Maps interaction was kept compact and mobile friendly.
- Additional photo/slideshow work remained a future enhancement.

### Hosting setup

- Created GitHub repository: `iamgokuhaaaaa-lgtm/divyadharshni-vishnu-wedding`.
- Uploaded the invitation.
- Renamed `wedding-invitation.html` → `index.html`.
- GitHub Pages became the public host.
- Live URL established:
  `https://iamgokuhaaaaa-lgtm.github.io/divyadharshni-vishnu-wedding/`

### WhatsApp preview work

- Owner requested a rich WhatsApp link preview.
- Owner supplied the couple image to use as the preview visual.
- A 1200 × 630 social-preview concept was prepared.
- Open Graph/Twitter metadata was prepared conceptually and must point to the actual image file hosted in the repository.

### Context persistence

- This file was created specifically so future ChatGPT sessions and collaborators can recover the project state, decisions, pending work, and important constraints.
- Update this file after meaningful changes.

## 12. Pending next steps

1. Verify which of the uploaded PNGs is the intended 1200 × 630 WhatsApp preview, or upload/rename the final preview as `preview.jpg`.
2. Ensure `index.html` contains the final Open Graph metadata pointing to the real image path.
3. Commit the metadata update.
4. Wait for GitHub Pages to redeploy.
5. Test the URL in WhatsApp by sending it to a private/self chat.
6. If WhatsApp caches an older preview, test with a fresh URL/query only for debugging; do not change the permanent public URL unnecessarily.
7. Continue visual polish only after confirming the share preview works.

## 13. Editing rules for future work

- Preserve the existing invitation's overall visual language unless the owner requests a redesign.
- Do not remove working mobile fixes without testing the result.
- Keep the public URL stable.
- Prefer simple files and simple deployment.
- Keep important decisions in this file.
- Whenever changing a feature, append a short dated entry to the change log.
- Never assume an asset exists: verify the repository path before putting it into HTML.
- Before changing `index.html`, preserve existing functionality and test the resulting live page on mobile.
