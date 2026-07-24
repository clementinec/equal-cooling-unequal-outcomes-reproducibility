# Review-v6 release

This release adds an independently executable public-source reconstruction
and refit check for the empirical thermal-sensation-vote (TSV) analysis.

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
publication outputs byte-for-byte and passes 46 self-contained tests, with
five full-project checks explicitly deselected.

The Chinese OSF record is publicly downloadable but declares no explicit
dataset licence, so its files are downloaded directly and hash-verified rather
than redistributed. ASHRAE Database II v2.1.0 is CC0. The existing EPW
redistribution boundary and the separately checksummed hourly BEM companion
remain unchanged.

Compact archive:

- file: `reviewer_result_reproduction_v6_compact.tar.gz`
- bytes: `6,946,667`
- SHA-256:
  `efcb9cf34cf2e59c6177873ded0f0b8543064297a8ba073ac8e139d4011c4421`
