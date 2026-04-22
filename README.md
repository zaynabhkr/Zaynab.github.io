# Zaynab's Portfolio – Quarto Website

A personal portfolio site built with [Quarto](https://quarto.org), deployed via GitHub Pages.

## Structure

```
zaynab-portfolio/
├── _quarto.yml        # Site config & navbar
├── custom.scss        # Color palette, fonts, components
├── index.qmd          # Home / landing page
├── resume.qmd         # Resume page
├── cover-letter.qmd   # Cover letter (customizable template)
└── project.qmd        # Team ML project page
```

## Local Development

```bash
# Preview the site locally (live reload)
quarto preview
```

## Deploy to GitHub Pages

### First-time setup
1. Push this folder as a GitHub repo.
2. In `_quarto.yml`, `output-dir: docs` is already set — this is what GitHub Pages needs.
3. Run:
   ```bash
   quarto render
   git add docs/
   git commit -m "Build site"
   git push
   ```
4. In your repo → **Settings → Pages → Source: Deploy from branch → `main` → `/docs`**.

### On every update
```bash
quarto render
git add -A
git commit -m "Update site"
git push
```

## Customization Checklist

- [X] **`index.qmd`** – Update skills pills to match yours
- [X] **`resume.qmd`** – Fill in real university, GPA, experience, and project details; swap `href="#"` on Download button for a real PDF link
- [X] **`cover-letter.qmd`** – Highlighted placeholders guide what to personalize per application
- [X] **`project.qmd`** – Replace project title, description, teammates, roles, and progress %
- [X] **`_quarto.yml`** – Update GitHub/LinkedIn links in the navbar
- [X] **`custom.scss`** – Tweak colors in `:root` variables to change the whole palette
