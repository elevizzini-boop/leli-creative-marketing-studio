# AGENTS.md

## Architecture
A single-page static site. `netlify.toml` publishes `public/`, and there is no build step or package.json. All markup and CSS live in `public/index.html`, written as several inline `<style>` blocks, which is how the owner supplied it.

## Key directories
- `public/index.html` — the landing page. Copy is in Italian (`lang="it"`).
- `public/assets/` — original PNGs (hero, logo, photo2–4, 6, 7). The files are large (up to about 3 MB).

## Conventions and decisions
- Never reference `/assets/*.png` directly. Always go through the Image CDN: `/.netlify/images?url=/assets/<file>&w=<width>&fm=webp`. Content images use `srcset` at 600w and 1100w, plus `loading="lazy"`.
- Brand palette (CSS vars in `:root`): ink `#191816`, cream `#f2ece4`, paper `#fbf8f3`, terracotta `#a65e45`. Headings use a Baskerville serif and body text uses Avenir Next / Montserrat.
- The primary CTA is WhatsApp (`wa.me/393480825351`). The "Scopri…" links on the offer cards anchor to `#contatti`.
- The section anchors used by the nav are `#about`, `#servizi`, `#consulenze` and `#contatti`.
- Make small, targeted edits to the existing HTML and CSS rather than restructuring. The design is the owner's.
