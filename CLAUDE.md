# CLAUDE.md

## Project

Single-page site (`index.html`) that calculates "sister days" — mirror dates equidistant from the coldest day of the year.

## Version footer

The footer in `index.html` uses a `__COMMIT_HASH__` placeholder. The GitHub Actions deploy workflow (`.github/workflows/deploy.yml`) replaces it with the real short SHA at deploy time. **Do not** hardcode a commit hash — leave the placeholder as-is.

## Deployment

The site deploys to GitHub Pages automatically on push to `main` via GitHub Actions. The workflow injects the commit hash and publishes — no build step needed.
