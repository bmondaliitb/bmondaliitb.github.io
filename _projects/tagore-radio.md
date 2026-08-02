---
title: Tagore Radio
kind: Web, API, and desktop app
stack: Python · FastAPI · JavaScript
mark: TR
accent: amber
order: 2
featured: true
summary: A continuous Rabindra Sangeet radio with shared playback, Bengali lyric lookup, and a small desktop companion.
image: /assets/images/tagore-artwork.webp
image_alt: Monochrome line illustration from the public-domain Tagore artwork collection used by Tagore Radio.
image_caption: One of the historical illustrations used as quiet visual accompaniment in the radio interface.
---

Tagore Radio is a small internet-radio system for Rabindra Sangeet and recordings of Rabindranath Tagore. A static, installable web app talks to a FastAPI service that chooses tracks, resolves playable public audio, and maintains a shared station state so listeners hear the same current song.

## A resilient catalogue

The backend builds a reusable catalogue from Wikimedia Commons and Internet Archive recordings, keeping source and license information with each track. It rotates by normalized composition title rather than raw filename, which avoids presenting the same song as new simply because another singer recorded it. Archival recordings in Tagore's own voice form a separate station and periodically appear in the mixed station.

The project can use a home-hosted backend through a Cloudflare tunnel and fall back to a hosted Render service when the primary endpoint is unavailable. The browser reflects that change rather than silently failing.

## Recognition and lyrics

The Linux desktop companion can sample the current audio, identify it through SongRec, and match the result to Bengali lyrics from Geetabitan or Tagoreweb. Matching has to cope with transliteration, performer prefixes, alternative spellings, and cases where an upload title describes an album rather than an individual composition.

The repository is currently private, so this page describes the project without exposing a dead or inaccessible code link.
