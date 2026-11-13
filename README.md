# DBE 2027

An unofficial, installable page for the 2027 edition of
[Dark Bombastic Evening](https://darkbombasticevening.com): 12–14 August 2027,
RYMA, Alba Iulia, Romania.

**[Open it](https://aoprisan.github.io/dbe2027/)**

It carries only what the festival has announced so far — the dates, three
nights each marked TBA, and a link to the tickets on eventbook.ro. Bands and
times get added when the festival names them. This is a fan-made project and is
not affiliated with Dark Bombastic Evening.

The 2026 planner is a separate app with its own repository:
[aoprisan/dbe2026](https://github.com/aoprisan/dbe2026).

## Development

Node.js 20 or newer.

```bash
npm install
npm run dev
```

```bash
npm run build
```

Vite serves the project under `/dbe2027/` to match its GitHub Pages path. A push
to `main` builds and deploys it through
[`.github/workflows/deploy.yml`](.github/workflows/deploy.yml); GitHub Pages
must be set to deploy from GitHub Actions in the repository settings.

## Where things live

- [`src/data.ts`](src/data.ts) — the dates, the venue, the links, the nights
- [`src/main.ts`](src/main.ts) — the page
- [`src/style.css`](src/style.css) — the palette, taken from the 2027 poster
- [`scripts/logo-art.mjs`](scripts/logo-art.mjs) — the emblem, as vector art;
  `npm run icons` (run by the build) rasterises it into the PWA icons

## License

AGPL-3.0-only — see [LICENSE](LICENSE).
