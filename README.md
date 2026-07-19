# Equal cooling setpoints, unequal thermal outcomes

Minimal public result-reproduction snapshot for the manuscript:

> *Equal cooling setpoints, unequal thermal outcomes: residential cooling
> service under future weather and ageing*

## Download

Download `reviewer_result_reproduction_v5_compact.tar.gz` and its `.sha256`
sidecar from the repository's latest GitHub release. The sidecar is also kept
at the repository root.

The 6,898,927-byte archive contains the analysis code, authenticated curated
inputs and outputs, tests, model cards, checksums, and documentation needed to
regenerate the revision's publication tables from the included derived data.
Its isolated reproduction check regenerated 16 outputs byte-for-byte.

This is a compact **result-reproduction** packet, not an end-to-end
reproducibility claim. It excludes the 144 derived EPW files, full hourly BEM
archive, third-party raw comfort observations, and the exact row-level
prepared comfort-data table used for the empirical TSV fit. The TSV model
therefore cannot be independently refitted from this archive. The included
documentation records these boundaries explicitly.

## Verify and extract

On macOS:

```sh
shasum -a 256 -c reviewer_result_reproduction_v5_compact.tar.gz.sha256
tar -xzf reviewer_result_reproduction_v5_compact.tar.gz
```

On Linux:

```sh
sha256sum -c reviewer_result_reproduction_v5_compact.tar.gz.sha256
tar -xzf reviewer_result_reproduction_v5_compact.tar.gz
```

Expected SHA-256:

```text
16f79f61b20366c90d667bebbfbad2af75869890fe4595a27465be3282a7e61b
```

After extraction, begin with
`reviewer_result_reproduction_v5_compact/README.md`, then follow
`RUNBOOK.md`.

## Deposit status

This repository is a public peer-review snapshot. A permanent archival DOI and
reuse licence have not yet been assigned. Unless a licence is added later, no
reuse permission is granted beyond applicable law.
