# Effects Atlas

A hands-on catalogue of 37 motion and interaction effects for web covers and portfolio pages — each one live in its own tab, built with plain HTML, CSS and JavaScript.

**Live:** https://oz-the-magician.github.io/effects-atlas/

## Effects

| Type | Effects |
|---|---|
| Typography | Variable font · Masks · Scramble · Circular text · Marquee · Rubber text · Gravity · Grid shuffle · Velocity stretch · Shatter · Wave line · Text tunnel · Split-flap · Dithered text · Marker · 3D letters |
| Images | Liquid image · Particles · Pixel reveal · Halftone · Morph · Lens · Layered parallax · Image trail · Holo cards |
| Layout & navigation | 3D cards · Ring carousel · Scroll story · Cursor and magnet · Case transition · Ribbon · Ribbon + mesh |
| Backgrounds & 3D | Gradient mesh · Dot wave · Dots + trail · Sphere over cubes · Exploded view |

Open a tab, move the mouse, scroll or drag — most effects react to input. You can link straight to an effect with its id, e.g. `#ci` for circular text.

## How it's built

- One self-contained `index.html`: images are embedded, and GSAP, Lenis and three.js are inlined, so nothing loads from a CDN except Google Fonts.
- WebGL shaders for the image and mesh effects, Canvas 2D for dots and pixels, three.js for the 3D scene.
- Respects `prefers-reduced-motion`.

## Run locally

Open `index.html` in a browser. No build step.

---

## Русский

**Effects Atlas** — живой каталог из 37 моушн- и интерактивных эффектов для обложек сайтов и страниц портфолио. Каждый эффект открыт в отдельном табе и сделан на чистом HTML, CSS и JavaScript.

**Посмотреть:** https://oz-the-magician.github.io/effects-atlas/

- Типографика: variable-шрифт, маски, scramble, текст по кругу, бегущая строка, резиновый текст, гравитация, перестановка по сетке, растяжение от скорости, разлёт на осколки, волна по строке, текстовый туннель, табло split-flap, дизеринг, маркер, 3D-буквы.
- Изображения: жидкая картинка, частицы, пиксельный reveal, halftone, перетекание, линза, слоевой параллакс, шлейф картинок, голо-карточки.
- Раскладка и навигация: 3D-карточки, карусель по кругу, скролл-история, курсор и магниты, переход в кейс, лента, лента на меше.
- Фоны и 3D: градиентный меш, точки-волна, точки со шлейфом, шар над кубами, часы в разборе (exploded view).

Всё в одном файле `index.html`: картинки и библиотеки (GSAP, Lenis, three.js) встроены внутрь, сборка не нужна — достаточно открыть файл в браузере.
