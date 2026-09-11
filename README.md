# manuelweiss.info

Source of the academic website of Manuel Weiss, published at **[manuelweiss.info](https://manuelweiss.info)**.

The site is built with [Jekyll](https://jekyllrb.com) on the [Academic Pages](https://github.com/academicpages/academicpages.github.io) theme and deployed with GitHub Pages.

## Where things live

| Path | Content |
|------|---------|
| `_config.yml` | Site settings, sidebar profile and social links |
| `_data/navigation.yml` | Top navigation menu |
| `_pages/` | Home page (`about.md`, including News), Projects, Publications, Teaching, 404 |
| `_publications/` | One file per paper |
| `_teaching/` | One file per course |
| `images/` | Images, video and favicons |
| `files/` | Downloads such as a CV (served at `/files/<name>`) |
| `_sass/_custom.scss` | Site-specific styles on top of the theme |

The theme itself lives in `_layouts/`, `_includes/`, `_sass/` and `assets/`.

## Adding a publication

Create `_publications/YYYY-MM-DD-short-slug.md`:

```yaml
---
title: "Paper title"
collection: publications
pub_type: journal        # or: conference
date: 2026-01-14
venue: "Journal or conference name"
paperurl: "https://doi.org/..."
citation: 'A. Author, <b>M. Weiss</b> and B. Author, "Paper title," <i>Venue</i>, 2026.'
---
```

It shows up on `/publications/` automatically, grouped by `pub_type` and sorted by date.

## Local preview

Requires Ruby and Bundler.

```sh
bundle install
bundle exec jekyll serve -l
```

Then open <http://localhost:4000>. Pages rebuild on save; restart the server after editing `_config.yml`.

## Deployment

Pushing to `main` triggers the GitHub Pages build. The custom domain is configured in `CNAME`.

## License

The theme code comes from [Academic Pages](https://github.com/academicpages/academicpages.github.io) and [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes) and is released under the MIT License (see `LICENSE`). The site content (text, images and video) is © Manuel Weiss and is not covered by that license.
