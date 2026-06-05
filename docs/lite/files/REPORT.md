# Public Reproduction Delivery Report R997

Date: 2026-06-05

Public entry point: https://dkacz.github.io/self-defeating-public-investment-cuts-2025-repro-20260603/lite/lab/index.html?path=notebooks/self_defeating_public_investment_cuts_2025_current_reader_notebook_r966_20260604.ipynb

The public root opens the interactive JupyterLite notebook rather than a frozen rendered notebook page. The shipped notebook fetches official Eurostat and OECD TiVA sources where available, then falls back to packaged snapshots if a source is unavailable.

R997 updates the public manuscript render after Section 1.1 flow repairs. The redundant output-gap sentence was removed, the Poland euro-area sanctions sentence was folded into the Poland paragraph, the standalone DSM baseline opening was replaced with a smoother transition, and duplicate projection wording was removed. The notebook calculation remains R966 because this round changes manuscript prose and published render files, not the source-data or estimation logic.

Fresh-source QA:
- Eurostat annual source rows: used_live_official_api; requested end year 2025; actual max year 2025; rows 969.
- OECD TiVA GFCF and consumption import-content shares: used_live_official_api; requested end year 2025; actual max year 2022; rows 1512.
- Ireland 2025 missing financial-account rows: 3.
- Paper-number reference checks consistent: 6/6.
- Checks requiring review: none.

Interpretation for the paper: the current live official data do not change the accepted headline paper numbers. Response paths, debt endpoints, p-value appendix table and uncertainty summary remain consistent with the paper reference. The diagnostic metadata reference has been refreshed to the current notebook values; no paper-number update is required.

Current manuscript hashes:
- PDF: `6a171d1c3efafa14c7a3f661b64aee7f41e3adb23c88e4933c3adcc9b8689dea`
- EPUB: `281b0c3bf32b0510a4f4f65c44a582eb59c1b9e78c73fd39e1cea3c1916eb3a8`
- HTML: `1305b831740e39fa00b763ee6ee543752e33c1582b34d4ac3b7ae786df5c2565`
- QMD: `12a081d5b0f5f5b98346ca3b6194fe8b93c7e5e76f9ddf694482fe42e522583e`

Download package SHA-256 is stored in `docs/downloads/full_public_2025_repro_package.zip.sha256`.
