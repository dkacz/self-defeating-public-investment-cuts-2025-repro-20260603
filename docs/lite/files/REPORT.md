# Public Reproduction Delivery Report R1002

Date: 2026-06-05

Public entry point: https://dkacz.github.io/self-defeating-public-investment-cuts-2025-repro-20260603/lite/lab/index.html?path=notebooks/self_defeating_public_investment_cuts_2025_current_reader_notebook_r966_20260604.ipynb

The public root opens the interactive JupyterLite notebook rather than a frozen rendered notebook page. The shipped notebook fetches official Eurostat and OECD TiVA sources where available, then falls back to packaged snapshots if a source is unavailable.

R1002 updates the public manuscript render after targeted Section 1.1 and Section 1.2 wording repairs. The phrase `the next paragraphs explain why its assumptions are too demanding`, the closing `Commission construction` paragraph, and the Section 1.2 opening phrase `The point matters because...` were removed. `Scenario exercise` was replaced with a plainer reference to the analysis, interest and growth wording was unpacked, the DSM structural balance is reported exactly at -9.9 percent of GDP, and the Section 1.2 opening no longer suggests that the Commission DSA is internally consistent. The debt stabilisation sentence now separates the method source from the Commission baseline numbers and removes the `not a judgement...` construction. The notebook calculation remains R966 because this round changes manuscript prose and published render files, not the source-data or estimation logic.

Fresh-source QA:
- Eurostat annual source rows: used_live_official_api; requested end year 2025; actual max year 2025; rows 969.
- OECD TiVA GFCF and consumption import-content shares: used_live_official_api; requested end year 2025; actual max year 2022; rows 1512.
- Ireland 2025 missing financial-account rows: 3.
- Paper-number reference checks consistent: 6/6.
- Checks requiring review: none.

Interpretation for the paper: the current live official data do not change the accepted headline paper numbers. Response paths, debt endpoints, p-value appendix table and uncertainty summary remain consistent with the paper reference. The diagnostic metadata reference has been refreshed to the current notebook values; no paper-number update is required.

Current manuscript hashes:
- PDF: `b599ec4ff4b3bb8b1aab3e789c09eb6235c17f473b0a77ac7d0681af0f8583c3`
- EPUB: `4947bd56cc863b28ea8235bfb5e069427fb7a9878a74ea427c877b29792a6281`
- HTML: `24d30bdf650774d60ef2e252a3ade4e225c31f79fa86806126849b55fe6c5572`
- QMD: `45cb6d26e0531ca424cc079b058fe02de7467bd3d14dc92efaee6d4c28396c90`

Download package SHA-256 is stored in `docs/downloads/full_public_2025_repro_package.zip.sha256`.
