# Style: Dark / Luxe  (`dark`)

Paste this whole file into Claude Code, then say: **"Build me a &lt;section type&gt; section in this exact style."**
Claude will produce a self-contained HTML section matching the look.

## Design tokens (`:root`)
```css
:root{
  --bg:#121216; --panel:#1A1A20; --ink:#F4F4F5; --muted:#A1A1AA; --line:#2A2A33; --accent:#F59E42;
--sans:'Inter',system-ui,sans-serif; --serif:'Fraunces',Georgia,serif;
}
```

## Look & rules
Near-black background, off-white text, one warm amber accent. NO glow. Refined grotesk with optional serif headline. High contrast, generous spacing, subtle 1px panel borders (not shadows). Premium and quiet.

## Anti-AI-slop guardrails (apply to every section)
- No default purple/indigo->cyan gradient, no glassmorphism/frosted glow, no floating 3D blobs.
- No identical icon-tile card grid with uniform radius + uniform soft shadow. Vary card size/weight.
- No stock-smile faces (use CSS initial-avatars or inline SVG). No cream/"ChatGPT beige" reflex background.
- No everything-centered symmetry — establish one focal point, use asymmetry.
- Vary radius, spacing, elevation deliberately. One intentional accent, not rainbow.
- No generic "Elevate your workflow / all-in-one platform" copy. Write a specific verb + noun.
- Self-contained: inline CSS in <style>, :root tokens, no build step, no external JS libs, no external images (CSS/inline-SVG only). Google Fonts allowed.

## Output contract
One complete `<!DOCTYPE html>` file: `<head>` (Google Fonts link ok) + `<style>` (`:root` tokens above, then component CSS) + one full-width responsive section in `<body>` with a `@media(max-width:640px)` block. Real, specific placeholder copy. Lead the file with a comment `/* ===== <TYPE> — Dark / Luxe ===== */`.
