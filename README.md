# srrezaei.github.io

Personal academic website for Seyedreza Rezaei, built on the
[al-folio](https://github.com/alshedivat/al-folio) Jekyll starter (v1.x).

Live at <https://srrezaei.github.io>.

## How it deploys

Pushing to `main` triggers `.github/workflows/deploy.yml`, which installs Ruby, builds the site
with Jekyll, purges unused CSS, and pushes the result to the `gh-pages` branch. GitHub Pages serves
`gh-pages`. **You do not need Ruby installed locally to publish** — only to preview.

Set this once on GitHub: **Settings → Pages → Source: Deploy from a branch → `gh-pages` / `(root)`**.

## Where the content lives

| What | File |
| --- | --- |
| Name, description, URL, theme options | `_config.yml` |
| Bio and profile sidebar | `_pages/about.md` |
| Publications | `_bibliography/papers.bib` |
| CV | `_data/cv.yml` (rendered) and `assets/pdf/CV_Seyedreza_Rezaei.pdf` (download) |
| News / timeline items | `_news/*.md` — one file per item |
| Projects | `_projects/*.md` — one file per project |
| Social links | `_data/socials.yml` |
| Co-author links in the bibliography | `_data/coauthors.yml` |
| Venue links and badge colours | `_data/venues.yml` |
| Profile photo | `assets/img/prof_pic.jpg` |

### Adding a publication

Append a BibTeX entry to `_bibliography/papers.bib`. Useful extra fields al-folio understands:
`abbr`, `abstract`, `selected` (shows it on the homepage), `bibtex_show`, `pdf`, `arxiv`, `code`,
`video`, `html`, `preview` (a thumbnail in `assets/img/publication_preview/`), and
`additional_info`.

### Adding a news item

Copy any file in `_news/`. `inline: true` renders it as a one-liner in the homepage timeline.

### Adding a project

Copy any file in `_projects/`. `importance` sets the ordering, `category` must be one of the values
in `display_categories` in `_pages/projects.md` (currently `research` and `engineering`), and `img`
gives the card a thumbnail.

## Previewing locally

Requires Ruby plus build tools. On WSL Ubuntu, once:

```bash
sudo apt update && sudo apt install -y ruby-dev build-essential zlib1g-dev imagemagick
```

Then, from the repo:

```bash
bundle install && bundle exec jekyll serve
```

The site is served at <http://localhost:4000>. (`baseurl` is blank in `_config.yml`, since this is
a user site served from the domain root — do not add the `/al-folio` baseurl the upstream theme
uses for its demo.)

Docker is the alternative if you would rather not install Ruby: `docker compose up`.

## Notes on this copy

Trimmed from the upstream starter: the theme's own CI workflows (only `deploy.yml` is kept), its
docs and tests, its agent-instruction files, its demo blog posts, books and teaching collections,
and ~19 MB of demo images. The `static-site` branch holds an earlier hand-written version of this
site, kept for reference.
