<!-- .github/copilot-instructions.md: Guidance for automated coding agents working on this repo -->

This repository is a small, static Frontend Mentor challenge (HTML/CSS). The guidance below is intentionally narrow and practical so an AI coding agent can be immediately productive.

Keep instructions short, deterministic, and file-focused. When in doubt, prefer small, reversible edits (new CSS files, minor HTML tweaks) and reference the design files in `/design`.

- Project purpose: build a single responsive profile page to match the designs in `/design`.
- Primary stack: plain HTML + CSS. No build tooling, bundlers, or test runners are present.

Key files and folders
- `index.html` — single-page entry; contains minimal placeholder content and the attribution block.
- `style-guide.md` — contains the color palette, font family and sizes, and the two design widths (375px mobile, 1440px desktop). Use this as the authoritative style source.
- `assets/` — images and fonts. Use `assets/images/*` and `assets/fonts/*` paths when editing HTML/CSS.
- `design/` — static JPGs (mobile + desktop) that are the visual spec; use them when matching spacing, sizes and typography.
- `README-template.md` — template README provided by the challenge. `README.md` is starter content that can be replaced.

Conventions and patterns to follow
- Keep changes isolated and minimal: prefer adding a new `styles.css` (or `main.css`) rather than inlining large style blocks in `index.html`.
- Respect the design widths: implement responsive rules that target the mobile-first breakpoint (design mobile first at 375px) and add a media query for desktop at or near 1440px.
- Fonts: local font files are included under `assets/fonts/` — prefer using those (or link to Inter on Google Fonts if necessary). If you update font-face rules, keep file paths relative to `index.html`.
- Images: reference `assets/images/*`. Do not add large images; the repo is optimized for the challenge.
- Accessibility: interactive elements must have visible hover and focus states (the challenge explicitly requires this). Use :focus-visible when appropriate.

Build / preview / debug
- There is no build step. To preview changes, open `index.html` in a browser or serve the folder with a simple static server. (Example: a basic HTTP server is acceptable for local previews.)

Example actionable edit patterns
- Add a stylesheet and link it from `index.html`:
  - new file: `assets/css/main.css` or `styles.css` at repo root
  - update `index.html` head to reference the stylesheet with a relative path
- Use `style-guide.md` values for CSS variables or base styles (colors, font-sizes, font-family).
- For hover/focus example: ensure each social link element has both :hover and :focus-visible styles; cite `index.html` elements (they are plain text placeholders currently).

What not to change
- Do not remove the `design/` or `assets/` content — they are the visual spec and required assets.
- Avoid restructuring the repo; keep edits to `index.html`, new CSS files, and assets only.

Integration & external dependencies
- None required. Fonts can optionally be loaded from Google Fonts, and deployments commonly use GitHub Pages / Vercel / Netlify (mentioned in README).

Agent behavior checklist (short)
1. Read `style-guide.md` and `design/*` before making styling changes.
2. Prefer adding a new CSS file and linking it; keep changes minimal and reversible.
3. Use `assets/` paths for images/fonts; do not add large external assets.
4. Ensure hover and focus states for interactive elements (explicit requirement).
5. When reporting changes, list edited/added files and one-line rationale.

If you need more context or permission to restructure the project (introduce a build step, test harness, or different layout), ask the repository owner before making large changes.

-- End of guidance --
