# Serena Lee Photography

One-page personal site for Serena Lee, a freelance wedding and portrait photographer.
Plain HTML and CSS, no build step and no dependencies. Fonts load from Google Fonts.

## Files

- `index.html`: the whole site (styles inline)
- `photos/`: portfolio images
- `vercel.json`: Vercel settings (clean URLs, caching, basic headers)

## Deploy on Vercel

1. In Vercel, choose **Add New > Project** and import this repository.
2. Leave Framework Preset as **Other**. Leave Build Command and Output Directory empty. Set Root Directory to `./`.
3. Select **Deploy**. Every push to `main` redeploys the site.

Or from the command line: `npx vercel --prod`.

## Editing

- **Photos:** add images to `photos/`, then replace a placeholder `<div class="frame" ...></div>` in `index.html` with
  `<div class="frame"><img src="photos/your-file.jpg" width="1200" height="1500" alt="Describe the photo"></div>`.
  Use images about 1200 px wide or larger, cropped near 4:5.
- **Email:** change both the `href` and the text of the link inside `#contact`. It is currently the placeholder `hello@serenalee.com`.
- **Colors:** the dark palette lives in the `:root` block at the top of the `<style>` tag.
