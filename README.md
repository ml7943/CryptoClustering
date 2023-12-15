# CryptoClustering

## Overview

This project aims to perform clustering analysis on cryptocurrency market data using K-Means clustering. It involves data preprocessing, scaling, feature reduction with Principal Component Analysis (PCA), and K-Means clustering to identify patterns and group cryptocurrencies based on their market behavior.

## Project Structure

- **Data Preprocessing**: The original market data is loaded, cleaned, and scaled using StandardScaler from scikit-learn.
- **Principal Component Analysis (PCA)**: Reducing the dimensions of the data to three principal components using PCA.
- **K-Means Clustering**:
  - **Elbow Method**: Determining the optimal number of clusters using the elbow method on both the original and PCA-transformed data.
  - **Clustering**: Performing K-Means clustering with the optimal number of clusters obtained from the elbow method.
  - **Visualization**: Visualizing the clustered results using scatter plots and comparing the outcomes with and without PCA.

## Usage

1. **Setup**:
   - Ensure required libraries are installed (`pandas`, `scikit-learn`, `matplotlib`, `hvplot`).
   - Store the cryptocurrency market data in a CSV file (`crypto_market_data.csv`).

2. **Run the Code**:
   - Execute the provided Python script or Jupyter Notebook cells sequentially to perform the analysis.

## Results and Observations

- **Elbow Method Analysis**:
  - Without PCA: The elbow curve shows variations in inertia values, suggesting an optimal number of clusters.
  - With PCA: The elbow curve demonstrates inertia values, aiding in determining an optimal number of clusters after dimensionality reduction.

- **Clustering Analysis**:
  - Comparison between clusters obtained with and without PCA: Visualized clusters to observe differences in clustering results after dimensionality reduction.

- **Impact of Dimensionality Reduction**:
  - Using fewer features (with PCA): Shows trade-offs between retaining data information and decreasing computational costs, impacting clustering quality and interpretability.

## Conclusion

- Dimensionality reduction techniques like PCA influence clustering outcomes by compressing data information.
- The choice between fewer features and clustering quality requires balancing data preservation and computational efficiency.

## Author and Date
`Mu Li`
`12/14/2023`
