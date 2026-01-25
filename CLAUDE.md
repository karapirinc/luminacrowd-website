# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

LuminaCrowd Website is a static marketing and support site for the LuminaCrowd iOS app. It's hosted on GitHub Pages with automatic deployment.

## Development

This is a zero-dependency static site. No build tools, npm, or compilation required.

**Local preview:**
```bash
python -m http.server 8000
# or
npx serve .
```

**Deployment:** Automatic via GitHub Actions on push to `main` branch.

## Architecture

Two standalone HTML pages styled with Tailwind CSS (CDN):

- `index.html` - Marketing page with hero video, features grid, screenshot gallery
- `support.html` - FAQ (collapsible `<details>` elements), troubleshooting, contact info

Both pages include identical Tailwind config blocks defining custom colors and animations.

## Tailwind Customization

Custom brand colors available: `app-red`, `app-blue`, `app-green`, `app-yellow`, `app-purple`, `app-cyan`, `app-orange`, `app-pink`, `app-indigo`

Custom animations: `glow` (text-shadow pulse), `float` (Y-axis oscillation)

Font family: `font-display` for SF Pro Display with system fallbacks

## Conventions

- All styling uses Tailwind utility classes inline
- Custom styles defined in `<style>` blocks: `.gradient-text`, `.phone-frame`, `.screenshot-card`
- Semantic HTML structure with proper alt texts
- Mobile-first responsive design using Tailwind breakpoints (md/lg)
- Keep both pages' navigation and Tailwind configs synchronized
