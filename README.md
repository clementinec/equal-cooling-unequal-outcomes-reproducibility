# Equal cooling setpoints, unequal thermal outcomes

Minimal public result-reproduction snapshot for the manuscript:

> *Equal cooling setpoints, unequal thermal outcomes: residential cooling
> service under future weather and ageing*

## Download

The versioned
[`review-v3`](https://github.com/clementinec/equal-cooling-unequal-outcomes-reproducibility/releases/tag/review-v3)
release supplies two authenticated archives and their `.sha256` sidecars:

- `reviewer_result_reproduction_v5_compact.tar.gz` — 6,919,913 bytes,
  SHA-256
  `cbe0a744bf39148824f7c8fb7dde54407f7889f412e3a57b2a205061f41a0a86`;
- `reviewer_bem_hourly_v1_author_generated.tar.gz` — 127,442,067 bytes,
  SHA-256
  `3603c4dab978c306d1e01c19601fd0cddb0958582580d960590b43b6e15336f2`.

The compact packet contains the analysis code, authenticated curated inputs
and outputs, tests, model cards, checksums, and documentation needed to
regenerate 16 publication outputs byte-for-byte. The companion contains all
12 author-generated annual hourly BEM Parquet bundles: 1,296 logical cases and
7,568,640 rows.

This is **result reproduction**, not an end-to-end raw-data reconstruction
claim. The release excludes the 144 derived EPWs because the retained weather
chain does not preserve the original provider/version/URL, source-specific
redistribution grant, or complete attribution record. It also excludes
third-party raw comfort observations and the exact 148,148 × 78 prepared
comfort-data table because a redistribution grant was not retained and the
upstream curation record is incomplete. The TSV model therefore cannot be
independently refitted from this release. These boundaries are documented
inside the compact packet.

## Verify and extract

On macOS:

```sh
shasum -a 256 -c reviewer_result_reproduction_v5_compact.tar.gz.sha256
shasum -a 256 -c reviewer_bem_hourly_v1_author_generated.tar.gz.sha256
tar -xzf reviewer_result_reproduction_v5_compact.tar.gz
```

On Linux:

```sh
sha256sum -c reviewer_result_reproduction_v5_compact.tar.gz.sha256
sha256sum -c reviewer_bem_hourly_v1_author_generated.tar.gz.sha256
tar -xzf reviewer_result_reproduction_v5_compact.tar.gz
```

After extraction, begin with
`reviewer_result_reproduction_v5_compact/README.md`, then follow
`RUNBOOK.md`.

## Licensing and archival citation

Original project code is available under the MIT licence. Only the
author-generated result/model-output files enumerated by each archive's
`LICENSE_MATRIX.tsv` are available under CC BY 4.0. TSV-derived,
source-derived and third-party material is excluded from those grants. See
`LICENSING.md`, `LICENSE-DATA.md` and `THIRD_PARTY_NOTICES.md`.

Use `CITATION.cff`, the immutable release tag and the archive SHA-256 when
citing the present review materials.
