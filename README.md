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
  
<img width="1233" height="547" alt="image" src="https://github.com/user-attachments/assets/1c14e56b-834e-4750-a9b3-615e6f3e3b7e" />
<img width="3166" height="855" alt="image" src="https://github.com/user-attachments/assets/fef6ff5d-c043-4ff9-ae7c-15b2b0b1cc43" />
<img width="1489" height="590" alt="image" src="https://github.com/user-attachments/assets/3d888875-033d-483f-b93a-075224fc26b1" />
<img width="1001" height="790" alt="image" src="https://github.com/user-attachments/assets/3f5e7380-642e-4119-819e-4c8b1715fc20" />
<img width="1773" height="525" alt="newplot" src="https://github.com/user-attachments/assets/1248b003-2f88-46c4-951f-83363ed71265" />

## Strategy 2: Advanced Imputation (Robust Approach)

- Imputing missing values using the k-Nearest Neighbors (k-NN) algorithm.
- Evaluating the best k value for k-NN imputation.
- Performing PCA on the k-NN imputed data.
- Analyzing explained variance.
- Identifying top genes contributing to the first two principal components (PC1 and PC2).
- Visualizing PC1 vs PC2 colored by tumor subtype.
- Visualizing PC1 vs PC2 vs PC3 colored by tumor subtype.
- Conclusions based on k-NN Imputation.

<img width="1036" height="701" alt="image" src="https://github.com/user-attachments/assets/ab038148-bb4a-41ca-b8ee-02cae3335834" />
<img width="1233" height="547" alt="image" src="https://github.com/user-attachments/assets/c28fb5e0-fb12-44c2-8008-a3d06bcc1f07" />
<img width="2004" height="701" alt="image" src="https://github.com/user-attachments/assets/918d2a54-a7f6-4b58-88aa-d686d5d4ac3c" />
<img width="1489" height="590" alt="image" src="https://github.com/user-attachments/assets/47e62ad4-ae40-4a3d-8213-847be4d90ac3" />
<img width="1001" height="790" alt="image" src="https://github.com/user-attachments/assets/58acd0b8-8650-4b48-8ee0-578f282a716e" />
<img width="1773" height="525" alt="newplot (1)" src="https://github.com/user-attachments/assets/d9a55e29-89f6-4c21-b327-e07988eee245" />

## Strategy 3: Integrated PCA (Advanced)

- Using an integrated PCA method (NIPALS, implemented from scratch) that handles missing values natively.
- Performing PCA using the NIPALS algorithm.
- - Performing PCA using PPCA.
- Analyzing explained variance.
- Identifying top genes contributing to the first two principal components (PC1 and PC2).
- Visualizing PC1 vs PC2 colored by tumor subtype.
- Visualizing PC1 vs PC2 vs PC3 colored by tumor subtype.
- Conclusions based on NIPALS and PPCA.

### NIPALs
<img width="1233" height="547" alt="image" src="https://github.com/user-attachments/assets/a6eaa2f9-ab1a-4d70-9b4f-0a49aa815a30" />
<img width="1616" height="701" alt="image" src="https://github.com/user-attachments/assets/0bbd037c-c2a8-402d-bab9-687666116c49" />
<img width="1489" height="590" alt="image" src="https://github.com/user-attachments/assets/be7c6066-5d97-49e5-892e-1e2a7d426e77" />
<img width="1001" height="790" alt="image" src="https://github.com/user-attachments/assets/892fc76d-0358-4d32-bdb1-aa6df4e0f1b5" />
<img width="1773" height="525" alt="newplot (2)" src="https://github.com/user-attachments/assets/905ab55c-67bb-4d57-b6e0-a7221f7f99d1" />

### PPCA
<img width="1233" height="548" alt="image" src="https://github.com/user-attachments/assets/c565b9b1-4d3d-4cda-bfca-2303f1a1da6b" />
<img width="1616" height="701" alt="image" src="https://github.com/user-attachments/assets/e1659080-1046-412a-94f9-d7595b6a1309" />
<img width="1489" height="590" alt="image" src="https://github.com/user-attachments/assets/b651507f-6f32-4860-9f79-7652dbeafd74" />
<img width="1001" height="790" alt="image" src="https://github.com/user-attachments/assets/3fff1f34-2c08-43cd-a351-eba811fb2eab" />
<img width="1773" height="525" alt="newplot (3)" src="https://github.com/user-attachments/assets/7bb825d2-f575-4848-9757-9dfea7d037f2" />


## Author

* **Juan Guillermo Gómez**
* Linkedin: [@jggomezt](https://www.linkedin.com/in/jggomezt/)
