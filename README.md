# HTML Section Library

A free library of **305 self-contained landing-page sections** — heroes, pricing, FAQs, testimonials, footers and 57 more types — each in **five distinct styles** (editorial, brutalist, dark, minimal, acid-pop). No build step, no dependencies, no framework. Copy one file and drop it into Claude Code.

Every section is a single `index.html`: inline CSS with `:root` design tokens, Google Fonts, and CSS/inline-SVG visuals (no external images). Rebrand any section by changing the tokens at the top.

---

## Quick start

```bash
git clone https://github.com/utsavk-afk/html-section-library
cd html-section-library
```

Then open **`gallery.html`** in your browser to browse everything.

---

## Use it in Claude Code

**1. Browse the gallery.** Open `gallery.html` — filter by **type** and **style**, search, and click any card to open the live section. (If you enable GitHub Pages, it's also live at `https://utsavk-afk.github.io/html-section-library/gallery.html`.)

**2. Use a section — two ways:**

- **Point Claude at it (easiest).** With the repo in your workspace, just tell Claude Code:
  > "Use the `pricing--dark` section from html-section-library — drop it into my page and change the `:root` tokens to my brand colours."

  Claude reads `sections/pricing/pricing--dark/index.html` and adapts it to your project.

- **Copy the file.** Grab `sections/<type>/<type>--<style>/index.html`, paste it into your project, and edit the copy + the `:root` tokens at the top. Done — it works with zero setup.

**3. Generate NEW sections in a style.** Open a style spec in **`styles/`** (e.g. `styles/brutalist.md`), paste the whole file into Claude Code, and say:
  > "Build me a `<section type>` section in this exact style."

Claude returns a self-contained section matching the tokens, rules, and anti-slop guardrails of that style.

---

## The five styles

| Style | Look |
|---|---|
| **editorial** | Light, refined serif (Fraunces), tracked labels, deep whitespace, one warm accent |
| **brutalist** | Black + acid-yellow, heavy grotesk, thick borders, hard offset shadows, uppercase |
| **dark** | Near-black, off-white, one amber accent, quiet and premium (no glow) |
| **minimal** | White, one restrained accent, hairline rules, lots of space |
| **acid-pop** | Near-black, oversized type, lime + magenta, bold and flat |

## Structure

```
html-section-library/
  gallery.html          filterable, searchable index — start here
  manifest.json         every section (type, style, path)
  styles/               paste-into-Claude style specs (x5)
  sections/
    <type>/
      <type>--<style>/
        index.html      the section (copy this)
        screenshot.png  preview
        meta.json       type / style / name
```

## Built to not look AI-generated

Every section follows a strict anti-slop checklist: no default purple gradients, no glassmorphism, no identical icon-card grids, no stock-smile faces, no reflex beige backgrounds, no everything-centered symmetry. Real hierarchy, one intentional accent, deliberate spacing.

## License

Free to use in personal and client work. Attribution appreciated, not required.
