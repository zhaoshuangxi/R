Image processing and analysis toolbox for R
Bioconductor version: Release (3.9)

EBImage provides general purpose functionality for image processing and analysis. In the context of (high-throughput) microscopy-based cellular assays, EBImage offers tools to segment cells and extract quantitative cellular descriptors. This allows the automation of such tasks using the R programming language and facilitates the use of other tools in the R environment for signal processing, statistical modeling, machine learning and visualization with image data.

Author: Andrzej Oleś, Gregoire Pau, Mike Smith, Oleg Sklyar, Wolfgang Huber, with contributions from Joseph Barry and Philip A. Marais

Maintainer: Andrzej Oleś <andrzej.oles at embl.de>

Citation (from within R, enter citation("EBImage")):

Installation
To install this package, start R (version "3.6") and enter:

if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

BiocManager::install("EBImage")
For older versions of R, please refer to the appropriate Bioconductor release.

Documentation
To view documentation for the version of this package installed in your system, start R and enter:

browseVignettes("EBImage")
