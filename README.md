# elmlake.com

Landing page for [elmlake.com](https://elmlake.com) — a gateway to the Elm Lake family of ventures.

## Purpose

This site serves as a simple hub that directs visitors to either:

- **[Elm Lake Cranberry](https://elmlakecranberry.com)** — Four-generation cranberry farming operation in Cranmoor, Wisconsin. Grower-owners with Ocean Spray since 1901.
- **[Elm Lake Labs](https://elmlakelabs.com)** — Technology studio building modern software solutions.

The page is intentionally minimal: a hero section with the Elm Lake name, two cards linking to each venture, and nothing else. It's meant to load fast, look elegant, and get visitors where they need to go.

## Tech Stack

- **Framework**: [Astro](https://astro.build) (static site generation)
- **Styling**: Scoped CSS with CSS custom properties
- **Fonts**: Cormorant Garamond (display) + DM Sans (body) via Google Fonts
- **Node**: v22 (see `.nvmrc`)

## Project Structure

```
/
├── public/
│   ├── favicon.svg
│   └── images/
│       ├── ELC/          # Elm Lake Cranberry assets
│       │   └── logo-white.png
│       └── ELL/          # Elm Lake Labs assets
│           └── logo-white.png
├── src/
│   └── pages/
│       └── index.astro   # Single-page site
└── package.json
```

## Development

```bash
# Install dependencies
npm install

# Start dev server (localhost:4321)
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## Design Notes

- **Color palette**: Warm cream background (#FAF7F2) with cranberry/forest gradient for the farm card, slate/ink gradient for the labs card
- **Typography**: Elegant serif display font paired with clean sans-serif body text
- **Effects**: Subtle grain texture overlay, fade-up animations on load, hover lift on cards
- **Responsive**: Two-column grid on desktop, single column on mobile

## Related Repositories

- [elmlakecranberry.com](https://github.com/mossjm/elmlakecranberry.com) — Elm Lake Cranberry website
- elmlakelabs.com — Elm Lake Labs website (if/when created)

## Deployment

The site is static and can be deployed to any static hosting provider (Netlify, Vercel, Cloudflare Pages, etc.). The build output goes to `./dist/`.
