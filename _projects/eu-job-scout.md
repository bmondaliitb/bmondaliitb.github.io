---
title: EU Job Scout
kind: Personal web app
stack: Python · FastAPI · SQLite
mark: EU
accent: blue
order: 5
featured: true
summary: A local-first vacancy collector that ranks jobs against a chosen profile and CV while making source coverage explicit.
---

EU Job Scout collects vacancies from documented APIs and public feeds, normalizes them, removes duplicates, and ranks each role against a local profile. Country selection covers the EU while still allowing genuinely Europe-wide or worldwide-remote positions to surface.

## Transparent matching

The ranking combines desired roles, explicit skills, overlap with extracted CV text, work-style and location preferences, and excluded terms. Each result explains its score instead of presenting an unexplained recommendation. The source panel also shows which providers are configured, what geographic coverage they offer, when each was last crawled, and any exact provider error.

## Local by design

The profile and extracted CV text stay in a local SQLite database. The app has no accounts and is intended to bind to the loopback interface unless authentication and HTTPS are added.

The crawler deliberately uses documented feeds or APIs and does not automate sources whose terms prohibit unapproved scraping. One provider can fail without blocking the others, and adapters are replaceable as access conditions change.

This personal tool is not currently published on GitHub.
