# Publishing the library (GitHub + Notion)

The whole library lives in this folder. Two ways to share it publicly.

---

## A. GitHub (recommended for Claude Code users)

One-command clone for anyone; you push once.

```bash
cd C:/Users/khamb/html-section-library
git init
git add .
git commit -m "HTML Section Library — ~300 sections across 5 styles"
gh repo create html-section-library --public --source=. --push
```

That creates the public repo and pushes. Users then:

```bash
git clone https://github.com/<you>/html-section-library
# open gallery.html, or copy any sections/<type>/<type>--<style>/index.html
```

The public link is the repo URL. `gallery.html` renders on GitHub Pages too if you enable Pages (Settings → Pages → deploy from `main` / root).

---

## B. Notion (visual gallery + public page)

There's no Notion API connector wired here, so this part is a short manual setup — but I've generated everything you need.

1. In Notion, create a new **Table** database → switch its layout to **Gallery**.
2. **Import the data:** `Import → CSV → notion-import.csv` (in this folder). It creates a row per section with **Name, Type, Style** properties.
3. **Card preview = screenshot:** add a **Files & media** property called `Preview`, then drag each `sections/<dir>/screenshot.png` onto its row (or bulk-upload). Set the gallery **Card preview** to `Preview`.
4. **Filters:** the Type and Style columns become instant filter/group options — exactly the filtering you wanted.
5. **Public link:** top-right **Share → Publish → Publish to web**. That URL is your public library.
6. (Optional) In each row, paste the section's raw HTML or link to the GitHub file so people can copy it from Notion.

**Tip:** if you did path A first, you can skip step 3 — instead add a `HTML` URL property in the CSV pointing at each GitHub file, so Notion is the pretty front-door and GitHub is the download.

---

## What's in the box
- `gallery.html` — filterable/searchable index (open locally)
- `styles/*.md` — 5 paste-into-Claude style specs
- `sections/<type>/<type>--<style>/` — `index.html` + `screenshot.png` + `meta.json`
- `manifest.json` — machine-readable list of every section
- `notion-import.csv` — ready to import (generated)
- `README.md` — how to use it
