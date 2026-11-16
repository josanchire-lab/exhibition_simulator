# Exhibition simulator

A 3D simulator for exhibition layouts built from Aluvision aluminium frames and glass
showcases, drawn in millimetres at real size. It is one self-contained HTML file:
open `index.html` in a browser and everything runs locally, with no build and no server.

## What it does

- **Composition** — one to eight units in a row, each one a size M frame (992 mm),
  a size L frame (1,240 mm) or a showcase on legs.
- **Layout** — straight, curved, accordion or facing, with spacing, curve, fold angle,
  stagger and, in facing, one or two rows. Builder mode drags the units by hand.
- **Panel content** — a sample typographic sheet at 1:1 on every plate, your own
  pictures per plate, or your own text written in the panel editor.
- **Panel editor** — blocks of title, subtitle, body, quote, caption, picture and bar,
  moved and resized on the panel itself, with the point sizes you would print.
  It saves and loads its own file, a Word (A4) file, and an InDesign package (IDML).
- **Readability** — the reading distance measures from the camera to the cross in the
  middle of the view, and the eye-height line sits at 1.6, 1.7 or 1.8 m on the panels.
- **Taking it away** — Export PNG for the current view, and Augmented Reality mode,
  which opens the whole composition at real size on an iPhone or iPad.

## How it is made

Plain HTML, CSS and JavaScript in a single file, with three.js (r128) loaded from a CDN.
The frame and showcase meshes are embedded as base64 in a `<script type="application/json">`
block; the plates, the floor grid, the labels and the demo sheet are drawn into canvases
at run time. The Word, IDML and USDZ files are written by hand, zip and all.

## Status

Work in progress. The version number in the header goes up with every change.
