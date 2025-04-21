# CosMx_OV 
Analysis workflows, tools, and visualizations for CosMx Spatial Molecular Imager datasets

## This repository used ovarian cancer CosMx (the link included in the raw folder)
## This workflow will be **updated** continually

## ================================
## Author: Ji Wang
## Description: End-to-end script for analyzing CosMx spatial transcriptomics data on ovarian cancer
## ================================


| Step | Title                               | Description                                                                 |
|------|-------------------------------------|------------------------------------------------------------------------------|
| 📁 1 | Setup & Imports                     | - Import libraries  <br> - Define global parameters and paths  <br> - Establish directory tree |
| 📂 2 | Load Input Data                     | - Load CosMx expression matrix  <br> - Load cell metadata and segmentation  <br> - Load FOV positions |
| 🧪 3 | Quality Control                     | - Filter low-quality cells (e.g., low counts, %NegProbe)  <br> - Filter low-confidence genes  <br> - Visualize QC metrics |
| 🧬 4 | Normalization & Transformation      | - Normalize total counts (e.g., CP10K)  <br> - Log-transform expression (log1p) |
| 🧩 5 | Dimensionality Reduction & Clustering | - Identify HVGs  <br> - Perform PCA, compute neighbors  <br> - Generate UMAP and Leiden clusters |
| 🔍 6 | Cell Type Annotation                | - Annotate clusters using known markers or reference signatures  <br> - Visualize expression per cluster |
| 🧭 7 | Spatial Visualization               | - Stitch FOVs using global pixel coordinates  <br> - Overlay marker expression  <br> - Plot spatially resolved clusters |
| 🧪 8 | Advanced Analyses                   | - Spatial analysis  <br> - Ligand-receptor interaction inference |
| 💾 9 | Save Outputs                        | - Save filtered `.h5ad`, plots, stitched images  <br> - Export spatial data and expression matrices |

---
### 8. Advanced Analysis
#### Spatial_analysis_1.ipynb (relate structural characteristics/distances to cell transcriptomics)
#### - Analysis based on selection of cut-off values for determination of cell islands
#### - Analysis based on distances between cell islands and cells
#### - Analysis based on spatial structures

#### Spatial_analysis_2.ipynb (relate structural characteristics/distances to cell transcriptomics)
#### - Analysis based on Squidpy spatial analysis module
#### - Analysis based on fovs
####   - analysis of individual fovs followed by aggregation/analysis of all fovs using global coordinates
####   - analysis on one specific fov

---
## 📚 Citation and Acknowledgment

If you find this repository useful in your work, please consider citing it as:

> Wang, Ji. *CosMx_OV: Spatial Transcriptomics Analysis Pipeline for Ovarian Cancer*. GitHub repository: [https://github.com/gynecoloji/CosMx_OV](https://github.com/gynecoloji/CosMx_OV)




