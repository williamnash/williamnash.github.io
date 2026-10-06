# williamnash.github.io

Personal site, built by GitHub Pages from `master` with Jekyll. No theme gem: the layout lives in `_layouts/`, `_includes/` and `public/css/site.css`.

- Pages: `index.html` (home), `professional.md` (Work), `writing.md`, `personal.md`
- Layout: a sticky sidebar (`_includes/sidebar.html`) beside one reading column; colours are tokens at the top of `public/css/site.css`
- Dated lists use `<ul class="rows">` with `<li class="row"><span class="when">…</span>…</li>`; kramdown definition lists render the same way
- Posts: `_posts/`; the permalink in `_config.yml` keeps the original `/posts/YYYY-M-D-slug/` URLs
- Contact links, and whether a Resume link shows, are set under `author` and `resume` in `_config.yml`
- Link-preview image: `images/og.png` (1200×630), rendered from `_tools/og.html` with headless Chrome at 1200×630. Regenerate it if the name, title, colours or domain change
- Photos: keep them at most 2000 px on the long edge (`sips -Z 2000 -s formatOptions 80 photo.jpg`), with lowercase extensions, since Pages is case-sensitive

Preview locally: `jekyll serve` (Jekyll 3.x; GitHub Pages runs 3.10), then open http://localhost:4000.

Layout originally adapted from [Hyde](https://github.com/poole/hyde) by Mark Otto (MIT, see `LICENSE.md`).
