# Aditya Kumar

Aditya's personal site and blog, built with the official
[al-folio](https://github.com/alshedivat/al-folio) v1.1 starter and deployed
on Netlify.

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

Connect this repository to Netlify. [`netlify.toml`](./netlify.toml) pins the
Ruby version, builds the Jekyll site, and publishes `_site/`.

The current profile image is the public avatar from Aditya's GitHub account.
Replace `assets/img/prof_pic.jpeg` with a preferred headshot at any time.
