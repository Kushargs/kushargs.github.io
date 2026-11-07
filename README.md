# Kushagra Garg's website

A minimal academic homepage built with Jekyll. It uses system fonts and plain CSS,
with no JavaScript required.

## Editing

- `index.md`: introduction, background, and contact text.
- `_data/publications.yml`: publication titles, authors, venues, and links.
- `assets/css/main.css`: responsive layout and photo framing.
- `images/kushagra-portrait.jpeg`: selected portrait with a softened background.
- `cv/kushagra_cv.pdf`: the CV download.

Jekyll's post support can be used for a future blog. Add navigation when the first
posts or notes are ready to publish.

## Local preview

With a current Ruby and Bundler installed:

```sh
bundle install
bundle exec jekyll serve --destination ../website-preview/site --host 127.0.0.1 --port 4173
```

The destination above keeps preview output separate from the repository's legacy
tracked `_site` directory. The source files remain compatible with GitHub Pages.
