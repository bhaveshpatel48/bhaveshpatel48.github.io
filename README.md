# bhaveshpatel48.github.io

Personal portfolio site for **Bhavesh Vaviya** — Senior Software Engineer (Python · GenAI · Backend).

**Live:** https://bhaveshpatel48.github.io

## Files

| File | Purpose |
|------|---------|
| `index.html` | Single-page portfolio + JSON-LD structured data |
| `styles.css` | All styles (light theme, responsive, print stylesheet) |
| `script.js` | Progressive enhancement only — scroll-spy nav highlight |
| `assets/profile.svg` | **Placeholder** profile photo — replace this |
| `assets/favicon.svg` | Browser tab icon |
| `robots.txt` / `sitemap.xml` | Search engine directives |
| `.nojekyll` | Tells GitHub Pages to serve files as-is |

## Built for discoverability

The site is optimized so recruiters and sourcing tools surface it:

- **Zero-JS content** — every resume fact is in the raw HTML. Scrapers that don't run
  JavaScript still see all 900+ words and all 37 skill keywords.
- **JSON-LD `Person` schema** — machine-readable job title, employer, location, education,
  `sameAs` profile links, and a 40-entry `knowsAbout` skills list. This is what powers
  Google's knowledge panels and what many ATS/sourcing crawlers parse first.
- **Semantic HTML** — one `<h1>`, ordered heading hierarchy, `<time datetime>` on all dates.
- **SEO meta** — title (57 chars) and description (153 chars) both sized to display in full
  in search results, plus canonical URL and Open Graph tags for LinkedIn previews.
- **Print stylesheet** — recruiters who "Save as PDF" get a clean, ink-friendly document.
- **Accessible** — skip link, visible focus rings, alt text, `prefers-reduced-motion` support.

## TODO before sharing widely

1. **Replace the profile photo.** Drop a square image (600×600 or larger) at
   `assets/profile.jpg`, then update the `<img class="avatar">` `src` in `index.html`
   and the `og:image` / JSON-LD `image` URLs.
2. **Consider a resume PDF.** Add `assets/resume.pdf` and link it from the hero for
   one-click download.
3. **Submit to Google.** Add the site in
   [Search Console](https://search.google.com/search-console) and submit `sitemap.xml`
   so it gets indexed in days rather than weeks.

## Profile links

Confirmed and live in both the visible HTML and the JSON-LD `sameAs` array:

- LinkedIn — https://www.linkedin.com/in/bhavesh-vaviya/
- GitHub — https://github.com/bhaveshpatel48
- LeetCode — https://leetcode.com/u/BhaveshVaviya/
- Email — bhaveshvaviya48@gmail.com

If any of these change, update them in **both** places in `index.html`.

## Adding a project

`index.html` has a commented-out `<article class="card">` template in the
Selected Work section — copy it and fill in the details.

## Local preview

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy

Push to `main`. GitHub Pages serves the repo automatically at the URL above.
