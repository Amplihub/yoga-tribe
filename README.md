# Yoga Tribe · Black Friday landing page

Static build of the V3 design for the 4-Week Mobility Reset Black Friday page.

- `index.html` is the desktop layout, served at the site root.
- `mobile.html` is the mobile layout.

A one-line script at the top of each page picks the right layout: screens narrower than 768px
go to `mobile.html`, and wider screens go to `/`. Old preview links (`/v3/...`, `/v4/...`,
`/v6/...`) redirect to the right page through `vercel.json`.

This is a design preview only. The real page gets built in Wix. Videos stream from Cloudinary;
photo slots are still labelled placeholders.

## Deploy on Vercel

The repo is a plain static site with no build step. `vercel.json` already tells Vercel to use the
**Other** preset, with no install or build command and the repo root as the output directory.

1. In Vercel: **Add New → Project**, then import `Amplihub/yoga-tribe`.
2. Leave every setting at its default and click **Deploy**.
3. Every push to `main` updates the site, and other branches get their own preview URLs.

The pages are set to `noindex`, so search engines won't list them.

## Run locally

Serve the folder with any static server, for example:

```
npx serve .
```
