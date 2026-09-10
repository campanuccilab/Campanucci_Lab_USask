# Campanucci Lab

Website for the Campanucci Lab — Dr. Veronica Campanucci, Department of Anatomy,
Physiology, and Pharmacology, College of Medicine, University of Saskatchewan.

Research in neuroscience and electrophysiology: patch-clamp and extracellular
recording, stem-cell-derived organoid models, and cystic fibrosis / CFTR
modulator work.

## What is here

| Path | What it is |
| --- | --- |
| `index.html` | The entire site — markup, styles and scripts in one self-contained file. |
| `images/` | The 25 photographs, micrographs and one video the page references. |
| `.nojekyll` | Tells GitHub Pages to serve the files as-is rather than running Jekyll. |

## Design constraints

These are deliberate. Please keep them.

- **No external dependencies.** No CDN scripts, no web fonts, no remote images,
  no build step. The page opens by double-clicking it, offline, on any machine.
  The single exception is the contact map, which is created in JavaScript only
  when a visitor scrolls to the contact section, is skipped entirely when
  offline, and falls back to a painted card if the request fails.
- **Filename case must match exactly.** GitHub Pages is case-sensitive; Windows
  is not. A reference that works locally can 404 once published.
- **Images are not downscaled.** The lightbox displays them far larger than the
  tile does.

## Editing

The top of `index.html` contains a plain-data block (`SITE`) holding the text,
people, publications, gallery entries and contact details. Ordinary content
changes — a new lab member, a new paper, a different photo — are edits to that
block and need no knowledge of the rest of the file.

## Authoring notes

The working copy, the regression test suite, the alternative design candidates
and a detailed `AI-README.md` live alongside this site on the lab's internal
share and are intentionally not published here.
