# Review-v6 release

This release adds an independently executable public-source reconstruction
and refit check for the empirical thermal-sensation-vote (TSV) analysis.

## Packaging correction (24 July 2026)

The compact asset was rebuilt in place to remove local workflow documents and
non-portable path metadata that were unrelated to the scientific record. The
clean packet adds a completed physiology QA record, its executable trajectory
test, and fail-closed exact inventory/content checks. The 16 publication
reproduction targets and curated scientific result assets are unchanged.

The superseded package had SHA-256
`efcb9cf34cf2e59c6177873ded0f0b8543064297a8ba073ac8e139d4011c4421`.
The governing package checksum is given below.

The compact archive now includes:

- checksum-pinned source manifests for ASHRAE Global Thermal Comfort Database
  II v2.1.0 and the Chinese Thermal Comfort Dataset;
- a downloader that rejects source-file hash mismatches;
- documented field alignment, cleaning, and derived-variable rules;
- reconstruction of the 148,148-row, 36-column model-ready training view;
- independent refitting of all 258 coefficients across five reported
  age-specification branches; and
- five additional reconstruction-contract tests.

The verified maximum absolute coefficient difference is
`9.410250356722827e-13`. The complete compact-packet gate regenerates 16
publication outputs byte-for-byte and passes 49 self-contained tests, with
five full-project checks explicitly deselected.

The Chinese OSF record is publicly downloadable but declares no explicit
dataset licence, so its files are downloaded directly and hash-verified rather
than redistributed. ASHRAE Database II v2.1.0 is CC0. The existing EPW
redistribution boundary and the separately checksummed hourly BEM companion
remain unchanged.

Compact archive:

- file: `reviewer_result_reproduction_v6_compact.tar.gz`
- bytes: `6,909,846`
- SHA-256:
  `904a1a98d7590689cf2ece4725c6f1e21f918a5e40c31c124f657daf2df3fc50`
