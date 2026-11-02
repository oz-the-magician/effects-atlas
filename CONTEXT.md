# Effects Atlas — context

Live: https://oz-the-magician.github.io/effects-atlas/ · Repo: oz-the-magician/effects-atlas · Local: ~/Projects/effects-atlas

## What it is
A single self-contained `index.html` with 37 interactive web motion effects, one per tab, each with a **Copy prompt** button. Images are embedded as data URIs; GSAP, Lenis and three.js are inlined (no CDN except Google Fonts).

## Groups
- Typography: Variable font, Masks, Scramble, Circular text, Marquee, Rubber text, Gravity, Grid shuffle, Velocity stretch, Shatter, Wave line, Text tunnel, Split-flap, Dithered text, Marker, 3D letters
- Images: Liquid image, Particles, Pixel reveal, Halftone, Morph, Lens, Layered parallax, Image trail, Holo cards
- Layout & navigation: 3D cards, Ring carousel, Scroll story, Cursor and magnet, Case transition, Ribbon, Ribbon + mesh
- Backgrounds & 3D: Gradient mesh, Dot wave, Dots + trail, Sphere over cubes, Exploded view

## Decisions
- Removed for good: Text window, Blinds, Bend + Lenis, Flythrough: canyon.
- Ribbon + mesh: background colours are sampled from the card in the centre.
- Dot wave and Dots + trail run at half the original speed.
- Exploded view shows a generic mechanical watch — no brand marks.
- Prompts are in English with placeholders in [square brackets] and a shared tail (reduced motion, touch, single HTML file, mobile).

## How to add an effect
1. Add `<section class="fx" id="xx" data-name="Name">` with a `.cap` (title + description). Tabs are built from section order.
2. Add CSS scoped to `#xx`.
3. Add JS before `const start=(location.hash…`: register `fx.xx={start(){…},stop(){…}}`, wrapped in `try{…}catch`.
4. Add the prompt text to the `P` object (key = id) in the copy-prompt block.
5. Update README (count + table, EN and RU).

## Notes
- GitHub Pages is enabled manually: Settings → Pages → Deploy from a branch → main / root.
- `_refs/` holds local reference videos and is git-ignored.
- Commits only after OZ confirms (files + message), English messages.
