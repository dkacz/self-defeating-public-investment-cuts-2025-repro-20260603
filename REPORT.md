# Public Reproduction Delivery Report R996

Date: 2026-06-05

Public entry point: https://dkacz.github.io/self-defeating-public-investment-cuts-2025-repro-20260603/lite/lab/index.html?path=notebooks/self_defeating_public_investment_cuts_2025_current_reader_notebook_r966_20260604.ipynb

The public root opens the interactive JupyterLite notebook rather than a frozen rendered notebook page. The shipped notebook fetches official Eurostat and OECD TiVA sources where available, then falls back to packaged snapshots if a source is unavailable.

R996 updates the public manuscript render after removing a redundant output-gap sentence from Section 1.1. The notebook calculation remains R966 because this round changes manuscript prose and published render files, not the source-data or estimation logic.

Fresh-source QA:
- Eurostat annual source rows: used_live_official_api; requested end year 2025; actual max year 2025; rows 969.
- OECD TiVA GFCF and consumption import-content shares: used_live_official_api; requested end year 2025; actual max year 2022; rows 1512.
- Ireland 2025 missing financial-account rows: 3.
- Paper-number reference checks consistent: 6/6.
- Checks requiring review: none.

Interpretation for the paper: the current live official data do not change the accepted headline paper numbers. Response paths, debt endpoints, p-value appendix table and uncertainty summary remain consistent with the paper reference. The diagnostic metadata reference has been refreshed to the current notebook values; no paper-number update is required.

Current manuscript hashes:
- PDF: `7fc8227f31b4bd8e1c0d852b8e4558800b7a75da73e55d586166f89e042344ad`
- EPUB: `21c3797994847cfe00768cbf2881312c5f499a24a19e868c84114f312108cdac`
- QMD: `a5dd13d6327ac9230339ca733e8be7a910274e78ba4e5d2acc0c23177669a835`

Download package SHA-256 is stored in `docs/downloads/full_public_2025_repro_package.zip.sha256`; current ZIP SHA-256: `70e9e0c9fa94bb1bc66b4206dfd1ae4679bbc35cd6c3523ccd9ef71098719248`.
