# Public Reproduction Delivery Report R995

Date: 2026-06-05

Public entry point: https://dkacz.github.io/self-defeating-public-investment-cuts-2025-repro-20260603/lite/lab/index.html?path=notebooks/self_defeating_public_investment_cuts_2025_current_reader_notebook_r966_20260604.ipynb

The public root opens the interactive JupyterLite notebook rather than a frozen rendered notebook page. The shipped notebook fetches official Eurostat and OECD TiVA sources where available, then falls back to packaged snapshots if a source is unavailable.

R995 updates the public manuscript render after the operator-approved abstract wording tweak. The notebook calculation remains R966 because this round changes manuscript prose and published render files, not the source-data or estimation logic.

Fresh-source QA:
- Eurostat annual source rows: used_live_official_api; requested end year 2025; actual max year 2025; rows 969.
- OECD TiVA GFCF and consumption import-content shares: used_live_official_api; requested end year 2025; actual max year 2022; rows 1512.
- Ireland 2025 missing financial-account rows: 3.
- Paper-number reference checks consistent: 6/6.
- Checks requiring review: none.

Interpretation for the paper: the current live official data do not change the accepted headline paper numbers. Response paths, debt endpoints, p-value appendix table and uncertainty summary remain consistent with the paper reference. The diagnostic metadata reference has been refreshed to the current notebook values; no paper-number update is required.

Current manuscript hashes:
- PDF: `7b3dcaf2731a11df2150587782840b56294d4e67b5e847826d286dd2346e6e32`
- EPUB: `44c34185815a8ca8053c65a2425d69468226f493b5eb163701a458ddec5f3f47`
- QMD: `a38fa429c12f9b8861ecb2603bb386ea322e08b043e66fa34096d5c3ac86eefc`

Download package SHA-256 is stored in `docs/downloads/full_public_2025_repro_package.zip.sha256`; current ZIP SHA-256: `3295d32a771c56411f53542a75e07d49631d9de3c9b2bb383c7559cdbcf0fb86`.
