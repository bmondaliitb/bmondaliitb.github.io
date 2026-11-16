---
title: ATLAS pixel data-acquisition software
status: Completed
period: 2019–2023
order: 6
summary: Decoding, validating, and structuring the raw byte stream produced by the ATLAS pixel detector, from firmware-level diagnostics to reconstruction software.
tags: [ATLAS, pixel detector, data acquisition, C++, distributed computing]
---

I upgraded an ATLAS pixel raw-data analysis package to decode the binary stream, store the decoded records, and analyze them. I also developed Grid and HTCondor workflows to process larger datasets.

For the pixel byte-stream converter, I implemented summary logging of decoding errors. These diagnostics help detector experts distinguish isolated corrupt words from recurring acquisition or configuration problems.

The work spanned detector electronics, firmware formats, offline reconstruction, and distributed computing.
