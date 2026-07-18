# Equal cooling setpoints, unequal thermal outcomes

Minimal reviewer reproducibility snapshot for the manuscript:

> *Equal cooling setpoints, unequal thermal outcomes: residential cooling
> service under future weather and ageing*

## Download

Download `reviewer_reproducibility_v4_compact.tar.gz` from the repository's
latest GitHub release. Its SHA-256 sidecar is available both in the release and
at the repository root.

The archive is 9,048,487 bytes and contains 128 files after extraction. It
includes the analysis code, focused tests, curated derived result tables,
figure/table provenance, compact building-model inputs, and documentation
needed to inspect the reported revision analyses.

To keep this review snapshot small, it excludes private correspondence,
third-party raw comfort observations, and the optional large hourly-weather
data tiers. The archive records checksums and provenance for the excluded
optional tiers.

## Verify and extract

On macOS:

```sh
shasum -a 256 -c reviewer_reproducibility_v4_compact.tar.gz.sha256
tar -xzf reviewer_reproducibility_v4_compact.tar.gz
```

On Linux:

```sh
sha256sum -c reviewer_reproducibility_v4_compact.tar.gz.sha256
tar -xzf reviewer_reproducibility_v4_compact.tar.gz
```

Expected SHA-256:

```text
1f325715b5e0b94fa9ca5ce194bdde1ce7cf8fcab991f47078f0d186455005cc
```

After extraction, begin with
`reviewer_reproducibility_v4/manuscript_energy/revision/reproducibility_packet/README.md`
and the adjacent `RUNBOOK.md`.

## Deposit status

This repository is a public peer-review snapshot. A permanent archival DOI and
reuse licence have not yet been assigned. Unless a licence is added later, no
reuse permission is granted beyond applicable law.
