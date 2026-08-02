---
title: book2poem
kind: Document tool
stack: Python · GTK4 · OCR · SQLite
mark: b2p
accent: rose
order: 3
featured: true
summary: A visual workflow for turning poems and short stories in old PDFs into cropped images and searchable static libraries.
image: /assets/images/tagore-artwork.webp
image_alt: Historical monochrome illustration representative of scanned literature processed by book2poem.
image_caption: The tool preserves scanned Bengali pages as images while storing usable OCR text for search.
---

Old books rarely provide clean structural boundaries. A poem may continue across pages; recurring headers and page numbers should be removed; and Bengali text may use a legacy font with no usable Unicode mapping. `book2poem` addresses that messy middle between a scanned PDF and a browsable digital collection.

## Reviewable automation

The tool detects visually centered title lines, groups continuation pages, and proposes poem or story ranges. A GTK4 editor then makes those suggestions reviewable. It supports title-box OCR, same-page splits, per-page crop overrides, shared trims, boundary adjustment, merge operations, issue review, and undo/redo.

A small JSON manifest remains the source of truth. That decision separates human judgment—where one work starts and another ends—from repeatable rendering. Rebuilding can produce vertically merged WebP images, static JSON, or a searchable SQLite/FTS5 text library without changing the source PDF.

## Why it is useful

The project is aimed at cultural material for which perfect OCR is not a realistic prerequisite. Original typography and illustrations remain visible, while any reliable text becomes an additional search layer. This makes incremental curation possible: a collection can be useful before every title and line has been corrected.

The code repository is currently private, so this page describes the workflow without exposing an inaccessible code link.
