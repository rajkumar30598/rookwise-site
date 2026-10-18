# Rookwise Site

Marketing website and privacy policy for **Rookwise**, a free, ad-free Android chess coach app.

**Live site:** https://rajkumar30598.github.io/rookwise-site/

## About Rookwise

Rookwise helps players learn chess, review their games like a coach, and train on puzzles built from their own mistakes. The engine (Stockfish) runs on the phone, so most features work offline. The app is currently in testing on Google Play.

## What the site contains

- **Landing page** (`index.html`): app overview, feature sections (Learn, Review, Train, more ways to play), a carousel of 25 in-app screenshots, an interactive "find the winning move" puzzle, FAQ and an early-access sign-up link.
- **Privacy policy** (`privacy/index.html`): what stays on the device, data shared with Lichess and Chess.com, anonymous usage statistics (Google Analytics for Firebase, opt-out), permissions, and step-by-step data deletion (`privacy/#delete`).
- Light and dark themes, responsive layout, Open Graph image and `MobileApplication` structured data.
- `robots.txt` and `sitemap.xml` for search engines.

## Tech stack

- Plain static HTML and CSS with a small amount of inline JavaScript. No build step or dependencies.
- Fonts from Google Fonts (Bricolage Grotesque, Inter).
- Hosted on GitHub Pages (`.nojekyll` disables Jekyll processing).

## Project structure

```
index.html          Landing page
privacy/index.html  Privacy policy and data deletion instructions
img/app/            App screenshots
img/pieces/         Chess piece images for the interactive puzzle
img/og.jpg          Social preview image
icon-512.png        App icon
robots.txt, sitemap.xml
```

## Run locally

Any static file server works:

```bash
git clone https://github.com/rajkumar30598/rookwise-site.git
cd rookwise-site
python3 -m http.server 8000
# open http://localhost:8000
```

## Deployment

Pushes to `main` are served by GitHub Pages.

## Contact

rajkumar30598@gmail.com
