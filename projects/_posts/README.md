# README
The projects YAML front matter contains information for its appearance in the `_projects` main page as well as the content on the indivdual project page:

- `title`: Title text of the project that appears on the `_projects` page
- `excerpt`: Descriptive sub-text for the `title` that also appears on the `_projects` page
- `header.teaser`: Image that will appear on the `_projets` page. Check the rendering to make sure that the aspect ratio aligns with the other entries.
- `featured_figure.image`: Image that appears at the top of the individual project's page.
- `featured_figure.caption`: A caption for the `featured_figure.image`
- `learn_more`: A link to learn more about the project (e.g., a paper or talk)
- `code`: A link to the repository or code associated with the project.
- `people.name`: Name of the a person associated with the project
- `perople.ccog`: For the person, if they are associated with the CCOG group

Example:

```
---
title: "Linking ENSO to oceanic dynamical regimes using transparent ML"
excerpt:  "Investigating ENSO dynamics in several CMIP6 models"
header:
    teaser: "assets/images/enso_project-th.png"
featured_figure: 
    image: "assets/images/enso_project.png"
learn_more: "assets/papers/enso_project_paper.pdf"
code: "https://github.com/maikejulie/DNN4Cli"
people:
  - name: "Zouberou Sayibou"
    ccog: true
  - name: "Maike Sonnewald"
    ccog: true
  - name: "Aparna Radhakrishnan"
  - name: "Andrew Wittenberg"
  - name: "Redouane Lguensat"
  - name: "V. Balaji"
---
```

# TITLE OF THE PAPER

Put the abstract here.

```
