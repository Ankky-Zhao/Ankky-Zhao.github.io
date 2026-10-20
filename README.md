# Ankky-Zhao.github.io

Personal academic website of Anqi Zhao, PhD student at the Chair of Cartography and Visual Analytics, Technical University of Munich.

Live site: https://ankky-zhao.github.io/

Built with [Hugo](https://gohugo.io/) and the [HugoBlox Academic CV](https://github.com/HugoBlox/hugo-theme-academic-cv) template, bilingual (English / 中文), and deployed to GitHub Pages by the workflow in `.github/workflows/deploy.yml` on every push to `main`.

## Where to edit

| What | File |
|------|------|
| Name, bio, education (with supervisors), skills, honours, links | `data/authors/me.yaml` (English), `data/zh/authors/me.yaml` (Chinese overrides) |
| Profile photo | `assets/media/authors/me.png` (replace with a square photo, same file name) |
| Homepage (all sections, scrolling; research-interest statement is `interests_text` here) | `content/en/_index.md`, `content/zh/_index.md` |
| Single-section pages linked from the menu | `content/<lang>/publications/_index.md`, `projects/_index.md`, `news.md`, `profile.md`, `collaborate.md` (news and collaboration text appear on both the homepage and their own page, so edit both) |
| Publications (one card per paper, with Paper/Code buttons) | `content/<lang>/publications/<name>/index.md` and `featured.png` |
| Projects (GitHub projects, text + cover image) | `content/<lang>/projects/<name>/index.md` and `featured.png` |
| Blog posts | `content/<lang>/blog/<name>/index.md` |
| Profile (skills, honours, languages, hobbies; skills/honours/languages data in the author files) | `content/<lang>/profile.md` and the homepage; CV PDF at `static/uploads/cv.pdf` |
| Menu, languages | `config/_default/languages.yaml` |
| Colours, header, footer | `config/_default/params.yaml` |

To add a project, copy one of the folders under `content/en/projects/` and `content/zh/projects/`, edit the text, and replace `featured.png` (3:2 images look best on the cards). The `weight` field controls the order on the homepage, higher first.

## Writing a blog post

Each post is a folder with an `index.md` (and optionally a `featured.png` cover). English posts live in `content/en/blog/`, Chinese posts in `content/zh/blog/`; use the same folder name in both so the language switch links them. A post that exists in only one language is fine too.

On GitHub (no software needed): open `content/en/blog/` in the repository, choose **Add file → Create new file**, type `my-post-name/index.md` as the name, paste the template below, write the post in Markdown, and commit. Images can be added with **Add file → Upload files** into the same folder and referenced as `![caption](image.png)`. The site rebuilds automatically in a few minutes.

Locally: `hugo new content en/blog/my-post-name/index.md` creates the file from `archetypes/blog.md`.

```yaml
---
title: 'Post title'
date: 2026-10-20
summary: 'One sentence shown on the blog card.'
tags:
  - LLM agents
---
```

## Local preview

Requires Hugo Extended (version in `hugoblox.yaml`), Go and Node.js with pnpm.

```bash
pnpm install
hugo server
```

## One-time GitHub setup

In the repository go to **Settings → Pages** and set **Source** to **GitHub Actions**. The site is then rebuilt automatically after each push.

## Styling

Site-wide CSS tweaks (justified paragraphs) live in `assets/css/custom.css`.

## Local template fixes

`layouts/_partials/` overrides three template files: a fix for a build error in publication links (`functions/build_links.html`), taller image previews on project cards (`hbx/blocks/portfolio`), and no "Present" label for entries without dates (`hbx/blocks/resume-experience`, `hbx/blocks/resume-awards`), labelled contact buttons (`hbx/blocks/resume-biography-3`). Re-check them after upgrading the template modules.
