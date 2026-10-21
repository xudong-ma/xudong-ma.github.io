# xudong-ma.github.io

Personal academic homepage of **Xudong Ma** — https://xudong-ma.github.io

Built with the [al-folio](https://github.com/alshedivat/al-folio) Jekyll theme (MIT licence).

## Where to edit things

| What                        | File                                                                     |
| --------------------------- | ------------------------------------------------------------------------ |
| Bio, research interests, service | `_pages/about.md`                                                  |
| Publications                | `_bibliography/papers.bib` (`selected = {true}` puts a paper on the home page) |
| Paper thumbnails            | add `preview = {name.png}` to a bib entry and put the image in `assets/img/publication_preview/` |
| News                        | one Markdown file per item in `_news/`                                   |
| Email / Scholar / GitHub icons | `_data/socials.yml`                                                   |
| Venue badge colours         | `_data/venues.yml`                                                       |
| Profile photo               | `assets/img/prof_pic.jpg`                                                |
| Site-wide settings          | `_config.yml`                                                            |

`_includes/news.liquid` is a local override of the theme file (shows news dates as month + year); it is recorded in `.al-folio-overrides.yml`.

## Deploying

Every push to `main` runs `.github/workflows/deploy.yml`, which builds the site and publishes it to the `gh-pages` branch. In the repository's **Settings → Pages**, set the source to **Deploy from a branch → `gh-pages` / `(root)`** (one-time).

## Local preview

```bash
bundle install
bundle exec jekyll serve      # http://localhost:4000
```

or with Docker: `docker compose up` (http://localhost:8080).
