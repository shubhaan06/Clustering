# Iris Dataset Clustering Analysis

![Iris Dataset]([https://archive.ics.uci.edu/ml/assets/MLimages/Large53.jpg](https://archive.ics.uci.edu/ml/datasets/iris))

This project explores different clustering techniques on the famous Iris dataset, comparing various preprocessing methods and clustering algorithms to find the optimal grouping of iris flowers based on their morphological characteristics.

## 📌 Table of Contents
- [Project Overview](#-project-overview)
- [Features](#-features)
- [Algorithms Used](#-algorithms-used)
- [Preprocessing Methods](#-preprocessing-methods)
- [Evaluation Metrics](#-evaluation-metrics)
- [Results](#-results)
- [Installation](#-installation)
- [Usage](#-usage)
- [Contributing](#-contributing)
- [License](#-license)

## 🌟 Project Overview

The goal of this project is to:
1. Implement and compare multiple clustering algorithms
2. Evaluate different preprocessing techniques
3. Determine the optimal clustering configuration for the Iris dataset
4. Provide a framework for reproducible clustering experiments

## ✨ Features

- **Comprehensive preprocessing pipeline** with 6 different transformation approaches
- **Three clustering algorithms** for comparative analysis
- **Automated evaluation** using multiple validation metrics
- **Optimal configuration selection** through normalized scoring

## 🧠 Algorithms Used

1. **K-Means** - Centroid-based partitioning algorithm
2. **Agglomerative Hierarchical Clustering** - Bottom-up hierarchical approach
3. **Gaussian Mixture Models (GMM)** - Probabilistic model-based clustering

## 🔧 Preprocessing Methods

| Method        | Description                          |
|---------------|--------------------------------------|
| Raw           | Original data without transformation|
| Normalized    | Min-max scaling (0-1 range)          |
| Log Transform | Natural log transformation           |
| PCA           | Principal Component Analysis (2D)    |
| T+N           | Log transform + Normalization        |
| T+N+PCA       | Log → Normalize → PCA                |

## 📊 Evaluation Metrics

1. **Silhouette Score** (-1 to 1) - Higher is better
2. **Calinski-Harabasz Index** - Higher is better
3. **Davies-Bouldin Index** - Lower is better
4. **Composite Score** - Normalized combination of all metrics

## 📈 Results

The automated evaluation identifies the best clustering configuration based on the composite score. Typical best performers include:

- **Best Algorithm**: Gaussian Mixture Models
- **Best Preprocessing**: PCA or T+N+PCA
- **Optimal Clusters**: 3 (matches ground truth)

Sample output:
=== 🔍 Best Clustering Configuration ===
Algorithm : GMM
Preprocessing : PCA
Clusters : 3
Silhouette : 0.59
Calinski-Harabasz : 560.25
Davies-Bouldin : 0.46
Overall Score : 0.872
