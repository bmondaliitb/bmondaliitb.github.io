---
title: Thought Breaker
kind: Desktop app
stack: Python · GTK4 · Libadwaita
mark: TB
accent: green
order: 1
featured: true
summary: A spatial thinking tool for breaking an idea into connected, actionable notes on a zoomable canvas.
github: https://github.com/bmondaliitb/thought-breaker
image: /assets/images/thought-breaker.png
image_alt: Thought Breaker desktop application showing connected note cards on a canvas and a project sidebar.
image_caption: The native GNOME interface, with a freely arranged thought graph and directional dependencies.
---

Thought Breaker turns an open-ended idea into a graph of smaller thoughts. Notes can be placed freely, connected with directional arrows, and moved through todo, doing, done, or blocked states. Unlike a linear task list, the canvas keeps context visible: it shows which ideas depend on others and which can be acted on next.

## Design choices

The app is deliberately native rather than browser-based. GTK4 and Libadwaita provide familiar GNOME behavior, while the canvas handles panning, zooming, selection, dragging, and connection geometry. The same Python application also runs on macOS and can be packaged as an application bundle.

Projects are stored as readable Markdown instead of an opaque database. Completed graphs move into a separate archive, and an undo history makes rearranging a large map less risky.

## What it taught me

Building Thought Breaker meant treating interaction details as part of the data model: undo must restore graph structure as well as visual state, deleting a note affects edges, and marking the main thought complete changes the project's lifecycle. It has been a useful exercise in keeping a compact desktop tool understandable as its feature set grows.
