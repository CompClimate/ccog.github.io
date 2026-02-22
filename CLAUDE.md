# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is the **Computational Climate and Ocean Group (CCOG)** lab website, hosted on GitHub Pages. It is built with **Jekyll** using the **Minimal Mistakes** theme and **jekyll-scholar** for bibliography management.

## Local Development

```bash
bundle install          # Install Ruby dependencies
bundle exec jekyll serve  # Serve locally at http://localhost:4000
```

After editing `_config.yml`, restart the server (it does not auto-reload).

## Site Architecture

**Theme**: Minimal Mistakes (`minimal-mistakes-jekyll` gem), customized via `_layouts/`, `_includes/`, and `_sass/`.

**Collections** (defined in `_config.yml`):
- `_people/` — Group members. Each file has YAML front matter with `lastname`, `firstname`, `pub_id`, `role`, `status` (active/alumn), `sort_display`, `image_path`. Optional: `website`, `pronouns`.
- `projects/_posts/` — Research projects. Front matter: `title`, `excerpt`, `header.teaser`, `featured_figure`, `learn_more`, `code`, `people`.

**Data files** (`_data/`):
- `news.yml` — News items displayed on the home page. Each entry has `date` (quoted string) and `text` (Markdown). Sorted newest-first. To add news, prepend a new entry at the top of the file.

**Pages** (`_pages/`): Top-level site pages (home, publications, projects, impacts, people, join, contact). Navigation order is set in `_data/navigation.yml`.

**Publications**: Managed via `_data/publications.bib` (BibTeX) and rendered by jekyll-scholar using `nature-publishing-group-vancouver` style. The bibliography template is `_layouts/bibtemplate.html`. Person `pub_id` fields link authors to their profiles.

## Content Conventions

- People images should be square; a default otter image is available as placeholder.
- Project teaser images should have consistent aspect ratios across entries.
- News items live in `_data/news.yml`; only year and month render on the home page. Add new entries at the top of the file.
- To add a page to the top navigation bar, edit `_data/navigation.yml`.
