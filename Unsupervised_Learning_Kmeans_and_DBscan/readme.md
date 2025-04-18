# Unsupervised Learning K-Means and DBscan (NOT FINISHED)

## 📌 Overview
This project explores unsupervised learning by applying **K-Means** and **DBSCAN** clustering algorithms to the **MNIST** dataset of handwritten digits.  
The goal is to evaluate how well these algorithms can group digit images without using any labels and to experiment with clustering metrics such as **silhouette score** and **confusion matrix**.

## 🔍 Key Features
- **Dataset**: The MNIST dataset with 70,000 handwritten digits (we use a subset for performance).
- **Dimensionality Reduction**: Uses **PCA** to reduce 784-dimensional data to 2D for visualization.
- **K-Means Clustering**:
  - Tests cluster counts from 8 to 12.
  - Evaluates using **silhouette score** to determine the optimal number of clusters.
  - Compares cluster assignments to actual digits using a **confusion matrix**.
- **DBSCAN Clustering**:
  - Estimates `eps` parameter using Euclidean distances between samples.
  - Measures how the number of clusters changes for different `eps` values.
- **Pickle Exports**:
  - Saves silhouette scores, cluster mappings, distance values, and DBSCAN cluster counts to `.pkl` files for reuse.

## 📂 Project Structure  
- ensamble_learning_and_random_forests.ipynb  -->  Jupyter Notebook with code & analysis 
- ensamble_learning_and_random_forests.py     -->  Python file with code & analysis   
- readme.md                            -->  Project description  
- requirements.txt                     -->  Dependencies (if applicable)

## 🛠️ Installation & Setup  
To run this project locally:

1. Clone the repository:
   ```bash
   git clone https://github.com/ppaczek04/Machine_Learning_projects.git
   cd Unsupervised_Learning_Kmeans_and_DBscan
   ```

2. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebook:
   ```bash
   jupyter notebook unsupervised_learning_kmeans_and_dbscan.ipynb
   ```

## 📊 Results & Insights
- **K-Means**:
  - Clustering with `k=10` produced good alignment with the 10 actual digits.
  - Silhouette scores confirmed 8–10 as reasonable cluster counts.
  - Confusion matrix showed which clusters correspond to which digits.
- **DBSCAN**:
  - Required tuning the `eps` parameter based on distance heuristics.
  - Identified clusters of varying density and was able to mark outliers.
  - Provided a more flexible but sensitive alternative to K-Means.

## 📒 Why This Project?
This project provides a hands-on demonstration of unsupervised learning techniques on a real-world dataset.  
It shows how to apply, tune, and evaluate clustering algorithms, and helps develop a deeper understanding of model behavior without using labeled data.  

A great resource for:
- Data science students
- ML practitioners exploring clustering
- Anyone curious about machine learning beyond classification