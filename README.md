# Single-Cell RNA-Seq Analysis with Seurat

## Overview

This course provides a comprehensive introduction to Single-Cell RNA Sequencing (scRNA-seq) using the Seurat R package. Participants will learn the necessary steps for analyzing scRNA-seq data, including quality control, normalization, clustering, and annotation of cell types.

## Prerequisites

To be able to follow along you need to have a basic understanding of R programming and gene expression data. Familiarity with R Studio, ggplot2 and dplyr is recommended. [R for Data Science](https://r4ds.hadley.nz/) is a great resource for learning R programming.

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

## Installation

Make sure you have the required R packages installed:

``` r
install.packages("Seurat")
install.packages("dplyr")
install.packages("ggplot2")
install.packages("robustbase")
install.packages("scater")
install.packages("DoubletFinder")
install.packages("skimr")
install.packages("harmony")
```

## Usage

1.  Clone this repository to your local machine:

``` bash
git clone https://github.com/your_username/scRNA-seq-analysis.git
cd scRNA-seq-analysis
```

If you dont have git installed you can download the course content by clicking the green "code" button and selecting "Download ZIP".

2.  Open the R script and follow the instructions for analyzing your scRNA-seq data.

## License

This project is licensed under the MIT License.

## Author

Petter Storm
