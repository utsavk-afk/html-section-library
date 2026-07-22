# Style: Editorial  (`editorial`)

Paste this whole file into Claude Code, then say: **"Build me a &lt;section type&gt; section in this exact style."**
Claude will produce a self-contained HTML section matching the look.

## Design tokens (`:root`)
```css
:root{
  --bg:#FCFCFA; --ink:#1B1A17; --muted:#6C6A63; --line:#E7E4DC; --accent:#B4472B;
--serif:'Fraunces',Georgia,serif; --sans:'Inter',system-ui,sans-serif;
}
```

## Look & rules
Refined serif display (Fraunces) + Inter body. Small UPPERCASE tracked labels (letter-spacing .24em). Deep whitespace, hairline rules. One warm ink accent, italic serif for emphasis words. Calm, premium, print-like.

## Anti-AI-slop guardrails (apply to every section)
- No default purple/indigo->cyan gradient, no glassmorphism/frosted glow, no floating 3D blobs.
- No identical icon-tile card grid with uniform radius + uniform soft shadow. Vary card size/weight.
- No stock-smile faces (use CSS initial-avatars or inline SVG). No cream/"ChatGPT beige" reflex background.
- No everything-centered symmetry — establish one focal point, use asymmetry.
- Vary radius, spacing, elevation deliberately. One intentional accent, not rainbow.
- No generic "Elevate your workflow / all-in-one platform" copy. Write a specific verb + noun.
- Self-contained: inline CSS in <style>, :root tokens, no build step, no external JS libs, no external images (CSS/inline-SVG only). Google Fonts allowed.

## Output contract
One complete `<!DOCTYPE html>` file: `<head>` (Google Fonts link ok) + `<style>` (`:root` tokens above, then component CSS) + one full-width responsive section in `<body>` with a `@media(max-width:640px)` block. Real, specific placeholder copy. Lead the file with a comment `/* ===== <TYPE> — Editorial ===== */`.
