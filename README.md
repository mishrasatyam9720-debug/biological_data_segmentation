# 🧬 Breast Cancer Gene Expression Clustering

## 📌 Project Overview

This project performs **unsupervised clustering on breast cancer gene expression data** using **Hierarchical Agglomerative Clustering**.

The dataset contains a large number of gene-expression features, making it a high-dimensional dataset. To make clustering more efficient and meaningful, **StandardScaler** and **Principal Component Analysis (PCA)** were used before applying hierarchical clustering.

The project also uses a **Dendrogram** for visualizing the hierarchical structure and **Silhouette Score** for evaluating different numbers of clusters.

---

## 📊 Dataset

The dataset used in this project is the **Breast Cancer Gene Expression Dataset (GSE45827)**.

After data cleaning:

- **Samples:** 117
- **Original gene-expression features:** 54,675
- **Data type:** Gene expression data
- **Learning type:** Unsupervised Learning

The `samples` column represents sample IDs and `type` contains the known subtype information. The `type` column was **not used during clustering**.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- SciPy
- Jupyter / Google Colab

---

## 🔄 Project Workflow

```text
Raw Dataset
     ↓
Data Cleaning
     ↓
Feature Selection
     ↓
StandardScaler
     ↓
PCA (95% Variance)
     ↓
Hierarchical Agglomerative Clustering
     ↓
Ward Linkage
     ↓
Dendrogram
     ↓
Silhouette Score
     ↓
Selection of Number of Clusters
