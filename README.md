# CosMx_OV (Please download the script to check because some of them has exceeded the max rendering size in github)
Analysis workflows, tools, and visualizations for CosMx Spatial Molecular Imager datasets

## This repository used ovarian cancer CosMx (the link included in the raw folder)
## This workflow will be **updated** continually

# ================================
# Author: Ji Wang
# Description: End-to-end script for analyzing CosMx spatial transcriptomics data on ovarian cancer
# ================================

# --------------------------------
# 📁 1. Setup & Imports
# - Import libraries
# - Define global parameters and paths
# - Establish directory tree
# --------------------------------

# --------------------------------
# 📂 2. Load Input Data
# - Load CosMx expression, metadata, FOV positions, segmentation files
# --------------------------------

# --------------------------------
# 🧪 3. Quality Control
# - Filter low-quality cells (e.g., low counts, %NegProbe)
# - Filter low-confidence genes
# - Visualize QC metrics
# --------------------------------

# --------------------------------
# 🧬 4. Normalization & Transformation
# - Normalize total counts 
# - Log-transform gene expression
# --------------------------------

# --------------------------------
# 🧩 5. Dimensionality Reduction & Clustering
# - Identify HVGs
# - PCA, neighbors, UMAP
# - Leiden clustering
# --------------------------------

# --------------------------------
# 🔍 6. Cell Type Annotation
# - Annotate clusters using known markers/ref. gene signature matrix
# - Visualize cluster
# --------------------------------

# --------------------------------
# 🧭 7. **Spatial Visualization**
# - Stitch FOVs using global pixel coordinates
# - Overlay marker expression on tissue
# - Plot spatially resolved clusters
# --------------------------------

# --------------------------------
# 🧪 8. **Advanced Analyses**
# - Spatial co-occurrence and enrichment
# - Cell-cell interaction (e.g., ligand-receptor)
# --------------------------------

# --------------------------------
# 💾 9. Save Outputs
# - Save filtered data, plots, stitched images
# - Export various types of spatial, expression matrix and adata files
# --------------------------------
