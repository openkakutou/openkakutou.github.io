# CLAUDE.md — openkakutou.github.io

## Project overview

Public showcase site for [OpenKakutou](https://github.com/openkakutou): a landing page listing and linking out to whichever viewer, editor, and complete game (`mode-*`) apps are currently live, kept up to date as new apps ship. Uses GitHub's special user/organization-site repo name so it publishes at the bare root `https://openkakutou.github.io/` instead of a project-site sub-path. Doesn't host or reimplement any app's own functionality — each app keeps its own deployment; this is a discovery/marketing layer on top. See `roadmap`'s `.vibe/decisions/018` and `repos.md`.

**Stack:** plain HTML/CSS, no framework, no build step, no tests.
**Type:** static site (single `index.html`)

## Project language

English — matches the convention in every other OpenKakutou repo.

## Current state

Deliberately minimal first version (2026-08-10): a single hand-written `index.html` with links to the three live `*-viewer-web` apps and placeholder cards for the editors and `mode-quick-versus`, not yet deployed. No build tooling, no `.vibe/` scaffold yet — intentional, to be iterated on rather than over-built up front. When this grows past a single static page (e.g. a generated app list, a build step, tests), revisit the stack choice and set up `.vibe/` via `/vibe:init` at that point.

## Deployment

GitHub Pages, source = `main` branch, root — no GitHub Actions workflow needed for plain static HTML. Push to `main` and the live site updates automatically within a minute or two.
