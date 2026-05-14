# rna-seq-deseq2-workflow

## Reproducible RNA-seq Differential Expression and Reporting Workflow

This repository contains an end-to-end RNA-seq differential expression and downstream reporting workflow developed in R and Python using a publicly available influenza infection dataset (GSE203539).

The project combines upstream RNA-seq differential expression analysis using DESeq2 with downstream workflows for data consolidation, annotation, visualization, and exploratory reporting, designed to support reproducible bioscience data analysis.

## Analytical Objective

RNA-seq differential expression workflows often generate fragmented outputs across multiple tools, making downstream interpretation, reporting, and reproducibility difficult to standardize.

This project explores how reproducible R and Python workflows can improve quality control, differential expression analysis, downstream data consolidation, and the efficiency of biological reporting for RNA-seq datasets.

The workflow emphasizes:
- transparent QC and outlier assessment
- reproducible differential expression analysis
- standardized DEG aggregation across contrasts
- scalable reporting and visualization workflows
- interpretable downstream biological summaries

---

## Dataset

Public RNA-seq dataset:

- GEO accession: GSE203539
- Model: Influenza A virus (IAV) infection in mouse lung cell populations
- Cell types:
  - Alveolar epithelial cells (AEC)
  - Alveolar macrophages (AM)

Experimental comparisons include:

- WSN vs Mock
- WSN_PP1 vs WSN

---

## Workflow Structure

```text
rna-seq-deseq2-workflow/
│
├── README.md
├── environment.yml
├── data/
├── scripts/
│   ├── DESeq2_GSE203539_portfolio_revised.Rmd
│   └── helper_functions.R
├── notebooks/
│   └── downstream_reporting_and_go_analysis.ipynb
├── results/
│   ├── figures/
│   ├── tables/
│   └── deg_outputs/
└── docs/
```

---

## Methods Summary

### Upstream RNA-seq Analysis (R)

- DESeq2 differential expression workflow
- PCA and sample distance diagnostics
- Outlier sensitivity analysis
- Volcano plots and heatmaps
- DEG filtering and summary reporting

### Downstream Reporting and Analysis (Python)

- Consolidation of annotated DEG outputs
- Metadata cleaning and aggregation
- Cross-contrast DEG summaries
- Exploratory annotation text mining
- Reporting-focused visualizations and export utilities

---

## Key Tools and Libraries

### R
- DESeq2
- ggplot2
- pheatmap
- EnhancedVolcano
- tidyverse

### Python
- pandas
- NumPy
- matplotlib
- seaborn
- scikit-learn

---

## Reproducibility

This repository is organized to support reproducible analysis and reporting workflows.

The workflow documents:
- sample QC procedures
- sensitivity analyses
- filtering decisions
- DEG thresholds
- exported intermediate and final outputs

---

## Repository Goals

This project was developed to demonstrate:
- reproducible bioscience data workflows
- RNA-seq differential expression analysis
- structured QC and analytical reasoning
- downstream reporting automation
- integration of R and Python workflows for scientific data analysis
