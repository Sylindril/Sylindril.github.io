# Aditya Kumar

Aditya's personal site and blog, built with the official
[al-folio](https://github.com/alshedivat/al-folio) v1.1 starter and deployed
on GitHub Pages.

## Run locally

The site targets Ruby 3.3.5 and uses the dependency versions pinned in
`Gemfile.lock`.

```sh
bundle install
bundle exec jekyll serve --livereload
```

Then open `http://localhost:4000`.

## Write a post

Add a Markdown file to `_posts/` using the filename format
`YYYY-MM-DD-post-title.md`:

```md
---
layout: post
title: your title
date: 2026-08-03 09:00:00-0400
description: one sentence shown on the blog index
tags: poetry
categories: literary # use scientific for research writing
---

Start writing here.
```

Posts categorized as `literary` appear at `/literary/`; posts categorized as
`scientific` appear at `/scientific/`.

## Deploy

Push to `main`. The GitHub Actions workflow in
`.github/workflows/deploy-pages.yml` builds the site and publishes `_site/` to
GitHub Pages.

Replace `assets/img/prof_pic.jpeg` with a new headshot at any time.
