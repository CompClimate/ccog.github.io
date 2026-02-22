# Computational Climate and Ocean Group Website

Source for the [CCOG lab website](https://compclimate.github.io), built with Jekyll and hosted on GitHub Pages.

## Site Structure

| Path | Purpose |
|---|---|
| `_people/` | Lab member profiles |
| `projects/_posts/` | Research project pages |
| `_data/news.yml` | Home page news items |
| `_data/publications.bib` | BibTeX bibliography |
| `_pages/` | Top-level site pages |

## Adding Content

### News

File: `_data/news.yml`

Prepend a new entry at the top of the file. Only year and month are shown on the home page.

```yaml
- date: "2026-02-01"
  text: |
    Your news item here. Supports **Markdown** and [links](https://example.com).
```

### People

Directory: `_people/`

Create a new `.md` file (e.g., `_people/firstname.md`) with front matter only — no body text needed:

```yaml
---
lastname: "Smith"
firstname: "Jane"
pub_id: "Smith J"           # Must match author string in publications.bib
role: "PhD Student"         # e.g. PI, Postdoc, PhD Student, MS Student, Undergrad
status: "active"            # active or alumn
sort_display: 5             # Lower numbers appear first
image_path: /assets/images/jane.jpeg   # Square images recommended
pronouns: "she/her"         # Optional
website: "https://example.com"         # Optional
---
```

People images should be square. The default placeholder is the otter image at `/assets/images/otter.png`.

### Publications

File: `_data/publications.bib`

Add a standard BibTeX entry. The `pub_id` field in a person's profile links their name in the bibliography to their CCOG profile — ensure the `pub_id` matches the author string exactly as it appears in BibTeX entries.

### Projects

Directory: `projects/_posts/`

Create a new file named `0000-01-01-<slug>.md` (the date prefix is required by Jekyll but is not displayed):

```yaml
---
title: "Project Title"
excerpt: "One-sentence description shown on the projects listing page."
header:
    teaser: /assets/images/your-figure.png
featured_figure:
    image: /assets/images/your-figure.png
    caption: "Figure caption."
learn_more: "https://doi.org/..."   # Optional: link to paper
code: "https://github.com/..."      # Optional: link to code
people:
  - name: "Jane Smith"
    ccog: true                      # true if current/former CCOG member
  - name: "Collaborator Name"
tags:
  - ocean
  - deep learning
---

Body text describing the project. Supports full Markdown.
```

## Local Development

**Prerequisites**: Ruby and Bundler.

```bash
bundle install              # Install Ruby gem dependencies
bundle exec jekyll serve    # Serve locally at http://localhost:4000/ccog.github.io/
```

After editing `_config.yml`, restart the server — it does not auto-reload config changes.

## Deployment

Pushes to the `main` branch deploy automatically via GitHub Pages.

## Attribution

This site is built with:

- [Jekyll](https://jekyllrb.com/)
- [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) theme by [Michael Rose](https://mademistakes.com/) — MIT License
- [jekyll-scholar](https://github.com/inukshuk/jekyll-scholar) for bibliography rendering
