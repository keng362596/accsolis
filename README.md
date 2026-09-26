# AccSolis Website

Static bilingual corporate site for AccSolis, hosted on GitHub Pages at https://accsolis.co.th/.

## Files

- `index.html` — Thai homepage (default language)
- `en/index.html` — English homepage
- `styles.css` — shared stylesheet (brand palette documented at the top)
- `script.js` — footer year and mobile menu
- `robots.txt`, `sitemap.xml` — crawler access and sitemap with Thai/English alternates
- `llms.txt` — plain-language company summary for AI assistants (ChatGPT, Claude, Perplexity, etc.)
- `og-image.png` — 1200×630 social sharing image

## Editing content

The Thai and English pages are maintained by hand and must stay in sync. When you change
company facts, services or FAQ answers, update **all** of these:

1. The visible text in `index.html` and `en/index.html`
2. The JSON-LD block in the `<head>` of both pages (FAQ answers must match the visible text)
3. `llms.txt`
4. `dateModified` in the JSON-LD and `<lastmod>` in `sitemap.xml`

## Brand colours

| Role  | Hex       | Use |
|-------|-----------|-----|
| Teal  | `#2fa0bd` | Primary brand colour: fills, icons, large type |
| Sun   | `#ffda54` | Highlights and primary buttons on dark backgrounds only |
| Gold  | `#d69c23` | Accent rules; text only on dark backgrounds |
| Teal 700 | `#1b7690` | Derived: links and buttons on white (WCAG AA) |
| Teal 900 | `#0e3a47` | Derived: dark sections (hero, contact, footer) |

## GitHub Pages deployment

Deploy from the `main` branch, root folder (`/`). The `CNAME` file sets the custom domain.
