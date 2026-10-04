# Birthday Website — Restu Oktaviani

A personal cinematic birthday website. Dark, romantic, mobile-first.

## Quick Start

Open `index.html` in any browser. No server required.

## Deploy

- **GitHub Pages**: Push repo → Settings → Pages → `main` branch / root
- **Vercel / Netlify**: Drag the folder into the dashboard (static site, zero config)

## Photo Replacement

All photos live in `/assets/`. Replace with your actual files:

| File | Used in |
|------|---------|
| `assets/restu-2020.jpeg`    | Section 1 (The Beginning) + Memories |
| `assets/restu-past.jpeg`    | Section 2 (The Past) + Memories |
| `assets/reunited-2026.jpeg` | Section 4 (2026 / Reunion) + Memories |
| `assets/restu-closing.jpeg` | Section 6 (Memories) + Section 10 (Final) |

> Keep filenames exactly as above, or search `assets/` in `index.html` to update paths.

## Change the Song

1. Get the YouTube video ID from the URL (e.g. `https://youtu.be/XXXXXXXXX` → ID is `XXXXXXXXX`)
2. In `script.js`, update: `const YOUTUBE_VIDEO_ID = 'XXXXXXXXX';`
3. In `index.html`, find the `<iframe>` inside `#s5` and update the `src` attribute — replace `L926aNlMt8A` with your new ID

## Change Colors

Edit CSS variables at the top of `style.css`:

```css
:root {
  --color-maroon:    #6b1a1a;   /* main accent */
  --color-maroon-lt: #8b2a2a;   /* lighter accent */
  --color-bg:        #050505;   /* background */
  --color-text:      #e8e0d5;   /* body text */
}
```

## Change Birthday Details

Search `index.html` for:
- `22.10.2002` — birthday date
- `24th` — age
- `Restu` — name
- `13 March 2020` — first meeting date
- `2026` — reunion year

## Structure

```
/
├── index.html     ← all sections
├── style.css      ← all styles (design tokens at top)
├── script.js      ← interactions, YouTube player, scroll
├── README.md
└── assets/
    ├── restu-2020.jpeg
    ├── restu-past.jpeg
    ├── reunited-2026.jpeg
    └── restu-closing.jpeg
```
