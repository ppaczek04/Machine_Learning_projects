# Breast Cancer Classification with SVM models

## 📌 Overview  
This project demonstrates the application of **Support Vector Machine (SVM)** models for both classification and regression using real-world and synthetic datasets. It uses the `scikit-learn` library to train, evaluate, and visualize model performance under various preprocessing conditions, including feature scaling and hyperparameter tuning.

## 🧭 Introduction  
The project is divided into three main parts:

1. **Breast Cancer Classification** – the core component of this project, where a linear SVM model is trained to distinguish between malignant and benign tumors.
2. **Iris Species Classification** – BONUS: binary classification task that determines whether a flower belongs to the *Iris Virginica* species.
3. **SVM-based Regression** – BONUS: section where both `LinearSVR` and `SVR` are used to perform polynomial regression on synthetically generated data.

Each section highlights different aspects of SVM models — from linear classification and feature scaling to model complexity and hyperparameter tuning.

## 🔍 Key Features  
- **Classification with LinearSVC**:
  - Predicting **malignant vs. benign tumors** using selected features from the Breast Cancer dataset.
  - Recognizing **Iris Virginica** species vs. other species using petal dimensions.
- **Feature Scaling Impact**:
  - Comparison of model accuracy **with and without** feature normalization.
- **Regression with SVR**:
  - Fitting a 4th-degree polynomial using `LinearSVR` with polynomial features.
  - Comparing performance with standard `SVR` using a polynomial kernel.
- **Visualization**:
  - Plotting **decision boundaries** for classification tasks.
  - Plotting **regression curves** for SVR models.
- **Hyperparameter Tuning**:
  - Using `GridSearchCV` to improve regression accuracy through optimal `C` and `coef0` selection.

## 📂 Project Structure  
- breast_cancer_classification_with_SVM_models.ipynb  -->  Jupyter Notebook with code & analysis 
- breast_cancer_classification_with_SVM_models.py     -->  Python file with code & analysis   
- readme.md                            -->  Project description  
- requirements.txt                     -->  Dependencies (if applicable)

## 🛠️ Installation & Setup  
To run this project locally, follow these steps:

1. Clone the repository:
    ```bash
   git clone https://github.com/ppaczek04/Machine_Learning_projects.git
   cd Breast_Cancer_Classification_with_SVM_models
    ```

2. Install dependencies:
    ```
    pip install -r requirements.txt
    ```

3. Run Jupyter Notebook:
    ```
    jupyter notebook breast_cancer_classification_with_SVM_models.ipynb
    ```

## 📊 Results  

### ✅ Breast Cancer Classification:
This measurements are just illustrative results and might differ slightly:
- Without feature scaling:  
  - Training Accuracy: ~62%  
  - Testing Accuracy: ~68%
- With feature scaling:  
  - Training Accuracy: ~90%  
  - Testing Accuracy: ~90%
- ➤ **Conclusion**: Feature scaling significantly improves model performance for SVM classifiers.

### 🌸 Iris Virginica Classification (Bonus):
- Without feature scaling:  
  - Training Accuracy: ~96%  
  - Testing Accuracy: ~100%
- With feature scaling:  
  - Training Accuracy: ~95%  
  - Testing Accuracy: ~95% 
- ➤ Note: Scaling slightly reduced accuracy, likely due to features already being on similar scales.

### 📈 Polynomial Regression with SVR (Bonus):
- `LinearSVR` with polynomial features achieved lower Mean Squared Error (MSE) than standard `SVR`.
- After hyperparameter tuning using `GridSearchCV`, `SVR` model performance improved significantly.

## 💡 Why This Project  
Breast cancer remains one of the most common and life-threatening forms of cancer among women worldwide. Early and accurate detection significantly improves the chances of effective treatment and survival. This project demonstrates how **machine learning** — specifically **Support Vector Machines (SVM)** — can be applied to real-world medical data to aid in **automatic classification of tumors as malignant or benign**.  
By leveraging SVM models, we can support doctors and radiologists in making more informed decisions and reduce diagnostic errors.  
