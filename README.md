# Equal cooling setpoints, unequal thermal outcomes

Minimal public reproducibility materials for the manuscript:

> *Equal cooling setpoints, unequal thermal outcomes: residential cooling
> service under future weather and ageing*

## Download

The versioned
[`review-v6`](https://github.com/clementinec/equal-cooling-unequal-outcomes-reproducibility/releases/tag/review-v6)
release supplies the compact archive and its SHA-256 sidecar. The unchanged
hourly companion remains available as the verified `review-v4` asset:

- `reviewer_result_reproduction_v6_compact.tar.gz` — 6,909,846 bytes,
  SHA-256
  `904a1a98d7590689cf2ece4725c6f1e21f918a5e40c31c124f657daf2df3fc50`;
- [`reviewer_bem_hourly_v1_author_generated.tar.gz`](https://github.com/clementinec/equal-cooling-unequal-outcomes-reproducibility/releases/download/review-v4/reviewer_bem_hourly_v1_author_generated.tar.gz) — 127,442,067 bytes,
  SHA-256
  `3603c4dab978c306d1e01c19601fd0cddb0958582580d960590b43b6e15336f2`.

The compact packet regenerates 16 publication outputs byte-for-byte and
passes 49 self-contained tests, with five full-project checks explicitly
deselected. It also provides a clean public-source reconstruction of the
empirical thermal-sensation-vote analysis:

- ASHRAE Global Thermal Comfort Database II v2.1.0 is pinned to
  [Dryad DOI 10.6078/D1F671](https://doi.org/10.6078/D1F671) and its CC0
  source files;
- the Chinese Thermal Comfort Dataset is pinned to
  [OSF DOI 10.17605/OSF.IO/D465N](https://doi.org/10.17605/OSF.IO/D465N);
- exact filenames, download endpoints, hashes, field mappings, cleaning rules,
  and executable build/refit commands are included; and
- the workflow rebuilds 148,148 rows into a 36-column model-ready view and
  independently refits all 258 coefficients across five reported branches.
  The maximum absolute difference from the released coefficients is
  `9.410250356722827e-13`.

The Chinese OSF record is publicly downloadable but does not declare an
explicit dataset licence. Its files are therefore fetched directly from OSF
and hash-verified rather than redistributed in the archive. The 144 derived
EPWs also remain excluded because the retained weather-source record does not
establish the source-specific attribution and reuse terms needed for
redistribution. Weather-selection manifests, generated EnergyPlus inputs, and
the complete author-generated hourly BEM outputs are available.

## Packaging correction

On 24 July 2026, the compact `review-v6` asset was rebuilt in place to remove
local workflow documents and non-portable path metadata that were unrelated
to the scientific record. The clean packet adds a completed physiology QA
record and exact inventory/content gates. All 16 publication-reproduction
targets and the curated scientific result assets are unchanged. The
superseded package had SHA-256
`efcb9cf34cf2e59c6177873ded0f0b8543064297a8ba073ac8e139d4011c4421`;
the governing checksum is the one listed above.

## Verify and extract

On macOS:

```sh
shasum -a 256 -c reviewer_result_reproduction_v6_compact.tar.gz.sha256
tar -xzf reviewer_result_reproduction_v6_compact.tar.gz
```

On Linux:

```sh
sha256sum -c reviewer_result_reproduction_v6_compact.tar.gz.sha256
tar -xzf reviewer_result_reproduction_v6_compact.tar.gz
```

After extraction, begin with
`reviewer_result_reproduction_v6_compact/README.md`, then follow
`RUNBOOK.md` and `TSV_REPRODUCIBILITY.md`.

## Licensing and citation

Original project code is available under the MIT licence. Enumerated
author-generated result and model-output files are available under CC BY 4.0;
the archive's `LICENSE_MATRIX.tsv` controls the file-level scope. No project
licence is asserted for third-party observations or excluded weather files.
See `LICENSING.md`, `LICENSE-DATA.md`, and `THIRD_PARTY_NOTICES.md`.

Use `CITATION.cff`, the versioned release tag, and the archive SHA-256 when
citing these materials.
