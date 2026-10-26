# Dream Spire School: franchise brochure website

A plain static website: `index.html` plus the `assets/` folder (photos, videos, logo)
and the downloadable PDF brochure. No build step and no frameworks.

## Deploy on Netlify (easiest)
1. Go to https://app.netlify.com/drop
2. Drag this whole `website` folder onto the page.
3. Netlify gives you a live link. Rename it under Site settings, or add your own domain.

With the Netlify CLI:
```
netlify deploy --dir . --prod
```

## Deploy on Vercel
```
npx vercel --prod
```
Run it inside this folder. When asked, choose "Other" as the framework, with no build command.

## Host anywhere else
Upload the contents of this folder to any web host (cPanel, S3, GitHub Pages and so on).
`index.html` must sit at the root.

## After you have a domain
WhatsApp and Facebook need a full address for the link-preview image. In `index.html`, change
`<meta property="og:image" content="assets/og-image.jpg">`
to your full URL, for example
`https://franchise.dreamspireschool.com/assets/og-image.jpg`.

## Editing
- Text, prices and contact details are all in `index.html`. Search for the text you want to change.
- Replace a photo by overwriting the file in `assets/web/` with the same name.
- Videos live in `assets/video/`. Each has a full version (`v4.mp4`), a short silent preview
  (`v4-preview.mp4`) and a poster frame (`v4.jpg`).
