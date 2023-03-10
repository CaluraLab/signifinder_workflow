signifinder Workflow: Bulk, Single-cell and Spatial Transcriptomics
================

<!-- README.md is generated from README.Rmd. Please edit that file -->

This repository contains the scripts for data processing, signature
computation and figure generation using bulk, single-cell (SC) and
spatial transcriptomics (ST) RNA-Seq data, reported at
<https://www.biorxiv.org/content/10.1101/2023.03.07.530940v1>.

<img src=./signifinder_main_figure.png />

A single .Rmd file is provided for each dataset analysis.

The spatial transcriptomic dataset “Human Breast Cancer: Ductal
Carcinoma In Situ, Invasive Carcinoma (FFPE)”, from the 10x Genomics
Visium Spatial Gene Expression data (<https://www.10xgenomics.com>), is
already provided in the Data folder as a `SpatialExperiment`. The object
already includes the spot annotation of the histology image, performed
by an expert anatomopathologist.

## Required Packages

The `signifinder` package can be installed from Bioconductor:

``` r
if (!require("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

BiocManager::install("signifinder")
```

Further, to run the workflows, the `curatedTCGAData`, `EDASeq`,
`GEOquery`, `ggpubr`, `ggspavis`, `grid`, `NbClust`, `org.Hs.eg.db`,
`RColorBrewer`, `scater`, `scone`, `TMExplorer` R packages are required.

## Documentation and Contacts

Further details on how to use `signifinder` are available in the
[vignette](https://bioconductor.org/packages/release/bioc/vignettes/signifinder/inst/doc/signifinder.html),
that includes examples and documentation.

For any problems in using `signifinder`, please write to
<stefania.pirrotta@phd.unipd.it>.
