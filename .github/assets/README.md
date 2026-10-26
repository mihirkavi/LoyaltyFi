# README images

Images used by the root `README.md`.

| File | What it is | How it was made |
| --- | --- | --- |
| `banner-light.png`, `banner-dark.png` | README banner for light and dark mode | Rendered from [`source/banner.html`](source/banner.html) with headless Chrome (26 October 2026), using `assets/brand/logo.png` |

The README also shows the concept visuals already in the repository root (`UI Mobile User.png`, `Onboarding.png` and the value flywheel). Those are pitch illustrations, not screenshots of working software.

Images here must only show public or synthetic content. Label any concept art or mockup as such where it is used.

## Visual identity

Consumer fintech and rewards apps use crisp geometric sans-serifs, big confident numbers and card shapes. The palette comes straight from the logo so the banner, footer logo and mockup read as one brand.

- **Fonts:** **Plus Jakarta Sans** (display, 800) and **Inter** (body).
- **Colours:** `#4f194d` aubergine, `#fb5b4d` coral and `#fddbbd` peach (sampled from `assets/brand/logo.png`), `#0e1d2d` ink navy (the buttons in `UI Mobile User.png`), `#fff7f0` cream background and `#1c0b1f` dark background.
- **Motif:** two tilted loyalty cards ("Airline miles" and "Coffee stars", no real brands) joined by a round swap button, echoing the swap screen in the concept mockup.

The README badges use the same colours. To change the banner, edit [`source/banner.html`](source/banner.html) and follow [`source/README.md`](source/README.md) to re-render both PNGs.
