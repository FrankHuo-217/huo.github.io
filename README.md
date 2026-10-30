# Frank Yingjie Huo: academic homepage

Personal academic site built with the [Academic Pages](https://github.com/academicpages/academicpages.github.io) Jekyll template and deployed to GitHub Pages by a GitHub Actions workflow (`.github/workflows/jekyll.yml`).

## One-time setup

1. **Turn on Pages:** in the repository, go to Settings → Pages → Build and deployment → Source and choose **GitHub Actions**. Every push to `main` then rebuilds and deploys the site. Pull requests are built as a check but not deployed.
2. **Address:** the repository is named `yingjiehuo.github.io`, so GitHub serves the site at `https://yingjiehuo.github.io/`. If the account or repository is ever renamed, update `url` and `repository` in `_config.yml`; the workflow sets the base path automatically.

## Placeholders: `[VERIFY]`

Anything unconfirmed is shown on the site as a yellow `[VERIFY: …]` box, so a missed placeholder is easy to spot. None are left at launch; if you add one later, find them all with:

```bash
grep -rn "VERIFY" _config.yml _pages _publications _talks
```

## Editing content

All content is Markdown, with settings in YAML front matter at the top of each file.

| Page | File |
| --- | --- |
| Home | `_pages/about.md`: short paragraphs written by hand. Citations link straight to each paper (DOI, arXiv or publisher), so update them here too when a preprint is published. |
| Publications | one file per item in `_publications/`. The In the media section is in `_pages/publications.md`. |
| Teaching | `_pages/teaching.md` |
| Talks (listed on the CV page) | one file per talk in `_talks/` |
| CV | `_pages/cv.md`, and `files/Huo_CV.pdf` for the download. Upload only the website version of the PDF (the one without References), since the file is public. |
| Sidebar, site title, links, research interests line (`tagline`) | `_config.yml` |
| Photo | `images/profile.jpg`, a square image (600 × 600 works well); the site shows it as a circle. |
| Header menu | `_data/navigation.yml` |

### Add a publication

Copy an existing file in `_publications/` and edit its front matter:

```yaml
---
title: "Title of the paper"
authors: "F. Y. Huo, N. F. Johnson"
category: articles                    # book | articles | preprints | other
venue: "Phys. Rev. Lett."
volume: "133"
details: "247401"                     # article number or pages
year: 2024
date: 2024-12-10                      # used only for ordering, newest first
doi: "10.1103/..."                    # optional; links to https://doi.org/...
arxiv: "2508.01097"                   # optional; always quote arXiv IDs
publisher_url: "https://..."          # optional
pdf: "/files/paper.pdf"               # optional
note: "One-line note shown in italics" # optional
equal_contribution: true              # optional; adds the "† Equal contribution" footnote. Put † after the names in `authors`.
hide: true                            # optional; keeps the file but leaves it off the Publications page
---
```

When a preprint is published, change its `category` to `articles` and add `venue`, `volume`, `details` and `doi`. Keep the `arxiv` field.

### Add a talk

Copy a file in `_talks/`:

```yaml
---
title: "Talk title"
type: "Invited talk"
venue: "SIAM Annual Meeting"
session: "Minisymposium name"   # optional
location: "City"                # optional
date: 2026-07-08                # used for ordering
date_display: "July 2026"       # optional; how the date is printed
link: "https://..."             # optional link to the program entry
slides: "/files/slides.pdf"     # optional
---
```

## Local preview

You need Ruby 3.x and Bundler. Node is only used to minify the JavaScript.

```bash
bundle install
```

```bash
npx uglify-js assets/js/plugins/jquery.greedy-navigation.js assets/js/_main.js assets/js/theme.js -c -m -o assets/js/main.min.js
```

```bash
bundle exec jekyll serve
```

Then open http://localhost:4000. The Sass deprecation warnings during the build come from the template and are harmless.

## Template changes

Compared with the stock Academic Pages template:

- Removed the blog, portfolio, talk map, sample content and the template's own GitHub housekeeping.
- Publications are listed on the Publications page and talks on the CV page; they do not get a page each.
- New includes: `publication.html`, `publication-list.html`, `talk.html`, `cv-link.html`, `verify.html`.
- Site styles are in `_sass/layout/_custom.scss`. The page-load fade-in is turned off, and the footer follows the content.
- MathJax is not loaded, and Academicons is served from `assets/` rather than a CDN. The only remaining third-party script is jQuery, which the template needs.
- The workflow deploys from `main` and builds pull requests as a check.

Template code is MIT-licensed; see `LICENSE`.
