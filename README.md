# Photo Privacy Cleaner

See the hidden metadata in your photos - GPS location, camera, timestamps - and
strip it before you share. 100% local: your photo never leaves your browser.

Live website: https://photo-privacy-cleaner-weld.vercel.app

## What it does

- Drop, paste, or choose photos (JPEG, PNG, WebP; HEIC metadata is view-only; multiple at once)
- See what each photo reveals: GPS coordinates, device, date and time, and more
- Strip all metadata losslessly - image quality is untouched, byte for byte
- Download cleaned copies one by one or all together as a .zip
- Zero dependencies, no uploads, no accounts, no tracking

## Why it matters

Phone cameras embed EXIF metadata in every photo, often including the exact GPS
location where it was taken. Anyone who downloads the original file can read it.
This tool shows you that hidden data and removes it before you share the photo.

## Run locally

```bash
npm ci
npm run dev
```

Tests: `npm test` - Build the static site: `npm run build:web` (outputs to `docs/`)

## Tech

TypeScript + Vite, fully client-side. No backend, no cookies, no analytics.

## Credits

Adapted from scrubpix by didrod205,
licensed under the MIT License (see LICENSE and NOTICE.txt).

## Visual design

A black, warm-white and yellow editorial interface with self-hosted Caveat handwriting, a custom photo illustration, responsive upload workspace, accessible focus states and mobile layouts. The original metadata parsing and lossless cleaning engine is unchanged. Fonts make no external requests.

Caveat by the Caveat project authors is included under the SIL Open Font License. See FONT-LICENSE.txt.
