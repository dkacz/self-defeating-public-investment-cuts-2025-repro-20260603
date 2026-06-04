# Public Reproduction Delivery Report R967

Date: 2026-06-04

Public entry point: https://dkacz.github.io/self-defeating-public-investment-cuts-2025-repro-20260603/lite/lab/index.html?path=notebooks/self_defeating_public_investment_cuts_2025_current_reader_notebook_r966_20260604.ipynb

The public root now opens the interactive JupyterLite notebook rather than a frozen rendered notebook page. The shipped notebook fetches official Eurostat and OECD TiVA sources where available, then falls back to packaged snapshots if a source is unavailable.

Fresh-source QA:
- Eurostat annual source rows: used_live_official_api; requested end year 2025; actual max year 2025; rows 969.
- OECD TiVA GFCF and consumption import-content shares: used_live_official_api; requested end year 2025; actual max year 2022; rows 1512.
- Ireland 2025 missing financial-account rows: 3.
- Paper-number reference checks consistent: 5/6.
- Checks requiring review: model-admission screen.

Interpretation for the paper: the current live official data do not change the accepted headline paper numbers. Response paths, debt endpoints, p-value appendix table and uncertainty summary remain consistent with the paper reference. The only alert is a tiny live-Eurostat drift in diagnostic metadata, so it is documented as a monitoring issue rather than a paper-number update.

Download package SHA-256 is stored in `docs/downloads/full_public_2025_repro_package.zip.sha256`.
