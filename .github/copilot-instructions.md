### Repository overview

This is a small static-site course repository (WDD 130 starter template). It contains simple HTML pages and CSS grouped by week under top-level folders like `week01/`, `week02/`, etc. Key entry points are `index.html`, `README.md`, and the per-week HTML files (for example `week01/first-page.html`). Images live in top-level `images/` and each week may have its own `images/` and `styles/` subfolders.

### Goal for an AI coding agent

Help maintain, improve, and generate static HTML/CSS lesson pages and assets that follow the repository's minimal, educational structure. Preferred outputs are small, well-formed HTML files and matching CSS files, with relative paths and no build steps.

### Project-specific conventions

- Flat, week-based organization: each lesson is a folder `weekNN/` containing HTML and optionally `styles/` and `images/` subfolders.
- Keep files small and self-contained. For new styles, add a CSS file under the week's `styles/` folder and reference it with a relative link in the lesson HTML (example: `week02/styles/basic.css`).
- Images are referenced with relative paths (example in `index.html`: `images/salt-lake-temple.jpg`).
- Do not introduce a build system, package.json, or server-side code unless explicitly requested.

### Code style and quality

- Output valid HTML5 (<!DOCTYPE html>, lang attribute on `<html>`, meta charset and viewport). See `index.html` and `week01/first-page.html` for examples.
- Prefer semantic HTML (headings, paragraphs, lists, images with alt attributes).
- Keep CSS modular per-week; avoid global changes to the top-level `styles/` unless the user requests a site-wide stylesheet.

### Common tasks and examples

- Add a new lesson page: create `weekNN/new-lesson.html` and optionally `weekNN/styles/new-lesson.css`. Link CSS from the lesson with a relative path.
- Fix image path issues: verify image file exists (e.g., `images/` or `weekNN/images/`) and update the `<img src="...">` path to the correct relative location.
- Improve accessibility: ensure `<img>` tags include descriptive `alt` text and headings follow logical order.

### Files & patterns to reference

- `index.html` — top-level landing page; shows how images are referenced and basic structure.
- `week01/first-page.html` — minimal lesson example to mimic when creating new pages.
- Week folders like `week02/styles/` and `week04/styles/` — examples of per-week CSS organization.

### Developer workflows (what to assume)

- There is no build/test pipeline. Preview by opening HTML files in a browser or using a simple static server if requested (e.g., Python `http.server` or VS Code Live Server). Ask the user before suggesting or adding server tooling.
- Keep changes small and explicitly describe any added files and where they were placed.

### When to ask for clarification

- If a request affects multiple weeks or requires a site-wide stylesheet, confirm whether to place files at the top-level `styles/` or inside `weekNN/styles/`.
- If introducing tooling (linters, build systems, package managers), ask permission first.

### Examples of prompts for the user

- "Create a new lesson page `week06/contact.html` with a form and a local stylesheet `week06/styles/contact.css` — confirm if the form should be functional or static." 
- "I can add a site-wide stylesheet at `/styles/styles.css` and update all pages to reference it — proceed?"

### Safety and limits

- Don't add external dependencies or remote scripts without explicit user approval.
- Keep student content (names, images) generic unless user provides replacement assets.

If any part of these instructions is unclear or you want different conventions (for example, a centralized stylesheet or a build step), tell me and I will update this file.
