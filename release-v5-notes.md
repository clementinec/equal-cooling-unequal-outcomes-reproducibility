This release clarifies the storage arithmetic of the author-generated hourly
BEM companion; no scientific result, fitted model, table, figure or archived
hourly value changed.

The unchanged
[hourly companion](https://github.com/clementinec/equal-cooling-unequal-outcomes-reproducibility/releases/download/review-v4/reviewer_bem_hourly_v1_author_generated.tar.gz)
contains 12 Parquet bundles covering 864 unique annual BEM state series and
7,568,640 hourly rows. Because the fan pathway reuses the free-running
EnergyPlus state, these series represent 1,296 logical system-pathway cases.
The 432 fan cases are aliases in the case index, not missing or duplicated
annual state series. Its SHA-256 remains
`3603c4dab978c306d1e01c19601fd0cddb0958582580d960590b43b6e15336f2`.

The compact packet regenerates 16 publication outputs byte-for-byte from the
included curated derived data. Its hermetic packet command passes 41 tests and
deselects five explicitly labelled full-project-only checks.

This is result reproduction, not an end-to-end raw-data reconstruction claim.
The documented EPW, thermal-comfort, prepared-TSV and upstream-provenance
boundaries are unchanged.
