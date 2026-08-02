---
title: ATLAS pixel data-acquisition software
status: Completed
period: 2019–2023
order: 6
summary: Decoding, validating, and structuring the raw byte stream produced by the ATLAS pixel detector, from firmware-level diagnostics to reconstruction software.
tags: [ATLAS, pixel detector, data acquisition, C++, distributed computing]
---

Before detector data can be used for physics, its binary stream must be decoded and checked against the data-acquisition logic that produced it. My early ATLAS work focused on software for the pixel detector at this hardware–software boundary.

I led a major upgrade of a raw-data analysis package: decoding information from the byte stream, designing structures for persistent storage, and building an analysis layer on top of the decoded records. I also developed workflows for running these checks on Grid and HTCondor resources, allowing larger datasets to be processed systematically.

In a later contribution to the ATLAS pixel byte-stream converter, I implemented summary logging for errors encountered during decoding. Condensing low-level failures into actionable diagnostics helps detector experts distinguish isolated corrupt words from recurring acquisition or configuration problems.

This work gave me a detailed understanding of how detector electronics, firmware formats, offline reconstruction, and distributed software meet in a production experiment.
