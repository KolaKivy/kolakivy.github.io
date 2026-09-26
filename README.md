# kolakivy.github.io

Personal homepage of Qiwei Liang. Plain static HTML, no build step (`.nojekyll` keeps GitHub Pages from running Jekyll).

```
index.html            the homepage
404.html
assets/css/style.css
assets/js/main.js     Guangzhou clock + figure lightbox
assets/fonts/         self-hosted Newsreader and JetBrains Mono (latin subset)
assets/img/           portrait, seal, favicons, social preview
assets/papers/        one figure per paper (webp, ~2000px wide)
AFRO/  DQ/            project pages
```

## Adding a paper

1. Save the figure to `assets/papers/<name>.webp` (about 2000px wide is plenty).
2. In `index.html`, copy one `<li class="paper">` block inside `<ol class="papers">`, then update the number, venue, title, authors, one-line summary, links, and figure.
3. Use `class="venue is-pub"` for accepted papers and plain `class="venue"` for preprints.

## Preview locally

```
python -m http.server 8000
```

Then open http://localhost:8000.
