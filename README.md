# Human Brain Gene Regulatory Network Analysis (GSE5281) — Example Project

**Note:** This repository contains *synthetic, example* results created for demonstration and presentation purposes. The plots and hub genes below are generated from a simulated expression matrix — they are not derived from the real GSE5281 dataset.

## What this example includes
- Synthetic expression matrix: `data/processed/expression_synthetic.csv`
- Sample metadata (groups AD vs Control): `data/processed/sample_metadata.csv`
- PCA plot of samples: `results/figures/pca_samples.png`
- Top hub genes CSV: `results/hub_genes.csv`
- Hub barplot, heatmap, and network snapshot in `results/figures/`

## Quick preview

PCA:  
![PCA samples](results/figures/pca_samples.png)

Top hubs barplot:  
![Top hubs barplot](results/figures/top20_hub_genes_bar.png)

Heatmap of top hubs:  
![Heatmap top hubs](results/figures/heatmap_top_hubs.png)

Network snapshot:  
![Network snapshot](results/figures/network_top_hubs.png)

## How to reproduce (high-level)
1. Place your real expression matrix (genes as rows; samples as columns) in `data/raw/` and name it `expression.csv`.
2. Run `python src/preprocessing.py` to preprocess the data (script placeholder provided).
3. Run `python src/network_construction.py` to infer GRN (correlation-based or with recommended tools like ARACNe/GENIE3/CLR).
4. Run `python src/hub_gene_identification.py` and `python src/visualization.py` to generate hub lists and figures.
