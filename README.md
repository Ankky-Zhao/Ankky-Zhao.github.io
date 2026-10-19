# Ankky-Zhao.github.io

Personal academic website of Anqi Zhao, PhD student at the Chair of Cartography and Visual Analytics, Technical University of Munich.

Live site: https://ankky-zhao.github.io/

Built with [Hugo](https://gohugo.io/) and the [HugoBlox Academic CV](https://github.com/HugoBlox/hugo-theme-academic-cv) template, bilingual (English / 中文), and deployed to GitHub Pages by the workflow in `.github/workflows/deploy.yml` on every push to `main`.

## Where to edit

| What | File |
|------|------|
| Name, bio, education, experience, skills, links | `data/authors/me.yaml` (English), `data/zh/authors/me.yaml` (Chinese overrides) |
| Profile photo | `assets/media/authors/me.png` (replace with a square photo, same file name) |
| Homepage sections (research, news, teaching, map) | `content/en/_index.md`, `content/zh/_index.md` |
| Projects (text + cover image) | `content/<lang>/projects/<name>/index.md` and `featured.png` |
| Publications | `content/<lang>/publications/<name>/index.md` |
| Blog posts | `content/<lang>/blog/<name>/index.md` |
| Menu, languages | `config/_default/languages.yaml` |
| Colours, header, footer | `config/_default/params.yaml` |

To add a project, copy one of the folders under `content/en/projects/` and `content/zh/projects/`, edit the text, and replace `featured.png` (3:2 images look best on the cards). The `weight` field controls the order on the homepage, higher first.

## Local preview

Requires Hugo Extended (version in `hugoblox.yaml`), Go and Node.js with pnpm.

```bash
pnpm install
hugo server
```

## One-time GitHub setup

In the repository go to **Settings → Pages** and set **Source** to **GitHub Actions**. The site is then rebuilt automatically after each push.

## Local template fixes

`layouts/_partials/` overrides three template files: a fix for a build error in publication links (`functions/build_links.html`), taller image previews on project cards (`hbx/blocks/portfolio`), and no "Present" label for entries without dates (`hbx/blocks/resume-experience`, `hbx/blocks/resume-awards`), labelled contact buttons (`hbx/blocks/resume-biography-3`). Re-check them after upgrading the template modules.
