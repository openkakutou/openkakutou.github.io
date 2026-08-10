# openkakutou.github.io

Public showcase site for [OpenKakutou](https://github.com/openkakutou): lists and links out to whichever viewer, editor, and complete game apps are currently live. Published at [openkakutou.github.io](https://openkakutou.github.io/) via GitHub's special user/organization-site repo name — no build step, no CI, `index.html` on `main` is the deployed page.

Doesn't host or reimplement any app's own functionality — each app (`character-viewer-web`, `stage-editor`, `mode-quick-versus`, …) keeps its own deployment. This repo is a discovery layer on top.

## Editing

Plain static HTML/CSS in `index.html`, no build tooling. Edit, commit, push to `main` — GitHub Pages serves the new version within a minute or two.

See [`openkakutou/roadmap`](https://github.com/openkakutou/roadmap)'s `repos.md` and `.vibe/decisions/018` for how this repo fits the rest of the org.

## License

MIT — see [LICENSE](LICENSE).
