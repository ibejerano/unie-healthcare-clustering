# breast_cancer_clustering_GSE2034

**Academic, reproducible pipeline** for unsupervised clustering of breast cancer patients using GSE2034 microarray dataset (286 primary tumors, 22,283 Affymetrix HG-U133A probes) from NCBI GEO.

**Purpose**: End-to-end analysis emphasizing **leakage-proof preprocessing**, **MCAR validation (χ² p>0.05)**, **PCA dimensionality reduction (50 PCs, 53.6% variance)**, and robust **clustering (k=3, silhouette=0.094 KMeans/0.072 Ward, ARI=-0.002±0.005)**. **Reveals weak molecular structure** with **post-hoc χ² p=0.03 relapse association** (C0:25% vs C2:8%, OR 0.35-0.17). Interprets under **exploratory framework**, establishing methodological benchmark for transcriptomic subgroup discovery absent strong prognostic signal.

## Project Structure
```bash
.
├── datasets/
│   ├── LICENSE                                 # Public domain License (NCBI GEO dataset)
│   └── GSE2034_series_matrix.txt           
├── src/
│   └── breast_cancer_clustering_GSE2034.ipynb  # Complete executable pipeline
├── requirements.txt
├── LICENSE                                     # MIT License (code)
└── README.md

```

## Copyright and License

- **© 2026 Isabel Bejerano-Blazquez**
- **Notebook**: MIT License
- **Data**: Public domain (NCBI GEO) License

Developed and tested on:

- **Python ≥ 3.12**  
- **Dependencies:** see requirements.txt file

## Quick start

```bash
## Create and activate environment
python3 -m venv venv
source venv/bin/activate      # macOS/Linux
venv\Scripts\activate         # Windows

# Install dependencies
pip install -r requirements.txt  

# Run notebook
jupyter notebook breast_cancer_clustering_GSE2034.ipynb
```

**Disclaimer**: Provided *as is*, for academic use only.