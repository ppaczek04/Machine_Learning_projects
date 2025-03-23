# Handwritten Digit Recognition with Stochastic Gradient Descent (SGD)

## 📌 Overview
This project is a machine learning experiment focused on handwritten digit recognition using the **Stochastic Gradient Descent (SGD) classifier**. The dataset is split into training and testing sets, highlighting the importance of shuffling data before training. Additionally, the model is evaluated using **cross-validation and a confusion matrix**.

## 🔍 Key Features
- **Data Preparation**: Ensuring balanced representation of digits.
- **Train-Test Split**:
  - Manual split (to demonstrate data imbalance issues without shuffling).
  - Proper split using `train_test_split` with shuffling.
- **Model Training**:
  - Training an SGD classifier to recognize digit **'0'**.
  - Extending the model to recognize **all digits (0-9)**.
  - Performing **3-fold cross-validation**.
  - Evaluating performance using a **confusion matrix**.

## 📂 Project Structure
- handwritten_digit_recognition.ipynb  -->  Jupyter Notebook with code & analysis 
- handwritten_digit_recognition.py     -->  Python file with code & analysis   
- readme.md                            -->  Project description  
- requirements.txt                     -->  Dependencies (if applicable)

## 🛠️ Installation & Setup
To run this project locally, follow these steps:

1. Clone the repository:
    ```bash
   git clone https://github.com/ppaczek04/Machine_Learning_projects.git
   cd handwritten_digit_recognition
    ```

2. Install dependencies:
    ```
    pip install -r requirements.txt
    ```

3. Run Jupyter Notebook:
    ```
    jupyter notebook handwritten_digit_recognition.ipynb
    ```



## 📊 Results & Insights
- Without shuffling, some digits (like 8 and 9) were missing from the training set, making it impossible for the model to learn them.
- After applying **train-test split with shuffle**, the dataset was balanced, and the model could learn all digits.
- **Confusion matrix** helped visualize classification accuracy and misclassified digits.
- **SGD classifier** is a fast, scalable method suitable for large-scale machine learning problems.

## 📌 Why This Project?
This project demonstrates **essential data preprocessing techniques** and highlights **the importance of proper dataset splitting in machine learning**. It showcases fundamental ML concepts that are crucial for **data analysts and ML practitioners**.