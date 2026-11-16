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

Tagore Radio plays Rabindra Sangeet and recordings of Rabindranath Tagore. An installable static web app connects to a FastAPI service that selects tracks, resolves public audio, and keeps listeners on the same current song.

## Catalogue and playback

The catalogue draws from Wikimedia Commons and Internet Archive, retaining source and license information. Rotation uses normalized composition titles to avoid repeating a song under different performers or filenames. Recordings in Tagore's voice have a separate station and also appear periodically in the mixed station.

A home-hosted backend connects through a Cloudflare tunnel, with a hosted Render service as fallback. The browser shows when the endpoint changes.

## Recognition and lyrics

A Linux desktop companion samples audio, identifies it with SongRec, and finds Bengali lyrics on Geetabitan or Tagoreweb. Matching accounts for transliteration, performer prefixes, spelling variants, and uploads titled by album rather than song.
