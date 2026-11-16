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

`book2poem` turns old PDFs into browsable collections while preserving scanned pages. It handles works spanning multiple pages, recurring headers and page numbers, and Bengali legacy fonts without usable Unicode mappings.

## Editing and export

The tool detects centered titles, groups continuation pages, and proposes poem or story boundaries. A GTK4 editor supports title-box OCR, same-page splits, crop overrides, shared trims, boundary changes, merging, issue review, and undo/redo.

A JSON manifest stores the reviewed boundaries. From it, the tool exports vertically merged WebP images, static JSON, or a searchable SQLite/FTS5 library without changing the source PDF.

Original typography and illustrations remain visible. Reliable OCR adds search, so a collection can be used while text corrections are still in progress.
