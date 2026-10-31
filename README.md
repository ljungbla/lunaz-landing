# Lunaz landing page

A single-file, static landing page for the Lunaz iPhone app. Lumi, the light spirit, flies through a shifting nebula as you scroll, reacts at every section, and a live iPhone 17 mockup changes screens with the page.

- `index.html` holds everything (HTML, CSS and JS). three.js 0.149 loads from jsDelivr and fonts from Google Fonts.
- Served with GitHub Pages from the `main` branch root. `.nojekyll` skips the Jekyll build.

## Editing

- **App Store link:** set `APP_URL` near the top of the main script. Every download button uses it.
- **Copy:** each section is a `<section class="sec">` in `<main>`.
- **Lumi's path:** each section's `data-lumi="x,y,scale"` (desktop) and `data-lumi-m` (phone) set where Lumi rests, in screen units from -1 to 1. `data-emote` sets how Lumi reacts on arrival (`laugh`, `excite`, `cry`).
- **Sky colours:** the `SKIES` palette in the script, one entry per `data-sky` stage (`dusk`, `dusk2`, `night`, `aurora`, `sunrise`).

Open `index.html` in a browser to preview locally.
