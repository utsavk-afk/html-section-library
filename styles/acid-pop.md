# Style: Acid Pop  (`acid-pop`)

Paste this whole file into Claude Code, then say: **"Build me a &lt;section type&gt; section in this exact style."**
Claude will produce a self-contained HTML section matching the look.

## Design tokens (`:root`)
```css
:root{
  --bg:#0A0A0A; --ink:#F5F5F5; --lime:#C7F13B; --magenta:#FF4D9D; --line:#222;
--sans:'Archivo',Arial,sans-serif;
}
```

## Look & rules
Near-black background, OVERSIZED heavy type, lime primary accent with a magenta secondary. Bold, energetic, playful. Big letter-spacing-tight headlines, chunky pill buttons, one loud moment per section. Not neon-glow — flat bold color.

## Anti-AI-slop guardrails (apply to every section)
- No default purple/indigo->cyan gradient, no glassmorphism/frosted glow, no floating 3D blobs.
- No identical icon-tile card grid with uniform radius + uniform soft shadow. Vary card size/weight.
- No stock-smile faces (use CSS initial-avatars or inline SVG). No cream/"ChatGPT beige" reflex background.
- No everything-centered symmetry — establish one focal point, use asymmetry.
- Vary radius, spacing, elevation deliberately. One intentional accent, not rainbow.
- No generic "Elevate your workflow / all-in-one platform" copy. Write a specific verb + noun.
- Self-contained: inline CSS in <style>, :root tokens, no build step, no external JS libs, no external images (CSS/inline-SVG only). Google Fonts allowed.

## Output contract
One complete `<!DOCTYPE html>` file: `<head>` (Google Fonts link ok) + `<style>` (`:root` tokens above, then component CSS) + one full-width responsive section in `<body>` with a `@media(max-width:640px)` block. Real, specific placeholder copy. Lead the file with a comment `/* ===== <TYPE> — Acid Pop ===== */`.
