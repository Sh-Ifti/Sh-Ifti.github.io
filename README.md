# sh-ifti.github.io

Personal academic website of **Shahariar Ifti**, live at **https://sh-ifti.github.io**.

![Profile Views](https://komarev.com/ghpvc/?username=sh-ifti&color=blue)

Built with [Jekyll](https://jekyllrb.com/) and the [al-folio](https://github.com/alshedivat/al-folio) theme, hosted free on GitHub Pages. Every push to `main` rebuilds and publishes the site automatically (see the **Actions** tab); the built site lives on the `gh-pages` branch, which should not be edited by hand.

## Editing from the browser

Sign in to [Pages CMS](https://app.pagescms.org) with GitHub and open this repository. You can:

- write and edit **blog posts**
- add **news** items to the home page
- edit **projects**
- add **photos** to the gallery

Changes are saved as commits, and the site updates about two minutes later.

## Where things live

| Content | File or folder |
|---|---|
| Home page biography | `_pages/about.md` |
| Publications | `_bibliography/papers.bib` |
| Papers under review | `_pages/publications.md` |
| Projects | `_projects/` |
| Blog posts | `_posts/` |
| News items | `_news/` |
| CV page | `_data/cv.yml`, PDF in `assets/pdf/` |
| Gallery photos | `_data/gallery.yml`, images in `assets/img/uploads/` |
| Social links | `_data/socials.yml` |
| Site settings | `_config.yml` |
| Profile photo | `assets/img/prof_pic.jpg` (if missing, the GitHub profile photo is used) |

To show the Gallery in the menu, set `nav: true` in `_pages/gallery.md`.
