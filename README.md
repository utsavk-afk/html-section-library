# HTML Section Library

A free library of **self-contained landing-page sections** — heroes, pricing, FAQs, testimonials, footers and more — each built in **five distinct styles**. No build step, no dependencies, no framework. Copy one file and drop it into Claude Code.

Every section is a single `index.html`: inline CSS with `:root` design tokens, Google Fonts, and CSS/inline-SVG visuals (no external images). Rebrand any section by changing the tokens at the top.

---

## Browse

Open **`gallery.html`** in a browser. Filter by **type** and **style**, search, and click any card to open the live section.

## The five styles

| Style | Look |
|---|---|
| **editorial** | Light, refined serif (Fraunces), tracked labels, deep whitespace, one warm accent |
| **brutalist** | Black + acid-yellow, heavy grotesk, thick borders, hard offset shadows, uppercase |
| **dark** | Near-black, off-white, one amber accent, quiet and premium (no glow) |
| **minimal** | White, one restrained accent, hairline rules, lots of space |
| **acid-pop** | Near-black, oversized type, lime + magenta, bold and flat |

## How to use it in Claude Code

**Option A — grab a finished section**
1. Find one you like in the gallery.
2. Open its `sections/<type>/<type>--<style>/index.html`.
3. Copy the file into your project. Change the copy and the `:root` tokens to match your brand. Done.

**Option B — generate your own in a matching style**
1. Open the style spec you want in **`styles/`** (e.g. `styles/brutalist.md`).
2. Paste the whole file into Claude Code.
3. Say: *"Build me a `<section type>` section in this exact style."*

Claude will return a self-contained section that matches the look — same tokens, same rules, same anti-slop guardrails.

## Structure

```
html-section-library/
  gallery.html          filterable, searchable index
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
