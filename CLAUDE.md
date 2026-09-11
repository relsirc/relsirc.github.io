# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

`relsirc.github.io` — GitHub Pages site (repo name form triggers Pages auto-publish). No build tooling, no package manager, no test suite. Jekyll runs server-side on GitHub's infra using `_config.yml` (theme: `jekyll-theme-slate`); there is no local Jekyll setup in this repo.

## Commands

There are no build, lint, or test commands — this repo has no `package.json`, `Gemfile`, or CI config. Changes go live by committing to `main`; GitHub Pages rebuilds via Jekyll automatically. To preview HTML/Markdown changes, open the file directly in a browser or use a static file server (e.g. `python3 -m http.server`).

## Files

- `_config.yml` — Jekyll theme config for GitHub Pages.
- `README.md` — GitHub Pages default boilerplate (editor/Jekyll/theme instructions), not project-specific documentation.
- `config.json` — standalone settings blob (chat/call flags, work hours); not consumed by any code in this repo.
- `pets.json` — standalone data file (array of pet entries: image_url, title, content_url, date_added); not referenced by any HTML in this repo.
- `test1.html` — scratch/test page with sample button and form markup, plus an embedded `<div id="json">` containing an unrelated product-variant JSON blob (apparent copy-paste scratch data, not wired to any script).

Note: `config.json`, `pets.json`, and `test1.html` are disconnected from each other — nothing in the repo loads or links them together. Treat each as independent scratch content unless a task says otherwise.
