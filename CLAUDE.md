# CLAUDE.md

## Project

Single-page site (`index.html`) that calculates "sister days" — mirror dates equidistant from the coldest day of the year.

## Version footer

The footer in `index.html` contains a version link pointing to a specific git commit:

```html
<a href="https://github.com/q5m-ai/sister-day/commit/HASH" ...>vHASH</a>
```

**After every commit you push**, update the footer's commit hash to match the new HEAD commit. Run `git rev-parse --short HEAD` to get the short hash, then replace both the URL and display text in the footer's version link.
