# AGENTS.md

## What this is

A static, single-file 3D walkthrough viewer (`index.html`) served by GitHub
Pages from `main` at https://bpspricigo.github.io/3d-walkthrough/. The user
loads a `.glb` model locally in the browser; nothing is uploaded.

## Rules

- **Never commit 3D models** (`.glb`, `.gltf`, `.bin`) or anything identifying
  a real building or its owner. Models are private and shared directly.
- Keep it one file with no build step; dependencies come from the CDN import map.
- Test by opening `index.html` through a local web server (module scripts do not
  load from `file://` in every browser), load a `.glb`, try both modes.

## Workflow

- Every change on its own branch; no push, PR or merge until Bruno has tested it.
- Every issue and PR has an assignee (Bruno, `bpspricigo`, by default) and every
  PR links its issue (`Closes #N` / `Part of #N`).
- An issue assigned to someone else is theirs: do not pick it up.
- Commits and GitHub text carry no tool attribution.
