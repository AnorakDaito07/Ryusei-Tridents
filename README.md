# Ryusei Tridents

Static site (plain HTML/CSS/JS, no build step). Navigation uses hash routes (`#home`, `#events`, `#contact`), so no rewrites are needed.

## Deploy to Vercel

**Dashboard:** push this folder to GitHub, then Vercel > Add New > Project > import the repo.
Framework Preset: **Other**. Leave Build Command and Output Directory empty.

**CLI:**
```bash
npm i -g vercel
vercel        # preview
vercel --prod # production
```

## After the first deploy
Set absolute URLs for social previews in `index.html` (`og:image` must be absolute for Facebook/X/WhatsApp), e.g.
`<meta property="og:image" content="https://YOUR-DOMAIN/assets/crest.png">` and add `<meta property="og:url" content="https://YOUR-DOMAIN/">`.
