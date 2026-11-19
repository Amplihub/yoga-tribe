# Yoga Tribe · Black Friday landing page

Static build of the V3 design for the 4-Week Mobility Reset Black Friday page.

- `index.html` is the desktop layout, served at the site root.
- `mobile.html` is the mobile layout.

A one-line script at the top of each page picks the right layout: screens narrower than 768px
go to `mobile.html`, and wider screens go to `/`. Old preview links (`/v3/...`, `/v4/...`,
`/v6/...`) redirect to the right page through `vercel.json`.

This is a design preview only. The real page gets built in Wix. Videos stream from Cloudinary;
most photo slots are still labelled placeholders.

## Photo credits

Stock photos in `images/`, free to use under the [Unsplash License](https://unsplash.com/license):

- `back-stretch.jpg`: Margaret Young, [unsplash.com/photos/ocNf_njy6JA](https://unsplash.com/photos/ocNf_njy6JA)
- `hand-lower-back.jpg`: Sasun Bughdaryan, [unsplash.com/photos/bNdiJ1FEbV4](https://unsplash.com/photos/bNdiJ1FEbV4)
- `before-stiff.jpg` and `after-open.jpg` (toned muted / warm): Margaret Young, [unsplash.com/photos/K8EyMWEED3Y](https://unsplash.com/photos/K8EyMWEED3Y) and [unsplash.com/photos/5ARaBcZL_KU](https://unsplash.com/photos/5ARaBcZL_KU)
- `week1-breath.jpg`: Margaret Young, [unsplash.com/photos/yxDXkuAxwhE](https://unsplash.com/photos/yxDXkuAxwhE)
- `week2-pilates.jpg`: ROXANA POPOVICI, [unsplash.com/photos/aY5uOJ2o96g](https://unsplash.com/photos/aY5uOJ2o96g)
- `week3-hips.jpg`: Alina Rubo, [unsplash.com/photos/TaxQjdfhGQM](https://unsplash.com/photos/TaxQjdfhGQM)
- `week4-sound-bath.jpg`: THLT LCX, [unsplash.com/photos/Hn4wYHOaeIc](https://unsplash.com/photos/Hn4wYHOaeIc)

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
