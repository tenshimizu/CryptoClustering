# Crypto Clustering Analysis

## Overview

This project performs a cluster analysis of cryptocurrency market data using K-Means clustering and Principal Component Analysis (PCA). The goal is to identify distinct groupings of cryptocurrencies based on their price change percentages over various timeframes.

## Files

*   `crypto_market_data.csv`:  The dataset containing cryptocurrency market data, including price change percentages over different periods.
*   `Crypto_Clustering.ipynb`:  The Jupyter Notebook containing the analysis code.
*   `Resources/`: This folder should contain the CSV.
*   `README.md`: This file, providing an overview of the project.

## Dependencies

*   pandas
*   scikit-learn
*   matplotlib (implicitly used by pandas plotting)

## Execution

1.  Ensure that the `crypto_market_data.csv` file is located in the `Resources/` directory.
2.  Run the `Crypto_Clustering.ipynb` script in a Python environment with the installed dependencies.

## Methodology

The analysis follows these steps:

1.  **Data Preparation:** Load the data, normalize it using `StandardScaler`, and prepare it for clustering.
2.  **Finding Optimal k (Original Data):** Use the elbow method to determine the optimal number of clusters (k) for K-Means clustering on the original scaled data.
3.  **K-Means Clustering (Original Data):** Cluster the cryptocurrencies using K-Means with the chosen `k` value and visualize the clusters using a scatter plot.
4.  **Principal Component Analysis (PCA):** Apply PCA to reduce the dimensionality of the data to three principal components.
5.  **Finding Optimal k (PCA Data):**  Use the elbow method again to find the optimal `k` for K-Means clustering on the PCA-transformed data.
6.  **K-Means Clustering (PCA Data):** Cluster the cryptocurrencies using K-Means with the chosen `k` value on the PCA data and visualize the clusters.
7.  **Feature Weight Analysis:** Determine the weights of each original feature on each principal component to understand their influence.

## Results

The analysis identifies distinct clusters of cryptocurrencies based on their price movements. PCA helps to reduce the complexity of the data while retaining significant variance, allowing for more efficient clustering.  The optimal number of clusters is determined using the elbow method, both for the original data and the PCA-transformed data.

## Key Findings

*   The optimal number of clusters (k) was found to be 4.
*   PCA effectively reduces the dimensionality of the data while preserving a high percentage of the variance.
*   The analysis reveals the features that have the strongest influence on each principal component, providing insights into the underlying factors driving the clustering.

## Author

[Erin Spencer-Priebe]


