# williamnash.github.io

Personal site, built by GitHub Pages from `master` with Jekyll. No theme gem: the layout lives in `_layouts/`, `_includes/` and `public/css/site.css`.

- Pages: `index.html` (home), `professional.md` (Work), `writing.md`, `personal.md`
- Posts: `_posts/`; the permalink in `_config.yml` keeps the original `/posts/YYYY-M-D-slug/` URLs
- Contact links, and whether a Resume link shows, are set under `author` and `resume` in `_config.yml`
- Photos: keep them at most 2000 px on the long edge (`sips -Z 2000 -s formatOptions 80 photo.jpg`), with lowercase extensions, since Pages is case-sensitive

Preview locally: `jekyll serve` (Jekyll 3.9, as GitHub Pages runs), then open http://localhost:4000.

Layout originally adapted from [Hyde](https://github.com/poole/hyde) by Mark Otto (MIT, see `LICENSE.md`).
