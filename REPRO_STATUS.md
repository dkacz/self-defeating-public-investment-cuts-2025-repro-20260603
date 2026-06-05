# Public Reproduction Delivery Report R998

Date: 2026-06-05

Public entry point: https://dkacz.github.io/self-defeating-public-investment-cuts-2025-repro-20260603/lite/lab/index.html?path=notebooks/self_defeating_public_investment_cuts_2025_current_reader_notebook_r966_20260604.ipynb

The public root opens the interactive JupyterLite notebook rather than a frozen rendered notebook page. The shipped notebook fetches official Eurostat and OECD TiVA sources where available, then falls back to packaged snapshots if a source is unavailable.

R998 updates the public manuscript render after Section 1.1 flow repairs. The redundant output-gap sentence was removed, the Poland euro-area sanctions sentence was folded into the Poland paragraph, the standalone DSM baseline opening was replaced with a smoother transition, duplicate projection wording was removed, and unclear baseline meta-language was removed. The notebook calculation remains R966 because this round changes manuscript prose and published render files, not the source-data or estimation logic.

Fresh-source QA:
- Eurostat annual source rows: used_live_official_api; requested end year 2025; actual max year 2025; rows 969.
- OECD TiVA GFCF and consumption import-content shares: used_live_official_api; requested end year 2025; actual max year 2022; rows 1512.
- Ireland 2025 missing financial-account rows: 3.
- Paper-number reference checks consistent: 6/6.
- Checks requiring review: none.

Interpretation for the paper: the current live official data do not change the accepted headline paper numbers. Response paths, debt endpoints, p-value appendix table and uncertainty summary remain consistent with the paper reference. The diagnostic metadata reference has been refreshed to the current notebook values; no paper-number update is required.

Current manuscript hashes:
- PDF: `fea834abe479473107411f528ed0ba28231349e398091bc36d6d9f9a9d21bfe6`
- EPUB: `2f2e581a0db9f1bd5b08745ff588542da24a13982c2446b24d6967c4f0cc1cdd`
- HTML: `cf8ad4b4e8d69ddda4786ab2ae354a27e5f50edc786a5b0c8f9ea4d3da0155e1`
- QMD: `f651a6ea57c9e23afdbed91d4e7eabda58cc77823e39a98efc95256ed0644f96`

Download package SHA-256 is stored in `docs/downloads/full_public_2025_repro_package.zip.sha256`.
