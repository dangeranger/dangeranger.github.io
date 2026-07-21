# dangeranger.github.io

My personal site — a single-page profile served from GitHub Pages at
[dangeranger.github.io](https://dangeranger.github.io).

It's plain HTML and CSS. No build step, no framework, no JavaScript beyond a
one-liner that stamps the current year in the footer. If you can open a file in
a browser, you can run it.

## What's in here

```
index.html          The whole page: intro, current work, experience, links
assets/css/site.css  Styles — dark GitHub-ish theme, CSS variables up top
images/avatar.jpg    Profile photo
.nojekyll            Tells GitHub Pages to skip Jekyll and serve files as-is
.gitignore
LICENSE.txt
```

## Running it locally

Just open `index.html` in a browser. That's it.

If you'd rather serve it over HTTP (closer to how Pages actually serves it):

```sh
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploying

GitHub Pages builds from the `main` branch. Push to `main` and the live site
updates on its own — there's nothing to build.

## Editing notes

- Content lives directly in `index.html`. Edit the markup; there's no template
  layer or data file.
- Theme colors are CSS variables at the top of `site.css` (`--bg`, `--accent`,
  and friends) — change them there instead of hunting through the file.
- The footer year comes from a small inline script at the bottom of
  `index.html`, so it stays current without any edits.
