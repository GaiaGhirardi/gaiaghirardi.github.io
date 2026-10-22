# Gaia Ghirardi – website

Built with Jekyll. GitHub turns these files into the website automatically
every time changes are pushed (it takes about a minute).

## Where to edit what

| To change…                                         | Edit this file             |
|----------------------------------------------------|----------------------------|
| Bio paragraphs, research fields, bike photo        | `index.md`                 |
| Position, institution, email, photo, profile links | `_config.yml`              |
| Papers (titles, authors, journals, links)          | `_data/papers.yml`         |
| Work in progress page (photo at the bottom)        | `work-in-progress.md`      |
| PhD thesis                                         | `thesis.md`                |
| CV page                                            | `cv.md`                    |
| Teaching                                           | `teaching.md`              |
| Data & code                                        | `datacode.md`              |
| Links under your name                              | `_data/navigation.yml`     |
| Fonts, colors, spacing, buttons                    | `assets/site.css`          |
| CV                                                 | replace `files/Ghirardi_CV.pdf`, keeping the same name |

Put PDFs in `files/` and link them as `/files/name.pdf`, and images in
`images/`, linked as `/images/name.jpg`.

## Pages

The welcome page (`index.md`) shows the bio. Every other page is a Markdown file in the main folder with a header like this:

```
---
layout: page
title: Teaching
permalink: /teaching/
---
```

To add a page, copy one of them, change the title and permalink, and add a
line for it in `_data/navigation.yml`.

## Adding a paper

Copy an existing entry in `_data/papers.yml` and change it. Indentation
matters: use spaces (never Tab) and line up each field with the ones above it.
Groups marked `page: work-in-progress` appear on the Work in progress page,
groups marked `page: publications` on the Publications page, so when a working
paper is published, move its entry from "Work in progress" to
"Peer-reviewed articles".
Authors are listed in order, and your name is shown in bold when it is
written exactly as `citation_name` in `_config.yml` (`G. Ghirardi`).
An optional `abstract:` adds an "abstract" button that opens the text.

## Moving from the preview to the real site

The preview runs at https://giorgiopietrabissa.github.io/Web_Gaia/.
For the real site, change these two lines in `_config.yml`:

```
url: "https://gaiaghirardi.github.io"
baseurl: ""
```

## Credits

Font: Libertinus Serif (SIL Open Font License, `assets/fonts/OFL.txt`).
Thesis illustrations: Giuditta Furlan.
