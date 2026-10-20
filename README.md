# retroswim-site

Static site for the iOS game **Flip Turn** (formerly Retro Swim; the repo and URLs keep the old name), served by GitHub Pages from `main` (root).

- Home: https://akikawasaki21.github.io/retroswim-site/
- Privacy Policy: https://akikawasaki21.github.io/retroswim-site/privacy/
- Support: https://akikawasaki21.github.io/retroswim-site/support/

Plain HTML and CSS. No build step, no JavaScript, no analytics, no cookies, no third-party requests.
Fonts are self-hosted (SIL Open Font License, see `assets/fonts/*-OFL.txt`).

## When the app goes live

1. In `index.html`, replace both `href="#"` App Store buttons with `https://apps.apple.com/app/id<APP_ID>`
   and remove the two "Coming soon" lines.
2. Uncomment the Smart App Banner tag in the `<head>` of `index.html` (and add it to
   `privacy/index.html` and `support/index.html` if you want it there) with the real ID:
   `<meta name="apple-itunes-app" content="app-id=<APP_ID>">`

## Preview locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000/.
