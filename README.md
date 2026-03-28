# LuminaCrowd Website

Marketing and support website for the LuminaCrowd iOS app.

## URLs

- **Primary domain**: https://luminacrowd.yiok.ai/
- **Join**: https://luminacrowd.yiok.ai/join?c=<encodedConfig>
- **Support**: https://luminacrowd.yiok.ai/support.html
- **Universal links AASA**: https://luminacrowd.yiok.ai/.well-known/apple-app-site-association

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

This repo is intended to be served from `luminacrowd.yiok.ai`.

For Apple universal links, both of these files must resolve with `200 OK` and no redirect:

- `/.well-known/apple-app-site-association`
- `/apple-app-site-association`

The checked-in `_headers` file is for Cloudflare Pages so those extensionless files are served as `application/json`.

## License

Copyright 2024 LuminaCrowd. All rights reserved.
