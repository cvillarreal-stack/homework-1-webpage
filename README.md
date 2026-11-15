# Project Milestone 3: Accessible & Designed

Live Site: https://cvillarreal-stack.github.io/homework-1-webpage/

## Project Structure
- `index.html`: Home page
- `projects.html`: Featured projects and work
- `about.html`: About me and accessible contact form
- `styles.css`: Shared stylesheet with consistent colors, responsive layout, and Gestalt visual design

## Accessibility Fixes (WAVE & WCAG AA)
- Marked the decorative header SVG wave divider with `aria-hidden="true"` and `focusable="false"` so screen readers skip decorative graphics.
- Lightened the footer email link color on `#0f3460` from `#FF6B81` (4.3:1) to `#FF8598` (5.3:1) so all text and links pass WCAG AA contrast standards.
- Paired every `<input>`, `<select>`, and `<textarea>` in the `about.html` contact form with an explicit `<label for="...">` attribute to eliminate missing form label errors in WAVE.
- Grouped related form fields with `<fieldset>` and `<legend>` elements and added `aria-invalid` and `role="alert"` error states that use both `#c81e3b` text and thicker borders.

## Visual Design & Gestalt Principles
- **Proximity:** I used proximity to group my project cards and form inputs by keeping tight internal padding inside each `.project-card` and `.form-group` while placing wider margins between distinct `.card-section` containers.
- **Similarity:** I used similarity across `index.html`, `projects.html`, and `about.html` by styling all section cards with matching `#0f3460` borders, `8px` border radii, `#1a1a2e` headers, and `#e94560` accents.
- **Figure-Ground:** I used figure-ground contrast by placing `#ffffff` cards over a `#f8f9fa` page background with `#1a1a2e` text to separate foreground content from the page canvas.

## Consistent Color Palette
- **Primary Color:** `#1A1A2E` (Dark Slate / Navy)
- **Secondary Color:** `#0F3460` (Deep Blue)
- **Accent & High-Contrast Colors:** `#E94560` (Coral borders), `#FF6B81` / `#FF8598` (WCAG AA links on dark backgrounds), `#C81E3B` (WCAG AA form error text)
- **Background Color:** `#F8F9FA` (Off-white / Soft Grey)
