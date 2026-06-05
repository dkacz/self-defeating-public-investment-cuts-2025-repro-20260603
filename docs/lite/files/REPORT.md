# Public Reproduction Delivery Report R999

Date: 2026-06-05

Public entry point: https://dkacz.github.io/self-defeating-public-investment-cuts-2025-repro-20260603/lite/lab/index.html?path=notebooks/self_defeating_public_investment_cuts_2025_current_reader_notebook_r966_20260604.ipynb

The public root opens the interactive JupyterLite notebook rather than a frozen rendered notebook page. The shipped notebook fetches official Eurostat and OECD TiVA sources where available, then falls back to packaged snapshots if a source is unavailable.

R999 updates the public manuscript render after targeted Section 1.1 and Section 1.2 wording repairs. The phrase `the next paragraphs explain why its assumptions are too demanding`, the closing `Commission construction` paragraph, and the Section 1.2 opening phrase `The point matters because...` were removed. The baseline paragraph restores the DSM structural-balance endpoint near -10 percent of GDP in compact form. The notebook calculation remains R966 because this round changes manuscript prose and published render files, not the source-data or estimation logic.

Fresh-source QA:
- Eurostat annual source rows: used_live_official_api; requested end year 2025; actual max year 2025; rows 969.
- OECD TiVA GFCF and consumption import-content shares: used_live_official_api; requested end year 2025; actual max year 2022; rows 1512.
- Ireland 2025 missing financial-account rows: 3.
- Paper-number reference checks consistent: 6/6.
- Checks requiring review: none.

Interpretation for the paper: the current live official data do not change the accepted headline paper numbers. Response paths, debt endpoints, p-value appendix table and uncertainty summary remain consistent with the paper reference. The diagnostic metadata reference has been refreshed to the current notebook values; no paper-number update is required.

Current manuscript hashes:
- PDF: `061dd70c55ceea9b3943c91d7a427b1a160291c868fd85aa3472a5aca4506bd5`
- EPUB: `dfe458fa9fbc0630db343736a27b294237ea1e7cb2e9ad6c0fbecc9f5e783ff7`
- HTML: `355fd92a436149404c46f7f7171483334c8ab17c10c0dc4f7533fc6f3f11ca16`
- QMD: `42a0ddcd1ee3e2d56e60c65ea2b65de7366684031484d33962a83b92618fc022`

Download package SHA-256 is stored in `docs/downloads/full_public_2025_repro_package.zip.sha256`.
