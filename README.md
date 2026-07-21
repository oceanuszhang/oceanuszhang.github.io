# oceanuszhang.github.io

Personal academic portfolio and blog for **Oceanus (Zhuoyang) Zhang**, PhD student in Computational Biology at UC Merced.

🔗 Live site: [https://oceanuszhang.github.io/](https://oceanuszhang.github.io/)

## Built With

This site is built on [al-folio](https://github.com/alshedivat/al-folio), a Jekyll theme for academics, running on Jekyll 4.x with Ruby, Python (Jupyter notebook rendering), and Node.js (Prettier/PurgeCSS).

## Local Development

### Docker (recommended)

```bash
docker compose pull && docker compose up   # Start dev server at http://localhost:8080
docker compose up --build                  # Rebuild after Gemfile/Dockerfile changes
docker compose down                        # Stop and free port 8080
```

### Legacy (requires local Ruby + Python)

```bash
bundle install && pip install jupyter
bundle exec jekyll serve --port 4000
```

### Before Every Commit

```bash
npx prettier . --write
```

Prettier formatting is enforced by CI — PRs fail if files aren't formatted.

## Content

| Directory                  | Purpose                          |
| --------------------------- | --------------------------------- |
| `_pages/`                   | Static pages (about, CV, projects, publications, ...) |
| `_posts/`                   | Blog posts                        |
| `_projects/`                | Project cards                     |
| `_news/`                    | Homepage announcements            |
| `_teachings/`               | Course pages                      |
| `_bibliography/papers.bib`  | Publications (BibTeX)             |
| `_data/`                    | Structured data (CV, awards, events, books, socials, ...) |

## Deployment

Pushes to `main` trigger a GitHub Actions workflow that builds the site and publishes it to the `gh-pages` branch, which GitHub Pages serves. The `gh-pages` branch is auto-generated and should never be edited directly.

## License

The al-folio theme is licensed under the [MIT License](LICENSE).
