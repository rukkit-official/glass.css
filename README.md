# glass.css

> **Semantic HTML, but frosted.**

**glass.css** is a drop‑in Glassmorphism CSS layer that turns your existing UI into frosted glass.
No reset. No layout rules. No JavaScript.
Just load it, and everything becomes glass.

Designed to stack cleanly on top of minimal CSS frameworks like **Pico.css**, **Simple.css**, and **Water.css**.

---

## Why glass.css

Most Glassmorphism styles are snippets, not frameworks.
Most CSS frameworks handle layout, not visual effects.

**glass.css exists in between.**

* ✨ Glassmorphism as a *layer*, not a framework
* 🧱 Semantic‑first (styles real HTML elements)
* 🪶 Lightweight single file
* 🧩 Framework‑agnostic
* 📴 No JavaScript

---

## Features

* Automatic glass styling for:

  * `article`, `section`, `nav`, `header`, `footer`, `aside`
  * buttons and form controls
  * tables and dialogs
* CSS variables for easy customization
* Dark mode support (`prefers-color-scheme`)
* Graceful fallback when `backdrop-filter` is unsupported

---

## Usage from NPM

```html
npm install glass_ui.css
```

```html
yarn install glass_ui.css
```

## Usage from CDN

```html
<link rel="stylesheet" href="https://rukkit.net/css/glass.css">
```
```html
<link
  rel="stylesheet"
  href="https://cdn.jsdelivr.net/npm/glass_ui.css/glass_ui.css"
/>
```

Stack it on top of another framework:pico.css

```html
<link
  rel="stylesheet"
  href="https://cdn.jsdelivr.net/npm/@picocss/pico@2/css/pico.min.css"
>
```

No extra classes required.

---

## Basic Example

```html
<article>
  <h1>Hello Glass</h1>
  <p>Semantic HTML with a frosted UI.</p>
  <button>Click me</button>
</article>
```

---

## Utility Classes

Optional helpers are provided when you want manual control:

```html
<div class="glass">Default glass</div>
<div class="glass-soft">Softer glass</div>
<div class="glass-strong">Stronger glass</div>
```

---

## Customization

All visuals are controlled through CSS variables:

```css
:root {
  --glass-bg: rgba(255,255,255,0.16);
  --glass-border: rgba(255,255,255,0.28);
  --glass-blur: 14px;
  --glass-radius: 1rem;
}
```

Override them anywhere:

```css
body {
  --glass-blur: 20px;
}
```

---

## Dark Mode

glass.css automatically adapts to system dark mode:

* darker glass backgrounds
* softer borders
* same semantic structure

No configuration required.

---

## Browser Support

* Modern Chromium browsers ✅
* Safari (macOS / iOS) ✅
* Firefox ⚠️ (fallback background used)

When `backdrop-filter` is unavailable, glass.css falls back to solid translucent surfaces.

---

## Philosophy

* Glass is an effect, not a layout
* Semantic HTML should stay semantic
* CSS should be stackable, not invasive

**glass.css does not replace your framework.**
It enhances it.

---

## License

MIT License
