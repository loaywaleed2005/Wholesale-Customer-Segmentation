# Wholesale Customer Segmentation

An unsupervised machine learning project for segmenting wholesale customers based on annual spending behavior across different product categories.

## Project Overview

This project analyzes the Wholesale Customers dataset and groups customers into meaningful segments using multiple clustering algorithms.

The analysis compares:

- K-Means Clustering
- Spectral Clustering
- Gaussian Mixture Models

The goal is to identify customer groups with similar purchasing patterns and support business decisions such as targeted marketing and customer profiling.

## Dataset

The dataset includes annual spending across the following product categories:

- Fresh
- Milk
- Grocery
- Frozen
- Detergents and Paper
- Delicatessen

The `Channel` and `Region` columns are excluded from clustering because they are categorical identifiers.

## Data Preparation

The workflow includes:

- Dataset inspection
- Missing-value analysis
- Duplicate detection
- Outlier detection using the IQR method
- Feature selection
- Standardization using `StandardScaler`

## Dimensionality Reduction

The project uses:

- Principal Component Analysis
- t-SNE

PCA is used for explained-variance analysis and cluster visualization.

## Clustering Algorithms

### K-Means

K-Means is evaluated using:

- K = 2
- K = 3
- K = 4

The Elbow Method is used to estimate the optimal number of clusters.

### Spectral Clustering

Spectral Clustering is applied using an RBF affinity matrix and compared across multiple values of K.

### Gaussian Mixture Model

Gaussian Mixture Models are used to support probabilistic and flexible cluster assignments.

## Evaluation Metrics

The clustering algorithms are compared using:

- Silhouette Score
- Calinski-Harabasz Score
- Davies-Bouldin Index
- Dunn Index

## Key Findings

- K-Means provided the strongest and most interpretable results.
- Three clusters produced a useful balance between quality and interpretability.
- One segment showed high Grocery and Milk spending.
- Another segment showed high Fresh and Frozen spending.
- A third segment demonstrated more balanced spending behavior.

## Business Applications

The customer segments can support:

- Targeted marketing
- Personalized promotions
- Customer profiling
- Inventory planning
- Product bundling
- Customer relationship management

## Technologies

- Python
- Pandas
- NumPy
- Scikit-learn
- SciPy
- Matplotlib
- Seaborn
- Google Colab

## Project File

Open `Wholesale_Customer_Segmentation.ipynb` to view the complete preprocessing, visualization, clustering, evaluation, and interpretation workflow.

## Author

Loay Waleed
