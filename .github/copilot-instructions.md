# Copilot instructions

## Build, test, lint
- No build, test, or lint commands are defined in this repository.

## High-level architecture
- GitHub Pages/Jekyll site configured by `_config.yml` (remote theme `pages-themes/cayman@v0.2.0`, site title/description, analytics).
- The main page content lives in `index.md`, which mixes Markdown and inline HTML for layout and content.
- `_layouts/default.html` overrides the theme layout and loads the theme CSS, adds a Usercentrics script, and sets the favicon.
- Styling customization is minimal: `assets/css/style.scss` only imports the selected theme.
- `project-webmap/` is a standalone static HTML page with inline CSS and its own assets; it embeds an external QGIS Cloud map.
- Static assets are organized in `img/`, `downloads/`, and `project-webmap/` (with its own SVGs).

## Key conventions
- Page content is predominantly in German; keep new content consistent with that language.
- Prefer editing `index.md` for homepage content; it intentionally uses raw HTML for layout alongside Markdown.
- Keep the Jekyll theme usage via `_config.yml` and the minimal `assets/css/style.scss` import pattern.
- The web map page is independent of the Jekyll layout; changes there are made directly in `project-webmap/index.html` with inline styles and relative assets.
