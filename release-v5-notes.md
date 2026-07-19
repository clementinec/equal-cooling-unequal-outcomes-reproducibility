This release clarifies the storage arithmetic of the author-generated hourly
BEM companion; no scientific result, fitted model, table, figure or archived
hourly value changed.

The companion contains 12 Parquet bundles covering 864 unique annual BEM state
series and 7,568,640 hourly rows. Because the fan pathway reuses the
free-running EnergyPlus state, these series represent 1,296 logical
system-pathway cases. The 432 fan cases are aliases in the case index, not
missing or duplicated annual state series.

The compact packet regenerates 16 publication outputs byte-for-byte from the
included curated derived data. Its hermetic packet command passes 41 tests and
deselects five explicitly labelled full-project-only checks.

This is result reproduction, not an end-to-end raw-data reconstruction claim.
The documented EPW, thermal-comfort, prepared-TSV and upstream-provenance
boundaries are unchanged.
