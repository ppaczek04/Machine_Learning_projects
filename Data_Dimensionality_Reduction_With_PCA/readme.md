# Data Dimensionality Reduction with PCA

## 📌 Overview
This project demonstrates how to reduce the dimensionality of datasets using **Principal Component Analysis (PCA)**.  
We apply PCA to the **breast cancer** and **iris** datasets from scikit-learn, aiming to preserve at least **90% of the original data variance** while minimizing the number of features.

## 🔍 Key Features
- **Datasets**:
  - `breast_cancer`: 30 numerical features describing tumor properties.
  - `iris`: 4 numerical features describing flower dimensions.
- **StandardScaler**:
  - Applied before PCA to ensure all features contribute equally, regardless of their original scale.
- **PCA Analysis**:
  - Reduces the dimensionality of the data while preserving ≥90% variance.
  - Identifies how many components are needed to reach that threshold.
  - Extracts feature importance based on contribution to principal components.
- **Pickle Output**:
  - Saves explained variance ratios and sorted indices of original features based on importance.

## 📂 Project Structure
- data_dimensionality_reduction_with_PCA.ipynb --> Jupyter Notebook with full implementation  
- data_dimensionality_reduction_with_PCApy --> Script version for automatic grading  
- pca_bc.pkl, pca_ir.pkl --> Explained variance ratios (after scaling)  
- idx_bc.pkl, idx_ir.pkl --> Indices of original features ranked by importance
- readme.md                            -->  Project description  
- requirements.txt                     -->  Dependencies (if applicable)

## 🛠️ Installation & Setup
To run this project locally:

To run this project locally:

1. Clone the repository:
   ```bash
   git clone https://github.com/ppaczek04/Machine_Learning_projects.git
   cd Data_Dimensionality_Reduction_With_PCA
   ```

2. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebook:
   ```bash
   jupyter notebook data_dimensionality_reduction_with_PCA.ipynb
   ```