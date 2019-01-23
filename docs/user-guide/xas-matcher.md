# XAS Matcher
## Overview
We have computed X-Ray Absorption (XAS) spectra for over half of the materials in our database, and this number is growing. In particular, we have computed XANES K-edge spectra using the FEFF code. Read more about our methodology for computing spectra here (link to X-Ray Absorption Spectra page) and at the first reference below. We are also in the process of computing other kinds of spectra. This page focuses on use of our app for comparing computed x-ray absorption spectra and automatically matching our spectra against user-uploaded experimental spectra.

Reference for database and validation: [link](#references)

Reference for app: [link](#references)

## Using the App

### Comparing Spectra

You first enter a chemical system to ensure we have spectra calculated. Then, the first few spectra by increasing energy above hull (a proxy for thermodynamic stability) are plotted, and you can toggle plotting of spectra via the results table. You can filter the table by e.g. chemical formula via the search box above the table, and you can change the sorting by clicking on column headers (shift-click to sort secondary to the primary sort).

With an uploaded spectrum and after matching, the <em>P</em><sub>softmax</sub> column is the softmax probability that the given material's spectrum matches the one uploaded according to the match ranking of a suite of metrics. More info in [[#How Matching Works|How Matching Works]].

### Uploading Spectra

Spectra files should have two values per line, separated by a standard delimiter like a comma or tab character. Comment lines (beginning with a '#' are allowed and will be ignored by the parser. The first value on each line should be the energy in units of eV. The second value, the absorption coefficient of arbitrary units, will be max-value normalized for plotting and matching.

## How Matching Works
Coming soon...

## References

* Mathew, K. et al. High-throughput computational X-ray absorption spectroscopy. Sci. Data 5:180151 doi:[https://doi.org/10.1038/sdata.2018.151 10.1038/sdata.2018.151] (2018).

* Zheng, C. et al. Automated generation and ensemble-learned matching of X-ray absorption spectra. npj Computational Materials 12 doi:[http://dx.doi.org/10.1038/s41524-018-0067-x 10.1038/s41524-018-0067-x](2018)

## Authors

Donny Winston
Chen Zheng