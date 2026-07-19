# Third-party notices and excluded rights

The packet contains original project code and author-generated model outputs,
but it also documents or derives results from third-party sources. The project
licences do not grant rights that their copyright holder does not control.

## pythermalcomfort

`code/scripts/build_gagge_age_physiology_report.py` contains a vectorized,
extended implementation adapted from the algorithm and update order in
`pythermalcomfort` 3.9.8, particularly
`pythermalcomfort.models.two_nodes_gagge_ji`. The project modifications and
extensions are released under MIT, and the upstream MIT notice is retained
below.

> MIT License
>
> Copyright (c) 2019 Federico Tartarini
>
> Permission is hereby granted, free of charge, to any person obtaining a copy
> of this software and associated documentation files (the "Software"), to
> deal in the Software without restriction, including without limitation the
> rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
> sell copies of the Software, and to permit persons to whom the Software is
> furnished to do so, subject to the following conditions:
>
> The above copyright notice and this permission notice (including the next
> paragraph) shall be included in all copies or substantial portions of the
> Software.
>
> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
> IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
> FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
> AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
> LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
> OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
> SOFTWARE.

Source: <https://github.com/CenterForTheBuiltEnvironment/pythermalcomfort>.

## UN World Population Prospects

Raw UN World Population Prospects records are not redistributed. Some
population-weighted result tables contain author-generated aggregates
calculated from WPP inputs. CC BY 4.0 applies only to the author's original
analysis, selection and arrangement where the licence matrix says so; it does
not replace or modify the UN source terms.

## Thermal-comfort observations and TSV artefacts

Raw thermal-comfort observations and the prepared 148,148 × 78 fitting table
are excluded. Fitted coefficients, bootstrap results and other TSV-derived
artefacts in the compact review packet are marked
`LicenseRef-Pending-Third-Party-Rights` until the source-data redistribution
terms and required attribution are confirmed.

## Climate data and EPWs

The selected future-weather chain uses CMIP6 MPI-ESM1-2-LR source data. The
144 derived EPW files are excluded because a source-specific redistribution
grant and complete attribution record for the underlying climate files were
not retained. This deposit therefore cannot authorize redistribution of those
files and grants no climate-source or EPW reuse right. Author-generated BEM
results may be licensed separately without licensing their underlying weather
inputs. The retained evidence is documented inside the compact packet.

## EnergyPlus and Python dependencies

The packet does not redistribute EnergyPlus, pythermalcomfort, NumPy, pandas,
SciPy, scikit-learn, statsmodels, matplotlib, joblib, pytest or pyarrow
binaries. Their versions are recorded for reproducibility; each dependency
remains governed by its own licence. Generated EnergyPlus input files and
author-generated BEM outputs are covered only where `LICENSE_MATRIX.tsv`
explicitly says so.
