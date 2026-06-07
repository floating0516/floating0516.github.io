# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project overview

This is Li He's personal academic homepage, built with Hugo Blox Academic CV and Tailwind CSS. The site presents a bilingual academic profile, research interests, academic activities, experience, and selected projects.

The repository is primarily content/configuration, not application code. Most changes should be made in Hugo content Markdown files, Hugo YAML config, or small theme overrides.

## Common commands

Run these from the repository root (`floating0516.github.io/`).

```bash
# Install Node dependencies; package.json declares pnpm@10.14.0
pnpm install

# Local development server
pnpm dev
# equivalent: hugo server --disableFastRender --baseURL http://localhost:1313/

# Production build
pnpm build
# equivalent: hugo --minify

# Production-like build with warnings useful for CI/deploy debugging
hugo --gc --minify --logLevel debug --printI18nWarnings --printPathWarnings

# Generate the Pagefind search index after a build
pnpm dlx pagefind --source public
```

There is no test runner or lint script currently defined in `package.json`; use the Hugo build commands above as the main validation step.

## Toolchain and deployment

- Hugo version is pinned by `hugoblox.yaml`, Netlify, and GitHub Actions to Hugo `0.152.2`.
- `package.json` declares `packageManager: pnpm@10.14.0`; use `pnpm` as the only Node package manager and keep `pnpm-lock.yaml` as the lockfile.
- Hugo modules are managed through Go modules (`go.mod`, `go.sum`) and imported in `config/_default/module.yaml`.
- GitHub Pages deployment is configured in `.github/workflows/deploy.yml`: it installs dependencies, runs `hugo --minify --baseURL ...`, runs Pagefind, and uploads `public/`.
- Netlify deployment is configured in `netlify.toml` with similar Hugo + Pagefind build steps.

## Architecture and content flow

### Hugo Blox structure

- `config/_default/hugo.yaml` defines core Hugo settings: site title/base URL, Chinese as the default language, outputs, taxonomies, markup, and build behavior.
- `config/_default/module.yaml` imports Hugo Blox modules (`blox-plugin-netlify`, `blox-tailwind`) and mounts local `layouts` and `assets` so local overrides are applied on top of the theme modules.
- `config/_default/params.yaml` controls global appearance, SEO metadata, header, footer, locale, and feature toggles.
- `config/_default/languages.yaml` defines the bilingual setup. Chinese uses `content/zh` and is the default language; English uses `content/en`. Language-specific menus live here. `config/_default/menus.yaml` intentionally keeps the global menu empty.

### Content model

- Homepages are Hugo Blox landing pages (`type: landing`) composed from front matter `sections` arrays.
  - `content/zh/_index.md` is the Chinese homepage.
  - `content/en/_index.md` is the English homepage.
  - `content/_index.md` mirrors the Chinese landing page for the root/default content tree.
- The homepage `resume-biography-3` block reads the author profile by `username: admin`.
  - Default/root author data: `content/authors/admin/_index.md`
  - Chinese author data: `content/zh/authors/admin/_index.md`
  - English author data: `content/en/authors/admin/_index.md`
- Collection blocks on the homepages pull from section folders such as `events` and `projects`. Add bilingual entries under both `content/zh/...` and `content/en/...` when both languages should show the same item.
- Experience pages are separate Markdown pages under `content/zh/experience.md` and `content/en/experience.md`.
- Selected projects currently include `rtppp_b2b` entries under both language trees.

### Assets and overrides

- `assets/css/custom.css` contains local CSS overrides; currently it adjusts large homepage heading sizing on wide screens.
- Static/profile media are stored near the content that uses them, especially under `content/authors/admin/`.
- `layouts/_partials/hooks/head-end/github-button.html` injects the GitHub buttons script into the document head hook.

## Content editing notes

- This repository has been customized from an Academic CV starter template. Preserve Li He identity details and academic profile information; treat generic Hugo Blox sample content as replaceable template data.
- Keep bilingual content aligned when changing profile, homepage, event, project, or experience content. Update both `content/zh/...` and `content/en/...` unless the change is intentionally language-specific.
- The default language is Chinese and `defaultContentLanguageInSubdir` is `false`, so root URLs serve Chinese content while English lives under `/en/`.

### Phase 1 structure rules

- Treat `content/zh/...` as the authoritative Chinese content tree and `content/en/...` as the authoritative English content tree.
- Keep root-level `content/_index.md` and `content/authors/admin/_index.md` only as default-language compatibility content unless a future Hugo build test proves they can be removed safely.
- When editing homepage or author profile content, update the language-specific files first, then mirror only the necessary default-language content.
- Do not reintroduce template-only sections such as `courses` unless the site actually needs a course listing page.
- Use `pnpm` only; do not recreate `package-lock.json`.
