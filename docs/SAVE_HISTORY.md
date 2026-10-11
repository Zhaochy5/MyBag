# Public data repository history

This history records the files committed to the public GitHub data repository. Full datasets are distributed as versioned Release attachments. This repository is separate from the authors' local manuscript workspace.

## 1A Initialize the public data index

- Date: 2026-10-11
- Branch: main
- Previous save point: none
- Goal: establish a history for the reproducibility-data repository.
- File: `docs/SAVE_HISTORY.md`.
- Change: add this public repository history; numerical data remain in the separately prepared Release archive.
- Validation: inspect the Markdown content and the upload file list; the file contains no credentials, private contact details or manuscript correspondence.
- Remaining work: add the verified data-package instructions and publish the checked ZIP as a versioned Release.
- Commit message: `1A Initialize public reproducibility repository history`.

## 2A Add the verified release instructions

- Date: 2026-10-11
- Branch: main
- Previous save point: 1A
- Goal: make the full data package and checking commands easy to find.
- Files: `docs/README.md`, `docs/README_zh.md`, `docs/SAVE_HISTORY.md`.
- Change: add English and Chinese download instructions, the saved-data checking commands and the experimentally evaluated scope. The complete ZIP is a Release attachment, separate from GitHub's automatic source-code ZIP.
- Validation: 370 file identities, 24 complete episodes, 211000 training rows, 1055 validation evaluations, 90 saved runs, 1530 recomputed metrics and matched references/disturbances passed the local checks. All original numerical arrays, result tables, figure PDFs and historical functional records retain their bytes. Checkpoint edits only remove one machine-location string in each file; all tensor storage is unchanged. Content scans found no machine paths, credentials, private contact details or review correspondence.
- Prepared asset: `SNN_Quadrotor_Reproducibility_v1.0.0.zip`, 216938108 bytes, 373 files.
- ZIP SHA256: `bf858a91bc3fdaf4a6dade29f01f2075efdcd3f1c41c09a2a73ff233659a6210`.
- Remaining work: upload the verified ZIP and checksum as Release v1.0.0, then verify the public download. New simulations and retraining are separate tasks; this commit records no new experimental result. No additional reuse license is assigned.
- Commit message: `2A Add verified data download and reproducibility instructions`.
