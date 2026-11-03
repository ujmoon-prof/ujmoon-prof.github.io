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

- The publication list contains 31 entries; the 2013 item has no URL.
- Korean titles remain untranslated to avoid presenting unofficial English titles as published titles.
- Research themes are editorial summaries inferred from publication topics, not confirmed active research projects.
- All seven professional credentials are included; two are visible by default and five expand on request.
- The public phone number was deliberately omitted from this design to reduce exposure; the listed professional email is retained.
- No portrait or photographs are included because none were supplied or licensed for reuse.
- Please confirm biographical details, citations, affiliations, and consent before announcing the site as official.

## Local preview

Because the publication list is fetched from `publications.json`, use a local HTTP server rather than opening `index.html` directly:

```bash
python -m http.server 8000
```

Visit http://localhost:8000.


## v1.3
- Added a supplied profile portrait on the home page (`profile-photo.png`).
- Preserved Korean-first display and expandable professional credentials.
- Corrected language dictionaries for expanded credential labels.

Version 1.4: Reduced portrait size and placed research focus panel beside it for a smoother, balanced hero layout on desktop and mobile.

## v1.5 changes
- Moved the portrait from the hero to About (01), with text wrapping and responsive sizing.
- Credentials use one toggle label that changes between View all/Hide (English) and 전체 자격 보기/전체 자격 접기 (Korean).


Version 1.6: Language selector order is 한국어 then EN. Credential disclosure labels are Show more / Show less in both language modes.

Version 1.7: About portrait is in a responsive grid, with a controlled crop and no text float.


v1.8: On phones (580px and below), About displays a compact portrait alongside the name and affiliation, with the full introduction underneath. Desktop and tablet About layout is unchanged. Upload index.html, styles.css, and app.js.
