# Decision Tree Classification and Regression

## 📌 Overview
This project explores the use of **Decision Trees** for both classification and regression tasks. Decision Trees are easy to use and adapt well to data, making them an attractive choice for many machine learning problems. However, they are **prone to overfitting** — especially when the model becomes too complex. To address this, we regularize the model by tuning hyperparameters such as `max_depth` to ensure that the tree generalizes well on new, unseen data. 


## 🔍 Key Features
- **Data Import**: The project uses the **Breast Cancer dataset** from sklearn for classification.
- **Classification**:
  - **Decision Tree** model is trained to classify tumor types into Malignant or Benign.
  - **F1 Score** and **accuracy** are used to evaluate performance.
  - Regularization using `max_depth` to prevent overfitting.
  - Visualization of the trained decision tree and F1 scores over different tree depths.
- **Regression**:
  - A **Decision Tree Regressor** is used to fit a model to synthetic data.
  - The performance is evaluated using **Mean Squared Error (MSE)**.
  - The best model is selected based on minimizing the MSE and test data accuracy.
  
## 📂 Project Structure
- decision_tree_classification_and_regression.ipynb  -->  Jupyter Notebook with code & analysis 
- decision_tree_classification_and_regression.py     -->  Python file with code & analysis   
- readme.md                            -->  Project description  
- requirements.txt                     -->  Dependencies (if applicable)
- other files contain pngs of visualisations and data generated in the script
## 🛠️ Installation & Setup
To run this project locally, follow these steps:

1. Clone the repository:
    ```bash
   git clone https://github.com/yourusername/Decision_Tree_Project.git
   cd Decision_Tree_Classification_and_Regression
    ```

2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the Python script:
    ```bash
    python decision_tree_classification_and_regression.py
    ```

## 📊 Results & Insights
- **Classification**:
  - As `max_depth` increased, the training F1 score improved and eventually reached perfect classification. However, the test F1 score initially improved but then declined, indicating **overfitting**.
  - The best classification model parameters were stored in `f1acc_tree.pkl`.
  
- **Regression**:
  - The **Decision Tree Regressor** performed well in modeling the synthetic data, with the MSE being minimized for a specific `max_depth`.
  - The best regression model parameters were saved in `mse_tree.pkl`.

## 📒 Why This Project?
This project demonstrates how **Decision Trees** can be used for both classification and regression tasks, highlighting the importance of model regularization. It also emphasizes evaluating model performance using metrics like F1 score and MSE, and the need to tune hyperparameters such as `max_depth` to prevent overfitting and improve generalization.