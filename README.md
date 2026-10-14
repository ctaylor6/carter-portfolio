# Carter Taylor — Portfolio V2

A second portfolio website built with the [al-folio](https://github.com/alshedivat/al-folio) academic template. The original Next.js portfolio remains in [ctaylor6/carter-portfolio](https://github.com/ctaylor6/carter-portfolio).

**Site:** https://ctaylor6.github.io/Carter-Portfolio_V2/

## Content

- `_pages/about.md`: biography, profile, scrolling news, and selected publications.
- `_news/`: professional updates. `date_label` preserves month-only dates and internship ranges; `date` is a sorting key.
- `_bibliography/papers.bib`: all five publications. Only PI-TSAD has `selected = {true}`.
- `_projects/`: ten research and engineering projects with image galleries.
- `_data/socials.yml`: email, GitHub, LinkedIn, and Google Scholar.
- `_config.yml`: site metadata, theme options, and the project-site URL.

## Local preview

Use Ruby 3.3+, Bundler, Node.js, and ImageMagick.

```sh
bundle config set --local path vendor/bundle
bundle install
npm ci
bundle exec jekyll serve
```

Open `http://127.0.0.1:4000/Carter-Portfolio_V2/`.

```sh
npm run lint:prettier
bundle exec jekyll build
bundle exec al-folio upgrade audit
bundle exec al-folio upgrade overrides audit
```

The site intentionally overrides `_includes/news.liquid` to display month labels, preserve date ranges, and keep the homepage news area compact and keyboard-scrollable. The override is recorded in `.al-folio-overrides.yml`.

## Publishing

Pushes to `main` build the site and publish the generated files to `gh-pages`. GitHub Pages should use the `gh-pages` branch and `/` root. Keep `baseurl: /Carter-Portfolio_V2` for this project-site address.
