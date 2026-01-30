# Color & Typography Theme Generator

A small, focused frontend utility for generating **curated color palettes and typography pairings** and applying them to a realistic UI preview.  
Built as a **single-file static web application** using HTML, CSS, and vanilla JavaScript.

This project emphasizes **engineering judgment, restraint, and maintainability** over novelty.

---

## Purpose

This tool demonstrates how visual design rules can be encoded into clear, predictable frontend logic.

It is intentionally scoped to show:
- Thoughtful state management
- Constrained randomness (curation over chaos)
- Accessibility-aware UI decisions
- Clean separation between preview and control surfaces

The result is a practical design utility—not a demo or experiment.

---

## Features

### Theme Generation
- Generates a complete theme consisting of:
  - Background color
  - Text color
  - Primary color
  - Accent color
  - Heading font
  - Body font
- All combinations are **curated** to avoid low-quality or unreadable results.

### Live Preview
- Central preview surface that reflects the active theme.
- Includes:
  - Heading and body copy
  - Primary and secondary buttons
  - Secondary UI element (badge)
- Designed to resemble a real application UI, not a blank canvas.

### Controlled Iteration
- Lock colors or fonts independently.
- Regenerate only the unlocked parts of the theme.
- Lock state is explicit and accessible.

### Preview-only vs Global Application
- Toggle between:
  - **Preview-only**: theme applies only to the preview surface.
  - **Global**: theme applies to the entire document.
- Useful for validating real-world readability and typography behavior.

### Export
- Copy the current theme as CSS variables.
- Output is immediately usable in real projects.

### Reset
- Restores a known, stable default theme.
- Clears locks and global application state.

---

## Accessibility & UX Considerations

- Semantic HTML throughout.
- All controls are keyboard-accessible.
- Visible focus states for interactive elements.
- Respects system preferences:
  - `prefers-reduced-motion`
  - `prefers-color-scheme`
- Fonts include system fallbacks.
- Subtle, non-distracting transitions only.

---

## Technical Constraints

- Single `index.html` file.
- No frameworks, build tools, or runtime dependencies.
- All CSS in one `<style>` block.
- All JavaScript in one `<script>` block.
- Uses CSS variables as the primary theming mechanism.
- A single state object acts as the source of truth.

---

## Architecture Overview

- **State-driven UI**  
  All visual updates derive from a single state object.

- **Scoped theming**  
  Themes are applied via CSS variables to either:
  - the preview container, or
  - the document root (global mode).

- **Explicit logic**  
  Small, named functions with clear responsibility.
  No ad-hoc DOM manipulation.

---

## Why This Project Exists

This project is designed for **frontend engineers, engineering managers, and product-minded reviewers** who care about:

- Code clarity
- Predictable behavior
- Design-system thinking
- Professional restraint

It intentionally avoids:
- Over-customization UI
- Heavy visual effects
- Framework abstractions
- Artificial complexity

---

## Running the Project

1. Download or clone the repository.
2. Open `index.html` in any modern browser.
3. No setup required.

---

## License

MIT — free to use, modify, and adapt.

---

## Author Notes

This project prioritizes **how decisions are made** over how many features are included.  
Every interaction and constraint exists to demonstrate real-world frontend engineering judgment.
