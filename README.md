# LuminaCrowd Website

Marketing and support website for the LuminaCrowd iOS app.

## URLs

- **Marketing**: https://karapirinc.github.io/luminacrowd-website/
- **Join**: https://karapirinc.github.io/luminacrowd-website/join?c=<encodedConfig>
- **Support**: https://karapirinc.github.io/luminacrowd-website/support.html

## About LuminaCrowd

LuminaCrowd transforms your phone into a synchronized light show pixel for concerts and crowd events. Features include:

- 10-color iOS palette
- Three display modes: SOLID, PULSE, STROBE
- Music Sync with beat detection
- Pro Themes (Police, Rainbow, Fire, Ocean, Strobe)
- Haptic feedback

## Development

This is a static HTML site styled with Tailwind CSS (via CDN).

To preview locally, simply open `index.html` in a browser or use a local server:

```bash
# Using Python
python -m http.server 8000

# Using Node.js (npx)
npx serve .
```

## Deployment

Automatic deployment via GitHub Actions on push to the `main` branch.

The workflow:
1. Triggers on push to `main`
2. Uploads the entire repository as an artifact
3. Deploys to GitHub Pages

## License

Copyright 2024 LuminaCrowd. All rights reserved.
