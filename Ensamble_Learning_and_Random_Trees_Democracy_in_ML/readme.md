# Ensemble Learning and Random Forests

## 📌 Overview
This project is a machine learning experiment focused on **ensemble learning** methods, particularly **Bagging**, **Random Forests**, and **Boosting**. The primary goal is to classify samples into different categories using various ensemble techniques, demonstrating how combining multiple weak models can lead to stronger and more reliable predictions compared to individual models.

## 🔍 Key Features
- **Data Preparation**: Focused on two selected features for classification.
- **Base Classifiers**: Implemented **Decision Tree**, **Logistic Regression**, and **k-Nearest Neighbors (k-NN)**.
- **Voting Ensembles**:
  - **Hard Voting**: Class label is chosen based on the majority vote.
  - **Soft Voting**: Class label is determined by averaging predicted class probabilities.
- **Bagging and Random Forest**:
  - **Bagging (Bootstrap Aggregating)**: Trains multiple trees using random subsets of the data with replacement.
  - **Random Forest**: A type of Bagging with additional feature randomness, where each tree uses a random subset of features for splits.
- **Boosting**:
  - **AdaBoost**: Focuses on misclassified examples, adjusting their weights to prioritize harder-to-classify samples.
  - **Gradient Boosting**: Trains sequentially, each new model attempting to correct the errors of the previous ones.
- **Feature Sampling**: Demonstrates the impact of selecting random subsets of features to train each individual tree, improving robustness and model diversity.

## 📂 Project Structure  
- ensamble_learning_and_random_forests.ipynb  -->  Jupyter Notebook with code & analysis 
- ensamble_learning_and_random_forests.py     -->  Python file with code & analysis   
- readme.md                            -->  Project description  
- requirements.txt                     -->  Dependencies (if applicable)

## 🛠️ Installation & Setup  
To run this project locally, follow these steps:

1. Clone the repository:
    ```bash
   git clone https://github.com/ppaczek04/Machine_Learning_projects.git
   cd Ensamble_Learning_and_Random_Trees_Democracy_in_ML
    ```

2. Install dependencies:
    ```
    pip install -r requirements.txt
    ```

3. Run Jupyter Notebook:
    ```
    jupyter notebook ensemble_learning_and_random_forests.ipynb
    ```

4. Jupyter Notebooks or additional analysis can be run in an interactive environment if preferred.

## 📊 Results & Insights
- **Base classifiers**: Logistic Regression, Decision Trees, and k-NN showed moderate performance on their own.
- **Voting classifiers**: 
  - **Hard Voting** improved accuracy by aggregating the predictions of individual models.
  - **Soft Voting** generally provided the best results by considering model confidence.
- **Ensemble Methods**: 
  - **Random Forest** performed better than Bagging by using random feature selection.
  - **Boosting methods (AdaBoost, Gradient Boosting)** provided high accuracy by focusing on misclassified samples, but required careful hyperparameter tuning.
- **Feature Sampling**: Randomly selecting a subset of features for each tree reduced variance and made the model more robust.

## 📒 Why This Project?
This project demonstrates how **ensemble learning** techniques, such as Bagging, Random Forests, and Boosting, can be used to improve prediction accuracy. It showcases the importance of **model diversity** and the **impact of feature sampling** in creating more robust and generalizable machine learning models. This project is useful for **data scientists**, **machine learning practitioners**, and anyone looking to improve their skills in building powerful machine learning models.
