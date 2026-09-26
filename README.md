# kolakivy.github.io

Personal homepage of Qiwei Liang. Plain static HTML, no build step (`.nojekyll` keeps GitHub Pages from running Jekyll).

```
index.html            the homepage
404.html
assets/css/style.css
assets/js/main.js     Guangzhou clock + figure lightbox
assets/fonts/         self-hosted Fraunces and Nunito (latin subset)
assets/img/           portrait, 梁 mark / favicons, social preview
assets/papers/        one figure per paper (webp, ~2000px wide)
AFRO/  DQ/            project pages
```

## Adding a paper

1. Save the figure to `assets/papers/<name>.webp` (about 2000px wide is plenty).
2. In `index.html`, copy one `<li class="paper card">` block inside `<ol class="papers">`, then update the number, venue, title, authors, one-line summary, links, and figure. Cards alternate text/figure sides automatically.
3. Use `pill-coral` for the venue pill of accepted papers and `pill-soft` for preprints.

## Preview locally

```
python -m http.server 8000
```

Then open http://localhost:8000.
