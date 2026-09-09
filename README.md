# fredrikmoller1324.github.io

Personal site built with [Jekyll](https://jekyllrb.com/), hosted on GitHub Pages.

## Structure

- `index.md` — homepage
- `about.md` — about / resume page (served at `/about/`)
- `_posts/` — blog posts (`YYYY-MM-DD-title.md`)
- `_config.yml` — site configuration

## Local development

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.

## Publishing a post

Add a file to `_posts/` named `YYYY-MM-DD-title.md`:

```markdown
---
layout: post
title: "My Post Title"
date: 2026-01-01 12:00:00 +0000
categories: general
---

Post content here.
```

Push to `main` and GitHub Pages will rebuild the site automatically.
