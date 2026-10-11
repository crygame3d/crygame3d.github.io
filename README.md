# Gridfire Arena

A free first-person arena shooter for the browser. One page, no libraries, no external requests.

## Files

| File | Purpose |
|---|---|
| `index.html` | The game and the SEO content (everything in one file) |
| `og-image.png` | Preview image used when the link is shared (1200x630) |
| `sitemap.xml` | Tells search engines which pages exist |
| `robots.txt` | Allows crawling and points to the sitemap |

## Before publishing: replace the placeholder domain

The files contain `https://YOUR-DOMAIN.com/` in these places: canonical link, Open Graph and Twitter tags,
JSON-LD data in `index.html`, plus `sitemap.xml` and `robots.txt`.

Use Find & Replace in your editor across all files:

    https://YOUR-DOMAIN.com/   ->   https://your-real-address.com/

Keep the trailing slash. If you publish at `https://name.github.io/`, use that address.

## Publish with GitHub Pages (free)

1. Create a public repository named `<name>.github.io`.
2. Upload all four files to the root of the repository.
3. Settings -> Pages -> Deploy from a branch -> `main` and `/ (root)`.

## SEO checklist

- [ ] Replace the placeholder domain (see above)
- [ ] Open the live page and check the game loads
- [ ] Add the site to Google Search Console and submit `sitemap.xml`
- [ ] Test the page with PageSpeed Insights (aim for green scores)
- [ ] Share the link once in a chat app to confirm the preview image shows
- [ ] Add more original pages over time (guides, tips, weapon pages) and link them from the home page
- [ ] Keep the content original. Do not copy text, images, names or logos from other games

## Controls

WASD move, mouse aim, left click fire, Space jump, Shift sprint, R reload, 1-3 or wheel switch weapon,
M mute, F fullscreen, Esc pause.

## Tune the game

Near the top of the `<script>` in `index.html`:

- `DIFF` sets number of bots, their accuracy, damage and reaction time for each difficulty
- `LIMIT` is the number of eliminations needed to win
- `W` holds the three weapons (damage, spread, fire delay, magazine, reload time)
