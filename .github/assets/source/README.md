# Banner source

`banner.html` is the self-contained source of the README banner (`../banner-light.png` and `../banner-dark.png`). One file holds both themes: a `@media (prefers-color-scheme: dark)` block swaps the colours.

## Identity

- **Fonts:** **Plus Jakarta Sans** (display, 800) and **Inter** (body), loaded from Google Fonts.
- **Colours:** `#4f194d` aubergine, `#fb5b4d` coral and `#fddbbd` peach (sampled from `assets/brand/logo.png`), `#0e1d2d` ink navy (the buttons in `UI Mobile User.png`), `#fff7f0` cream background and `#1c0b1f` dark background.
- **Motif:** two tilted loyalty cards ("Airline miles" and "Coffee stars", no real brands) joined by a round swap button, echoing the swap screen in the concept mockup.
- The logo is loaded from `../../../assets/brand/logo.png`; in dark mode it sits on a cream tile so the aubergine stays visible.

## Re-render

From the repository root:

```bash
export CHROME_PATH="<path to a Chrome or Chromium binary>"
node render-html.mjs .github/assets/source/banner.html .github/assets/banner-light.png --scheme light
node render-html.mjs .github/assets/source/banner.html .github/assets/banner-dark.png --scheme dark
```

`render-html.mjs` is a small Playwright script (not in this repository) that opens the page at 1600 x 600, waits for fonts, and saves a 2x screenshot with the given `prefers-color-scheme`. Any headless browser that screenshots a 1600 x 600 viewport at 2x, once in light and once in dark mode, gives the same result.

## Notes for agents

- Keep the banner honest: no invented numbers, users, partners or results. Status words in the banner must match the README's "Honest status" section.
- Check both PNGs after rendering for overflow, clipped text and weak contrast.
