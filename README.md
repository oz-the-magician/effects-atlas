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

## How to use

1. Open the atlas and pick an effect tab.
2. Press **Copy prompt** under the description.
3. Paste it into Claude (or any capable model) and replace the placeholders in square brackets — `[your text]`, `[your image]`, `[palette]` and so on — with your own content.
4. Every prompt describes the look, the interaction, the key values used in the preview and the technique, and asks for a single self-contained HTML file that respects reduced motion and works on mobile.

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

**Как пользоваться:** откройте нужный эффект, нажмите **Copy prompt** под описанием, вставьте промпт в Claude или другую модель и замените плейсхолдеры в квадратных скобках (`[your text]`, `[your image]`, `[palette]` и т. д.) на свой контент. В каждом промпте описаны внешний вид, взаимодействие, ключевые параметры из превью и техника, а результат — один самодостаточный HTML-файл, который учитывает reduced motion и работает на телефоне.

Всё в одном файле `index.html`: картинки и библиотеки (GSAP, Lenis, three.js) встроены внутрь, сборка не нужна — достаточно открыть файл в браузере.
