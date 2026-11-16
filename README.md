# Yoga Tribe · Black Friday landing page previews

Static preview of the three current designs for the 4-Week Mobility Reset Black Friday page:

- **V6 · Black Friday Issue** (`/v6/mobile.html`, `/v6/desktop.html`)
- **V4 · The Black Friday Pass** (`/v4/...`)
- **V3 · New Fonts** (`/v3/...`)

Open `index.html` to switch designs with the tabs and flip between Mobile and Desktop.
Links can point straight at a view, e.g. `/#v4/desktop`.

These are design previews only. The real page gets built in Wix. Videos stream from Cloudinary;
photo slots are still labelled placeholders.

## Deploy on Vercel

The repo is a plain static site with no build step. `vercel.json` already tells Vercel to use the
**Other** preset, with no install or build command and the repo root as the output directory.

1. In Vercel: **Add New → Project**, then import `Amplihub/yoga-tribe`.
2. Leave every setting at its default and click **Deploy**.
3. Every push to `main` updates the preview, and other branches get their own preview URLs.

The `v3/`, `v4/` and `v6/` folders must be in the repo next to `index.html`, because the
preview loads them in iframes.

The pages are set to `noindex`, so search engines won't list the preview.

## Run locally

Open `index.html` through any static server, for example:

```
npx serve .
```
