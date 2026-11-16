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

1. Push this folder to a new GitHub repo (the files sit at the repo root).
2. In Vercel: **Add New → Project**, import the repo.
3. Framework preset: **Other**. Leave build command and output directory empty.
4. Deploy. Every push to the repo updates the preview.

The pages are set to `noindex`, so search engines won't list the preview.

## Run locally

Open `index.html` through any static server, for example:

```
npx serve .
```
