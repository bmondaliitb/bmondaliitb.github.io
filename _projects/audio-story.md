---
title: PDF to AudioStory
kind: Accessibility tool
stack: Python · FastAPI · Tkinter
mark: AS
accent: violet
order: 4
featured: true
summary: A modular desktop and API workflow for extracting Bengali or English text from PDFs and turning it into expressive narration.
---

PDF to AudioStory separates document extraction, narration, HTTP transport, and the desktop interface into independent components. The core library can be used directly; a FastAPI adapter exposes the same work through a documented contract; and the Tkinter client communicates only with that API.

## Text from difficult PDFs

The extraction pipeline can use embedded text or OCR page by page. In automatic mode it keeps strong native text, recognizes weak or image-only pages, and detects legacy Bengali font mappings that look like text to a PDF reader but do not produce valid Unicode.

## Narration as a second stage

Extracted text remains editable before synthesis. The narration layer can respond to headings, stage directions, questions, punctuation, and Bengali emotional cues by adjusting pace and pitch. A steady natural mode is available when consistency matters more than dramatic delivery.

The service is stateless: uploaded PDFs and generated audio are not retained after the response. This architecture also leaves room for a future browser client without coupling it to the extraction implementation.

This is currently a local project without a public repository.
