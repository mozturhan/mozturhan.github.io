# Munir Ozturhan — Academic Website

A static academic website built with plain HTML/CSS — no build step, no frameworks.
Works directly on GitHub Pages.

## Pages

- `index.html` — Home: about, three core projects, news
- `research.html` — Research program + detailed project descriptions
- `publications.html` — Journal articles and selected presentations
- `teaching.html` — Instructor-of-record courses, TA roles, mentoring
- `cv.html` — Embedded + downloadable CV (PDF at `assets/Munir_Ozturhan_CV.pdf`)
- `assets/style.css` — Shared stylesheet

## Deploy to GitHub Pages (personal site at munirozturhan.github.io)

1. Create a GitHub account if you don't have one, then create a **new public
   repository** named exactly `YOURUSERNAME.github.io`
   (e.g., `munirozturhan.github.io`).
2. Upload all files in this folder to the repository, keeping the folder
   structure (the `assets/` folder must stay next to the HTML files).
   Easiest way: on the repo page, click **Add file → Upload files**, drag
   everything in, and commit.
3. Go to the repository's **Settings → Pages**. Under "Build and deployment",
   Source should be **Deploy from a branch**, Branch: `main`, folder `/ (root)`.
4. Wait 1–2 minutes. Your site is live at `https://YOURUSERNAME.github.io`.

Any time you edit a file and commit, the site updates automatically within a
minute or two.

## Customizing

- **Photo**: add `assets/photo.jpg` (a portrait-orientation headshot), then in
  `index.html` replace the placeholder `<div class="photo-placeholder">` with
  `<img class="photo" src="assets/photo.jpg" alt="Munir Ozturhan">`.
- **Updating the CV**: replace `assets/Munir_Ozturhan_CV.pdf` with a newer file
  of the same name — both the embed and the download button will update.
- **News**: add a new `.news-item` block at the top of the News section in
  `index.html`.
- **OSF / Google Scholar / ORCID links**: uncomment and fill in the links in
  the footer of `index.html`, and replace the `#` placeholder links on the
  feature-reassembly entry in `publications.html` with your actual OSF URLs.
- **After your defense**: change "Ph.D. candidate" wording on `index.html` and
  the dissertation "Under review"/project statuses as things get published.

## Colors and fonts

Defined at the top of `assets/style.css` as CSS variables (`--cobalt`,
`--teal`, `--amber`, etc.) — change them in one place to re-theme the site.
Fonts (Spectral, Source Sans 3, IBM Plex Mono) load from Google Fonts.
