# Zhen Wei — academic website

A responsive personal website for neuroscience, perception research, and creative work. Built with Jekyll and compatible with GitHub Pages. The academic layout uses a pure white background, charcoal text, muted gray secondary text, and restrained slate-blue text links, individual colors for profile icons, and blue, ochre, teal, and violet research schematics. Conventional serif typography, a compact biography and photograph, profile-link icons, section indexes, and an education timeline keep the presentation academic. It does not require a frontend build or third-party fonts. Palette tokens are defined at the top of `assets/css/academic.css`; the original SVG schematics use coordinated colors and pale fills. Print styles use neutral text and links.

## Editing content

- `_pages/about.md`: homepage, research interests, education, and contact section.
- `_pages/cv.md`: curriculum vitae. Only education and research background documented on the original website are included; add dates and professional experience when available.
- `_pages/publications.md`: research overview and publication listing.
- `_publications/`: add real publication entries here. The original example paper is marked `published: false`.
- `_pages/portfolio.html` and `_portfolio/`: creative projects.
- `_layouts/academic.html`: navigation, metadata, footer, and page shell.
- `assets/css/academic.css`: responsive design, mobile navigation, reduced motion, and print styles.
- `_includes/academic-icon.html` and `assets/images/research-*.svg`: original line icons and conceptual research illustrations.
- `assets/js/academic.js`: mobile navigation only. Content and links remain accessible without JavaScript.
- `_config.yml`: site metadata and author details.

The homepage retains the original research topics, photograph, advisors, email, and LinkedIn/GitHub profiles. The Santier brochure project remains available in the portfolio. Placeholder social accounts, the missing PDF CV link, example publications, and example teaching/talk/blog entries are no longer presented as real work. The `/cv/` route is now the working CV destination. No new degrees, employment history, dates, or publications were invented.

## Local development

With a supported Ruby and Bundler installed:

```sh
bundle install
bundle exec jekyll serve
```

Open the local address printed by Jekyll. GitHub Pages builds the existing `main` branch with the repository's configured Pages settings; no new hosting service is required. To review before publishing, create a branch and pull request, then merge after checking the preview.

## Validation

The redesigned pages were built successfully using Jekyll 4.3.2, with the configured plugins installed in a workspace-local gem directory. The original GitHub Pages Gemfile and plugin configuration remain in place. JavaScript syntax and local navigation/assets were checked. Browser-based visual and interaction checks could not be completed because the browser automation connection was unavailable. The legacy theme emits Sass deprecation warnings in Jekyll 4; these do not prevent the build and the redesigned pages use standalone CSS.

## Design references

The compact profile and research-list rhythm draw inspiration from the personal websites of [Jon Barron](https://jonbarron.info/) and [Phillip Isola](https://web.mit.edu/phillipi/). Their text, photographs, research results, and page source are not reused. The line illustrations on this site are original conceptual diagrams of the existing research interests.

## Credits

The original site is based on [AcademicPages](https://github.com/academicpages/academicpages.github.io), derived from Michael Rose's [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes). The original MIT license is preserved in `LICENSE`. Existing photographs and portfolio work are retained from the original repository.
