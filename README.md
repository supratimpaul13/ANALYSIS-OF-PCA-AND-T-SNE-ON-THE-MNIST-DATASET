# ANALYSIS OF PCA AND T-SNE ON THE MNIST DATASET
## Comparative Study of PCA and t-SNE on the MNIST Dataset

This repository contains my **M.Tech (CSE) Second Semester project** that presents a
comparative study of **Principal Component Analysis (PCA)** and
**t-Distributed Stochastic Neighbor Embedding (t-SNE)** applied to the MNIST
handwritten digit dataset.

The project focuses on understanding the **theoretical foundations**, **algorithmic steps**,
and **practical behavior** of both linear and non-linear dimensionality reduction techniques.

---

## Project Overview

High-dimensional data such as images suffer from the curse of dimensionality, making
visualization and learning difficult. Dimensionality reduction techniques help project
data into lower dimensions while preserving meaningful structure.

This project compares:
- **PCA** – a linear technique preserving global variance
- **t-SNE** – a non-linear technique preserving local neighborhood structure
- **Hybrid PCA–t-SNE** – PCA for initial reduction followed by t-SNE for efficient visualization

---

## Objectives

- Study the internal working of PCA and t-SNE
- Compare global vs local structure preservation
- Analyze computational complexity and runtime behavior
- Evaluate clustering quality using silhouette score
- Implement a hybrid PCA–t-SNE pipeline for faster visualization

---

## Dataset

- **MNIST handwritten digit dataset**
- 70,000 grayscale images (28 × 28)
- Each image flattened into a 784-dimensional vector
- Pixel values normalized to [0, 1]

---

## Methodology

### Principal Component Analysis (PCA)
- Mean centering and normalization
- Covariance matrix computation
- Eigenvalue–eigenvector decomposition
- Projection onto top-k principal components
- Reconstruction and error analysis

### t-Distributed Stochastic Neighbor Embedding (t-SNE)
- Pairwise similarity computation in high-dimensional space
- Probability distribution modeling using perplexity
- KL-divergence minimization using gradient descent
- Non-linear 2D embedding for visualization

### Hybrid PCA–t-SNE
- PCA reduces data to 50 dimensions
- t-SNE applied on reduced data
- Achieves faster computation with strong cluster separation

---

## Results and Discussion

- **PCA** is fast, deterministic, and preserves global variance but struggles with local clusters
- **t-SNE** reveals well-separated local clusters but is computationally expensive
- **Hybrid PCA–t-SNE** provides a good balance between speed and visualization quality

Performance metrics such as runtime, silhouette score, and reconstruction error are
reported and compared in the project report.

---
