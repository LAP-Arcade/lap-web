# lap-web

Website for **Le LAP**.

Live site: <https://lelap.in>

## How it works

This is a **static site** generated with
[sssimp](https://github.com/Tina-otoge/sssimp), a small Jinja-based static site
generator. The build combines:

- **Templates & assets** in `input/content/` — HTML files are rendered as Jinja2
  templates, everything else is copied as-is.
- **Data** in `input/data/` — YAML files exposed to templates through the `data`
  variable. The folder hierarchy becomes the object hierarchy, e.g.
  `input/data/contests/contest2.yml` is available as `data.contests.contest2`.

The generated site is written to `output/` (git-ignored).

## Getting started

### Prerequisites

- Python 3
- [pipx](https://pipx.pypa.io/) (recommended) or pip

### Install the generator

```bash
pipx install sssimp
# or: pip install --user sssimp
```

### Build the site

From the project root:

```bash
sssimp
```

This reads `input/` and generates the site into `output/`.
