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
    -   Finding variable features & Scaling data
5.  **Dimensionality Reduction and Clustering**
    -   Principal Component Analysis (PCA)
    -   Clustering and visualization
    -   Integration using Harmony
6.  **Saving your processed object**
7.  **Annotating Clusters**
    -   Canonical markers
    -   Identifying marker genes
    -   Automated annotation using singleR
    -   Automated annotation using Seurats labeltransfer
8. **Extras**
    -   Pathway Analysis with clusterProfiler
    -   Identifying number of clusters
    -   Cell Cycle Analysis
    -   Species classification


## Installation

Make sure you have the required R packages installed:

``` r
# Install CRAN packages
install.packages(c("Seurat", "dplyr", "ggplot2", "robustbase", "patchwork", "devtools", 
                   "scRNAseq", "SingleR", "tibble", "viridis", "clusterProfiler"))

# Install Bioconductor packages
if (!requireNamespace("BiocManager", quietly = TRUE)) {
  install.packages("BiocManager")
}
BiocManager::install(c("scater", "harmony", "org.Hs.eg.db"))

# Install DoubletFinder from GitHub (since it is not available on CRAN)
devtools::install_github("chris-mcginnis-ucsf/DoubletFinder")
```

## Usage

1.  If you have git installed on your computer you can clone this repository to your local machine:

``` bash
git clone https://github.com/pettestor/scRNA-seq-1day-course.git
cd scRNA-seq-1day-course/
```

If you dont have git installed you can download the course content by clicking the green "code" button on the top right of this page and select [Download ZIP] or click this [link](https://github.com/pettestor/scRNA-seq-1day-course/archive/refs/heads/main.zip). 

2.  Open the scRNAseq-course.html file in your prefered browser. In R Studio, navigate to the folder where you have the course content, start a new script and follow scRNAseq-course.html.


## Author

Petter Storm
