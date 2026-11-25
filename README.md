# 3D walkthrough

A single-page viewer for `.glb` building models: look at the model from above
(dollhouse view, ceilings cut away) or walk through it at eye height.

**Open it:** https://bpspricigo.github.io/3d-walkthrough/

## Use

1. Open the link and drop a `.glb` file on the page (or click **Choose .glb file**).
   The file opens in your browser only; nothing is uploaded.
2. **Dollhouse**: drag to turn, scroll or pinch to zoom, right-drag to pan.
   Double-click (or tap) a spot on the floor to start walking there.
3. **Walk**: W A S D or arrow keys to move, drag to look around, Shift to walk
   faster, Esc to go back to the dollhouse. On a phone, use the stick in the
   bottom-left corner.

Works in any current desktop or mobile browser with WebGL.

## How it works

Everything is in [index.html](index.html): three.js (loaded from a CDN) renders
the model, three-mesh-bvh speeds up the raycasts used for floor detection and
wall collision. No build step and no server code; GitHub Pages serves the file
as is.

Models are never stored in this repo (`.gitignore` blocks `.glb` / `.gltf`).
