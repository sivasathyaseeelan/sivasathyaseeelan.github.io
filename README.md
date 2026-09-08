# sivasathyaseeelan.github.io

Academic website of Siva Sathyaseelan D N, built with Jekyll from the
[academic-website-template](https://github.com/sbryngelson/academic-website-template).

## Editing

| What | Where |
|------|-------|
| Name, links, accent colour, navbar pages | `_config.yml` |
| Publications | `assets/ref.bib` (BibTeX; `selected = {true}` shows an entry on the home page) |
| Research and work experience | `_data/experience.yml` |
| News, awards, achievements, software, teaching | `_data/*.yml` |
| Page text | `_pages/*.md` |
| Photo | `images/headshot.jpg` |
| CV | put `cv.pdf` in `papers/` and set `links.cv: "papers/cv.pdf"` |

## Local preview

```bash
bundle install
bundle exec jekyll serve   # http://localhost:4000
```

## Deployment

Pushing to the `source` branch runs `.github/workflows/deploy.yml`, which builds
the site and publishes it to GitHub Pages.
