# Vela copy demo

This repository is a source copy of the official [LuxAlgo/Vela](https://github.com/LuxAlgo/Vela) project at tag **v0.10.4** (upstream commit `12b624849c3c47666564373bc7cf405d093687d4`).

The complete upstream source tree is retained, including the chart core, native renderer, workspace, UI kit, documentation, tests, examples, original package lockfile, `LICENSE`, and `NOTICE`. The original upstream workflow definitions are preserved under `upstream-source/.github/workflows/` rather than activated in this copy; the only active workflow is the source-import workflow in `.github/workflows/`.

## Local development

```bash
npm ci
npm run playground
```

Open `http://localhost:5190/` for the full multi-chart workspace. The upstream `/widget.html` and `/workspace.html` examples remain available.

## Vercel

Import this repository using the repository root. `vercel.json` runs `npm ci`, builds the workspace through Vite, and publishes `playground/dist`.

## Changes in this copy

- `playground/index.html` now mounts the upstream `VelaWorkspace` directly, so the root route opens the full workspace instead of the playground selection page.
- `vercel.json` adds Vercel build and output settings.
- Upstream workflow definitions are retained under `upstream-source/.github/workflows/`; they are not activated automatically in this demo copy.
- `.github/workflows/import-vela.yml` records the reproducible source-import workflow.

## License and attribution

Vela is distributed under Apache-2.0. The upstream `LICENSE` and `NOTICE` files are preserved. The Vela attribution mark remains enabled on every chart, as required by the NOTICE.
