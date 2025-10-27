# Genomics Data Analysis and PCA Strategies

This notebook explores strategies for handling missing values and performing Principal Component Analysis (PCA) on a genomics dataset to identify patterns associated with tumor subtypes.

## Data Loading and Initial Exploration

- Loading the dataset.
- Initial data shape and preview.
- Evaluate the genes with the most support for variance
- Checking for missing values.

## Strategy 1: Simple Imputation (Naive Approach)

- Imputing missing values using the mean of each gene.
- Performing PCA on the imputed data.
- Analyzing explained variance and cumulative explained variance.
- Identifying top genes contributing to the first two principal components (PC1 and PC2).
- Visualizing PC1 vs PC2 colored by tumor subtype.
- Visualizing PC1 vs PC2 vs PC3 colored by tumor subtype (static and interactive plots).
- Conclusions based on Mean Imputation.
  
<img width="1233" height="547" alt="strategy1-cumulative-explained" src="https://github.com/user-attachments/assets/d15071c1-5456-4191-85ed-a74499f75741" />
<img width="1616" height="701" alt="strategy1-2" src="https://github.com/user-attachments/assets/a406cfa2-800f-4bcb-bb5c-c0af4a6b4e64" />
<img width="1001" height="790" alt="strategy1-5" src="https://github.com/user-attachments/assets/392debc0-7a58-46c3-becd-b744f55f49f1" />


## Strategy 2: Advanced Imputation (Robust Approach)

- Imputing missing values using the k-Nearest Neighbors (k-NN) algorithm.
- Evaluating the best k value for k-NN imputation.
- Performing PCA on the k-NN imputed data.
- Analyzing explained variance.
- Identifying top genes contributing to the first two principal components (PC1 and PC2).
- Visualizing PC1 vs PC2 colored by tumor subtype.
- Visualizing PC1 vs PC2 vs PC3 colored by tumor subtype.
- Conclusions based on k-NN Imputation.

<img width="1027" height="701" alt="strategy2-1" src="https://github.com/user-attachments/assets/17428867-c026-4274-87cb-76176d01a063" />
<img width="1233" height="547" alt="strategy2-2" src="https://github.com/user-attachments/assets/0e17d977-7bcc-422a-8228-ad45b02afebc" />
<img width="1001" height="790" alt="strategy2-6" src="https://github.com/user-attachments/assets/3c0a07d5-07a1-4698-8b7c-849a12966b98" />
<img width="1508" height="858" alt="Screenshot 2025-10-22 at 7 39 07 p m" src="https://github.com/user-attachments/assets/eeba6eb4-7ce3-48b8-9ebf-9e492f35bc87" />


## Strategy 3: Integrated PCA (Advanced)

- Using an integrated PCA method (NIPALS, implemented from scratch) that handles missing values natively.
- Performing PCA using the NIPALS algorithm.
- - Performing PCA using PPCA.
- Analyzing explained variance.
- Identifying top genes contributing to the first two principal components (PC1 and PC2).
- Visualizing PC1 vs PC2 colored by tumor subtype.
- Visualizing PC1 vs PC2 vs PC3 colored by tumor subtype.
- Conclusions based on NIPALS and PPCA.

<img width="1233" height="547" alt="strategy3-NIPALS-1" src="https://github.com/user-attachments/assets/6d71cac2-b212-4771-86d2-e531183fe26e" />
<img width="1001" height="790" alt="strategy3-NIPALS-6" src="https://github.com/user-attachments/assets/ea6cac80-65f2-4e7c-ae7a-682eb026d388" />


<img width="1233" height="548" alt="strategy3-PPCA-1" src="https://github.com/user-attachments/assets/8fbcf022-5a87-4d5b-8f1d-198a187b04d8" />

<img width="1616" height="701" alt="strategy3-PPCA-nuevo" src="https://github.com/user-attachments/assets/025bfc2a-13b3-46a0-805f-e0b75baad03d" />

<img width="1001" height="790" alt="strategy3-PPCA-5" src="https://github.com/user-attachments/assets/e2c50c63-b5ab-477c-a116-38ef438f15e8" />


## Author

* **Juan Guillermo Gómez**
* Linkedin: [@jggomezt](https://www.linkedin.com/in/jggomezt/)
