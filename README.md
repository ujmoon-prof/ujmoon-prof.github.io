# Ui Jeong Moon academic website

A bilingual English/Korean static academic website prepared for **https://ujmoon-prof.github.io/**.

## Deploy to GitHub Pages

1. Open https://github.com/ujmoon-prof/ujmoon-prof.github.io
2. Upload `index.html`, `styles.css`, `app.js`, and `publications.json` to the **root** of the repository (not inside a `ujmoon-site` folder).
3. Commit the changes to the `main` branch.
4. In **Settings > Pages**, select **Deploy from a branch**, `main`, `/ (root)`, then Save.
5. Allow a few minutes and open https://ujmoon-prof.github.io/.

No build step, paid service, or package installation is required. The site loads Google Fonts from the web; system fonts are used as fallback.

## Edit content

- Homepage and sections: `index.html`
- English/Korean interface text: `app.js`, `i18n` object
- Publications: `publications.json` (one record per paper; newest first)
- Visual styling: `styles.css`

## Content notes

Source: https://sites.google.com/view/ujmoon (reviewed November 3, 2026).

- All 31 publications were transcribed from the source page; one 2013 item has no URL on the source.
- Korean titles remain untranslated to avoid presenting unofficial English titles as published titles.
- Research themes are editorial summaries inferred from publication topics, not confirmed active research projects.
- Credentials are summarized; the original page contains the full list.
- The public phone number was deliberately omitted from this design to reduce exposure; the listed professional email is retained.
- No portrait or photographs are included because none were supplied or licensed for reuse.
- Please confirm biographical details, citations, affiliations, and consent before announcing the site as official.

## Local preview

Because the publication list is fetched from `publications.json`, use a local HTTP server rather than opening `index.html` directly:

```bash
python -m http.server 8000
```

Visit http://localhost:8000.
