# LELI — Creative Marketing Studio

Landing page for LELI Creative Marketing Studio by Eleonora Vizzini, marketing strategist and project manager. The page is in Italian. It presents her approach, services, method and the four ways clients can work with her (Focus, Content, Social, 360°). Visitors reach her by WhatsApp, email, Instagram or LinkedIn.

## Technologies

- Static HTML and CSS, with no framework or build step
- Netlify hosting
- Netlify Image CDN, which resizes the photos and serves them as WebP

## Run locally

```bash
netlify dev
```

You can also open `public/index.html` directly, but the images only load when the Netlify Image CDN is available (`netlify dev` or a deploy).

## Structure

- `public/index.html` — the whole landing page, with inline styles
- `public/assets/` — the original photos and logo
- `netlify.toml` — publish directory and cache headers
