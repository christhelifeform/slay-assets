# slay-assets

**Public image host for Slay Global brands.** Nothing here is private, and nothing private goes here.

Images are served to email clients over `raw.githubusercontent.com`, which is stable, unauthenticated
and not rate-limited for this volume. ⛔ **Google Drive and Google Photos were considered and rejected**
— both rewrite URLs and throttle hotlinking, which silently breaks images in already-delivered email.

## Why this exists

Brevo's image gallery ingests from a **public URL only** — it will not accept an upload — and every
other Slay Global repo is private. Email needs a stable public origin for every image it references,
**for as long as the email exists in someone's inbox.**

## Rules

- ⛔ **Finished, public-facing brand assets only.** No drafts, no client work, no data, no screenshots
  of anything internal.
- **Never delete or rename a file that has shipped in an email.** A delivered email keeps pointing at
  that URL forever, and a 404 is a broken image in an archive nobody can fix.
- ⭐ **TRANSPARENT CUTOUTS ARE THE BRAND LOOK** (Chris, 2026-08-16). Product shots keep their alpha.
- ⛔ **Flatten ONLY when the artwork is near-black or near-white.** A solid-black logo on transparent
  **disappears in dark mode**; a mid-tone silver printer reads fine on both white and dark. **The test
  is the artwork's own value, not a blanket rule.**
- ⚠️ **Never overwrite a file in place — add a new name.** `raw.githubusercontent.com` sits behind a
  CDN cache, so an overwrite can keep serving the old bytes for a while with no way to tell.
- Size for retina: export at 2x the display width.

## Contents

| File | Use |
|---|---|
| `hardwire/hardwire-masthead-600.png` | HARDWIRE masthead. 600x104, displays at 300px |
| `hardwire/a1-mini-cutout-560.png` | Bambu Lab A1 mini, giveaway prize. 560px, **transparent cutout** |
