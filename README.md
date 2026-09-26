# kolakivy.github.io

Personal homepage of Qiwei Liang. Plain static HTML, no build step (`.nojekyll` keeps GitHub Pages from running Jekyll).

```
index.html            the homepage
404.html
assets/css/style.css
assets/js/main.js     top bar divider on scroll + figure lightbox
assets/fonts/         self-hosted Figtree (latin subset)
assets/img/           portrait, 梁 mark / favicons, social preview
assets/papers/        one figure per paper (webp, ~2000px wide)
AFRO/  DQ/            project pages
```

## Adding a paper

1. Save the figure to `assets/papers/<name>.webp` (about 2000px wide is plenty).
2. In `index.html`, copy one `<li class="pub">` block inside `<ul class="pubs">`, then update the figure, title, authors, venue, and links.
3. Use `class="badge badge-pub"` for accepted papers and plain `class="badge"` for preprints.

## Preview locally

```
python -m http.server 8000
```

Then open http://localhost:8000.
