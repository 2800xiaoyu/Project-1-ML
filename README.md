# Project-1-ML

The project includes vegetation community analysis and RF modelling

1. Data Sources
Multitemporal high-resolution UAV imagery (preprocessed)
Vegetation inventory tables (cleaned)

2. Vegetation Community Analysis
Fuzzy K-means clustering
NMDS ordination → NMDS scores & cluster membership values
Indicator species analysis → Identify diagnostic species
Plant functional type (PFT) assignment

3. Spectral Data Extraction
Create buffers for field plots (90) + pure water points (20)
Extract spectral bands (Blue, Green, Red, RedEdge, NIR)
Compute vegetation indices (NDVI, NDWI, NDRE, EVI, SAVI)
Prepare spectral & index layers for each UAV date (and combined)

4. Training Dataset Assembly
Final training data table includes:
Plot ID | Cluster | NMDS | Membership| PFT | Spectral values | Vegetation indices

5. Machine Learning (Random Forest)
Predict NMDS scores from spectral values & indices
Predict membership values
Predict PFT proportions
Classify vegetation clusters
