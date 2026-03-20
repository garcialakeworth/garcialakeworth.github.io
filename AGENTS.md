## Cursor Cloud specific instructions

This is a static HTML/CSS/JS landing page ("Landed" by HTML5 UP) deployed to GitHub Pages. There is no build step, no package manager, no tests, and no linting infrastructure.

### Running the site locally

Serve the repository root with any static HTTP server:

```
python3 -m http.server 8080
```

Then open `http://localhost:8080/index.html` in a browser.

### Key points

- All JS libraries (jQuery, Scrollex, Scrolly, Dropotron) are vendored in `assets/js/` — no dependency installation is needed.
- CSS is pre-compiled at `assets/css/main.css`. Sass sources exist under `assets/sass/` but a Sass compiler is only needed when modifying styles at the `.scss` level.
- There are no automated tests, no linter configuration, and no build pipeline in this repository.
- Deployment is handled by GitHub Actions (`.github/workflows/static.yml`) which uploads the repo as-is to GitHub Pages.
