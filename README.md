# Transcriptomic Meta-Analysis Pipeline 
This repository contains an R-based meta-analysis and bioinformatics pipeline designed for integrating cross-study transcriptomic 
datasets (RNA-seq). The workflow performs differential expression meta-analysis, random-effects modeling (`metafor`), cross-study 
correlation matrices, and hierarchical clustering visualizations.

## Project Structure

```text
├── R/                          # R scripts for processing, meta-analysis, and plotting
├── data/                       # Processed inputs / expression matrices 
├── output/                     # Generated tables, correlation matrices, and figures
└── README.md
Random-Effects Meta-Analysis: Fits restricted maximum likelihood (REML) models using metafor to pool log2 fold changes across multiple
 independent studies.

Cross-Study Concordance: Computes pairwise Spearman correlation matrices of log2 fold changes.

Visualization: Generates forest plots for individual genes and clustered heatmaps using pheatmap and RColorBrewer.

