# Genomics Data Analysis and PCA Strategies

This notebook explores different strategies for handling missing values and performing Principal Component Analysis (PCA) on a genomics dataset to identify patterns related to tumor subtypes.

## Data Loading and Initial Exploration

- Loading the dataset.
- Initial data shape and preview.
- Taking a subset of the data (first 200 genes).
- Checking for missing values.

## Strategy 1: Simple Imputation (Naive Approach)

- Imputing missing values using the mean of each gene.
- Performing PCA on the imputed data.
- Analyzing explained variance and cumulative explained variance.
- Identifying top genes contributing to the first two principal components (PC1 and PC2).
- Visualizing PC1 vs PC2 colored by tumor subtype.
- Visualizing PC1 vs PC2 vs PC3 colored by tumor subtype (static and interactive plots).
- Conclusions based on Mean Imputation.

## Strategy 2: Advanced Imputation (Robust Approach)

- Imputing missing values using the k-Nearest Neighbors (k-NN) algorithm.
- Evaluating the best k value for k-NN imputation.
- Performing PCA on the k-NN imputed data.
- Analyzing explained variance.
- Identifying top genes contributing to the first two principal components (PC1 and PC2).
- Visualizing PC1 vs PC2 colored by tumor subtype.
- Visualizing PC1 vs PC2 vs PC3 colored by tumor subtype.
- Conclusions based on k-NN Imputation.

## Strategy 3: Integrated PCA (Advanced)

- Using an integrated PCA method (NIPALS, implemented from scratch) that handles missing values natively.
- Performing PCA using the NIPALS algorithm.
- Analyzing explained variance.
- Identifying top genes contributing to the first two principal components (PC1 and PC2).
- Visualizing PC1 vs PC2 colored by tumor subtype.
- Visualizing PC1 vs PC2 vs PC3 colored by tumor subtype.
- Conclusions based on NIPALS PCA.

## Author

* **Juan Guillermo Gómez**
* Linkedin: [@jggomezt](https://www.linkedin.com/in/jggomezt/)
