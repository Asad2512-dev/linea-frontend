# Studio Linea | Architecture & Interior Design Portfolio Website

A responsive, multi-section static portfolio site built for **Studio Linea**, an architecture and interior design studio based in Portland, Oregon. This project is a student portfolio submission demonstrating advanced layout architectures using modern CSS3 (Grid, Flexbox, Positioning, Box Model rules) and semantic, accessible HTML5 structures.

---

## Project Overview
This website showcases the work, philosophy, and services of an independent design firm in the Pacific Northwest. The layout is designed to prioritize clean whitespace, visual rhythm, and micro-asymmetry to evoke a premium editorial feel. 

No frameworks (Tailwind, Bootstrap), preprocessors, or JavaScript were used to develop this site.

---

## Features
- **Strict HTML5 Outline**: Built using semantic landmarks to enable logical outline navigation.
- **Pure CSS Scrollspy**: Implemented using modern Scroll-Driven Animations (`timeline-scope`, `view-timeline`) to highlight navigation links dynamically as the user scrolls, entirely free of JavaScript.
- **Micro-Asymmetrical Layout**: Card heights, border tints, and grid proportions are balanced dynamically to feel organic and hand-coded rather than template-generated.
- **Accents & Overlaps**: Experience tags, decorative coordinate lines, and portfolio project badges are placed using relative and absolute boundaries.
- **Fluid Grid Structures**: Clean columns that rearrange automatically using desktop, tablet, and mobile breakpoints.
- **JS-Free Interactive FAQ**: Implements responsive accordion blocks using native HTML `<details>` and `<summary>` elements.

---

## Learning Objectives
This project was designed to demonstrate:
1. Writing semantic, screen-reader accessible HTML document streams.
2. Managing system-wide styling variables (`:root`) for maintainable CSS files.
3. Structuring clear visual hierarchy with typography scale clamps.
4. Using Flexbox for structural alignment and CSS Grid for two-dimensional content sheets.
5. Implementing device boundaries and breakpoint reflow logic.

---

## Technologies Used
- **HTML5**: Markup, semantic regions, and accessibility hooks.
- **CSS3**: Variable states, reset rules, absolute placement coordinates, Flexbox, Grid layouts, and custom media queries.
- **Google Fonts**: Intergraded *Playfair Display* (for headings) and *DM Sans* (for primary copy).

---

## Folder Structure
```text
project/
├── index.html
├── style.css
└── README.md
```

---

## How to Run
1. Download this project directory to your local file system.
2. Double-click or open `index.html` in any browser (Chrome, Edge, Safari, Firefox).
3. No local build systems, servers, or packages are needed.

---

## Responsive Support
- **Desktop (1200px and up)**: Full multi-column viewports with side-by-side flex configurations.
- **Laptops (993px - 1024px)**: Fluid gutters scaling down gracefully to avoid text overflow.
- **Tablets (769px - 992px)**: Grids collapse from three columns to two; header elements stack; overlapping badges shift to natural inline flows.
- **Mobiles (768px and down)**: Clean stacking order, finger-friendly inputs, full-width buttons, and text alignment adjustments.

---

## Accessibility Features
- **Landmark Segments**: Screen reader users can skip sections using `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, and `<footer>`.
- **Keyboard Navigation Hooks**: A functional `.skip-link` allows users to skip directly to `#main-content`. All focusable elements highlight clearly with high-contrast `:focus-visible` borders.
- **WAI-ARIA Metadata**: Critical interactive features or descriptive tags are marked with appropriate `aria-label`, `aria-current="page"`, and `aria-hidden="true"` parameters.
- **Accessible Inputs**: Form controls contain associated structural `<label>` elements and explicit autocomplete values.

---

## CSS Techniques Used
- **Custom Variables**: Centrally declared color tints, font families, base margins, and speeds.
- **Border-Box Resets**: Implemented across all pseudo-elements to ensure padding and borders do not overflow parent widths.
- **CSS Grid Templates**: Utilizing `repeat(3, 1fr)` and asymmetric `grid-column: span 2` rules to align grid modules.
- **Flexbox Positioning**: Configured header columns, testimonial pairs, and footer layouts.

---

## Final Quality Checklist

Here is where each course requirement is explicitly demonstrated in the codebase:

### 1. Semantic HTML5
- `<header>` & `<nav>`: Defined at the top of the body for structural headers (see [index.html: L16-37](file:///Applications/MAMP/htdocs/html/project/index.html#L16-L37)).
- `<main>`: Wraps the core page content (see [index.html: L40](file:///Applications/MAMP/htdocs/html/project/index.html#L40)).
- `<section>`: Applied to discrete sections (`hero-section`, `about-section`, etc.).
- `<article>`: Used for individual service cards and portfolio items (see [index.html: L121-137](file:///Applications/MAMP/htdocs/html/project/index.html#L121-L137)).
- `<aside>`: Defined to present secondary design values (see [index.html: L106-114](file:///Applications/MAMP/htdocs/html/project/index.html#L106-L114)).
- `<footer>`: Structural copyright and columns at page bottom (see [index.html: L374-406](file:///Applications/MAMP/htdocs/html/project/index.html#L374-L406)).

### 2. CSS Box Model (Margin & Padding)
- Custom margins and paddings are styled for block headers, cards, and section divisions (e.g. section margins, card internal paddings, and button elements, see [style.css: L121-133](file:///Applications/MAMP/htdocs/html/project/style.css#L121-L133) and [style.css: L141-155](file:///Applications/MAMP/htdocs/html/project/style.css#L141-L155)).

### 3. Relative & Absolute Positioning
- Relative: `.hero-graphic-container` (see [style.css: L244](file:///Applications/MAMP/htdocs/html/project/style.css#L244)) and `.portfolio-image-box` (see [style.css: L589](file:///Applications/MAMP/htdocs/html/project/style.css#L589)).
- Absolute: Overlapping `.hero-badge` (see [style.css: L269](file:///Applications/MAMP/htdocs/html/project/style.css#L269)) and `.portfolio-card-badge` (see [style.css: L601](file:///Applications/MAMP/htdocs/html/project/style.css#L601)).

### 4. Flexbox
- Header elements align via `.site-header-container` (see [style.css: L175](file:///Applications/MAMP/htdocs/html/project/style.css#L175)).
- Testimonials align via `.reviews-flex-layout` (see [style.css: L457](file:///Applications/MAMP/htdocs/html/project/style.css#L457)).
- Nav links align via `.nav-list` (see [style.css: L189](file:///Applications/MAMP/htdocs/html/project/style.css#L189)).

### 5. CSS Grid
- Services layout matches `.services-grid-layout` (see [style.css: L359](file:///Applications/MAMP/htdocs/html/project/style.css#L359)).
- Portfolio items match `.portfolio-grid-layout` (see [style.css: L380](file:///Applications/MAMP/htdocs/html/project/style.css#L380)).

### 6. Responsive Design
- Handled via mobile-first and viewport media queries (e.g. tablet and mobile viewport configurations, see [style.css: L742-835](file:///Applications/MAMP/htdocs/html/project/style.css#L742-L835)).

---

## Future Improvements
- Implement a CSS-only dark mode using media state queries.
- Add structural SVG inline backgrounds for the blueprint mockups.

