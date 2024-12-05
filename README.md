# Single-Cell RNA-Seq Analysis with Seurat

## Overview

This course provides a crash introduction to Single-Cell/Nuclei RNA Sequencing (from now on scRNA-seq) using the Seurat R package. Participants will learn the necessary steps for analyzing scRNA-seq data, including quality control, normalization, clustering, and annotation of cell types.

## Prerequisites

To be able to follow along you need to have a basic understanding of R programming and and single cell RNA-seq expression data. Familiarity with R Studio, ggplot2 and dplyr is highly recommended. Also navigating around the file system and loading data will be helpful. [R for Data Science](https://r4ds.hadley.nz/) is a great resource for learning R programming.

## Contents

1.  **Introduction to Single-Cell RNA Sequencing (scRNA-seq)**
    -   Overview of scRNA-seq technology
    -   scRNA-seq workflow
2.  **Setting Up the Environment**
    -   Required packages
    -   Loading packages
3.  **Loading and Preprocessing Data**
    -   Loading data
    -   Quality control
    -   Doublet removal
    -   Final outlier filtering
4.  **Normalization and Scaling**
    -   Normalization techniques
    -   Finding variable features
    -   Scaling data
5.  **Dimensionality Reduction and Clustering**
    -   Principal Component Analysis (PCA)
    -   Clustering and visualization
    -   Integration using Harmony
6.  **Annotating Clusters**
    -   Canonical markers
    -   Identifying marker genes
7. **Extras**
    -   Pathway Analysis with clusterProfiler
    -   Identifying number of clusters
    -   Cell Cycle Analysis
    -   Species classification


## Installation

Make sure you have the required R packages installed:

``` r
# Install required packages

install.packages(c("Seurat", "dplyr", "ggplot2", "robustbase", "tibble", "viridis", "patchwork", "remotes"))


# The following packages are part of Bioconductor, so you'll need to set up Bioconductor to install them
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")
BiocManager::install(c("SingleR", "scRNAseq", "org.Hs.eg.db", "scater", "clusterProfiler"))

# DoubletFinder and harmonu is not available in Rs standard repositories, so we need to install them from GitHub
remotes::install_github('chris-mcginnis-ucsf/DoubletFinder')
remotes::install_github("immunogenomics/harmony")




```

## Usage

1.  If you have git installed on your computer you can clone this repository to your local machine:

``` bash
git clone https://github.com/pettestor/scRNA-seq-1day-course.git
cd scRNA-seq-analysis
```

If you dont have git installed you can download the course content by clicking the green "code" button on the top right of this page and selecting "Download ZIP". 

2.  Open [scRNAseq-course.qmd](https://github.com/pettestor/scRNA-seq-1day-course/blob/main/scRNAseq-course.qmd) in R Studio and follow the instructions for analyzing your scRNA-seq data.


## Author

Petter Storm
