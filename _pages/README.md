# README

To add a new page create the .md file with a layout, permalink, and title in the YAML frontmatter. Content
is then rendered by markdown. You can add the page to the site's top bar in `data/navigation.yml`.

Example:
```
---
layout: single
permalink: /new_page/
---

Some content for this *new page*.
```