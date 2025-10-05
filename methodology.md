Methodology (example synthetic data)

- Generated a synthetic expression matrix with 3000 genes and 100 samples (50 AD, 50 Control).
- Planted 15 hub genes that produce correlated signals across subsets of target genes.
- For network inference, used Pearson correlation and a hard threshold of 0.7 on absolute correlation.
- Hub genes were identified by degree (number of connections) in the thresholded network.

Notes:
- For real data, consider more robust GRN tools (ARACNe, GENIE3, CLR) and statistical validation (permutation tests, bootstrapping).
- Always preprocess (normalization, batch correction) real microarray/RNA-seq data before network inference.
