# Carlos Patricio Personal Site

This repository contains a Jekyll-powered personal website and writing archive published through GitHub Pages.

## Structure

- `_config.yml`: site configuration, navigation, and permalink settings
- `_layouts/`: shared HTML layouts for default pages, standalone pages, and blog posts
- `_posts/`: dated Markdown posts
- `index.md`, `about.md`, `posts.md`: top-level site pages
- `assets/`: styles and static images

## Local development

Prerequisites:

- Ruby
- RubyGems
- Jekyll

Install the required gems if needed:

```bash
gem install jekyll bundler
```

Start the local server from the repository root:

```bash
jekyll serve
```

Open `http://127.0.0.1:4000` in your browser.

## Build

To generate the static site locally:

```bash
jekyll build
```

The output will be written to `_site/`.

## Deployment

The site is configured for GitHub Pages at `https://capatric.github.io`.

Push changes to the default branch and GitHub Pages will publish the updated site according to the repository settings.

## Writing posts

Create new posts in `_posts/` using the filename format:

```text
YYYY-MM-DD-title.md
```

Each post should include front matter similar to:

```yaml
---
layout: post
title: "Post title"
date: 2026-04-23
description: "Short summary for metadata."
excerpt: "Short summary used in post listings."
---
```
