# confox.github.io

Personal portfolio site for [Turkish](https://github.com/confox) — cybersecurity researcher and solo developer at [@D4rk-Wolf](https://github.com/D4rk-Wolf).

**Live site → [confox.github.io](https://confox.github.io)**

---

## Stack

Static HTML/CSS — no framework, no build step. Hosted on GitHub Pages.

| File | Purpose |
|------|---------|
| `index.html` | Single-page portfolio |
| `stylesheet.css` | All styles — dark theme, responsive |
| `_config.yml` | Jekyll config (GitHub Pages metadata) |

**Fonts:** Inter + JetBrains Mono (Google Fonts)  
**Icons:** Font Awesome 6.5

---

## Featured Projects

### [AI Document Generator](https://confox.github.io/AI-Document-Generator/)
Browser-based and desktop tool for generating the 10 essential AI project documents. Built with React 19, Vite, and Tauri. Deployed via its own [GitHub Actions workflow](https://github.com/confox/AI-Document-Generator/blob/main/.github/workflows/pages.yml).

### [ByeBye](https://github.com/confox/ByeBye)
Python script for securely overwriting and deleting drive data.

---

## Development

No build process — edit and push.

```bash
git clone https://github.com/confox/confox.github.io
cd confox.github.io

# Preview locally (optional)
python3 -m http.server 8080
# → http://localhost:8080
```

Changes pushed to `main` are deployed automatically by GitHub Pages.

---

## Adding a Project

Add a new `.project-card` block inside the `projects-grid` section in `index.html`:

```html
<div class="project-card">
    <div class="project-header">
        <div class="project-icon-wrap"><i class="fas fa-icon-name"></i></div>
        <h3>Project Name</h3>
    </div>
    <p>Short description.</p>
    <div class="project-footer">
        <span class="lang-tag"><span class="lang-dot js"></span>JavaScript</span>
        <a href="https://github.com/confox/repo" class="project-link" target="_blank">
            View on GitHub <i class="fas fa-arrow-right"></i>
        </a>
    </div>
</div>
```

Available `lang-dot` colours: `.js` (yellow), `.python` (blue). Add more in `stylesheet.css` under `.lang-dot`.

---

## License

Site code is MIT. Project content and branding belong to Turkish / D4rkwolf Studios.
