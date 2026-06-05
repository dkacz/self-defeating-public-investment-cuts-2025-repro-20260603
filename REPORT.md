# Public Reproduction Delivery Report R993

Date: 2026-06-05

Public entry point: https://dkacz.github.io/self-defeating-public-investment-cuts-2025-repro-20260603/lite/lab/index.html?path=notebooks/self_defeating_public_investment_cuts_2025_current_reader_notebook_r966_20260604.ipynb

The public root opens the interactive JupyterLite notebook rather than a frozen rendered notebook page. The shipped notebook fetches official Eurostat and OECD TiVA sources where available, then falls back to packaged snapshots if a source is unavailable.

R993 updates the public manuscript render after the operator-approved abstract logic rewrite. The notebook calculation remains R966 because this round changes manuscript prose and published render files, not the source-data or estimation logic.

Fresh-source QA:
- Eurostat annual source rows: used_live_official_api; requested end year 2025; actual max year 2025; rows 969.
- OECD TiVA GFCF and consumption import-content shares: used_live_official_api; requested end year 2025; actual max year 2022; rows 1512.
- Ireland 2025 missing financial-account rows: 3.
- Paper-number reference checks consistent: 6/6.
- Checks requiring review: none.

Interpretation for the paper: the current live official data do not change the accepted headline paper numbers. Response paths, debt endpoints, p-value appendix table and uncertainty summary remain consistent with the paper reference. The diagnostic metadata reference has been refreshed to the current notebook values; no paper-number update is required.

Current manuscript hashes:
- PDF: `e60574f2580d7537b3ef24ba2298c1385107abaa77977dfabc73c3fee5aca745`
- EPUB: `988511ccf76b1ef5891497cf8a5de37f93862b20ff07769921538e2587743007`
- QMD: `06feb4b183b7055ee51f3d7c85a660a95953f1fa7d69de896273d3d57a24ce78`

Download package SHA-256 is stored in `docs/downloads/full_public_2025_repro_package.zip.sha256`; current ZIP SHA-256: `05e3d752c950f0de99ee9b38ef6ca0325531f326b4393deb8c10d473dadd1fc1`.
