# 🧠 Image Classification & Regression with Neural Networks in Keras

## 📌 Overview
This project demonstrates how to apply **neural networks using Keras and TensorFlow** to two key machine learning tasks:

1. **Image Classification** – using the Fashion MNIST dataset.
2. **Regression** – predicting California housing prices based on multiple input features.

The models are trained and evaluated using the `Sequential` API in Keras, and their performance is visualized using **TensorBoard**. We also explore how different model architectures impact training outcomes.

---

## 🧭 Project Structure

1. **Image Classification** (Fashion MNIST):
   - Normalize image data to `[0, 1]`
   - Build a 3-layer dense neural network
   - Train and validate with `TensorBoard` logging
   - Save trained model to `fashion_clf.keras`

2. **Regression Task** (California Housing Dataset):
   - Load and split data into training, validation, and test sets
   - Normalize features using a `Normalization` layer
   - Train multiple models with different architectures:
     - 100/50/20
     - 20/50/100
     - 50/50/50
   - Use `EarlyStopping` to prevent overfitting
   - Visualize training in TensorBoard
   - Save models as `reg_housing_1.keras`, `reg_housing_2.keras`, etc.

---

## 🔍 Key Features

- **Fashion MNIST Classification**
  - Multi-class classification (10 categories)
  - Uses ReLU and Softmax activations
  - Visual inspection of predictions and labels

- **California Housing Regression**
  - Mean Squared Error and Root Mean Squared Error as loss/metric
  - Normalization layer to improve convergence
  - TensorBoard logging for every model run
  - EarlyStopping to prevent unnecessary training

- **TensorBoard Support**
  - Real-time logging of loss and metrics
  - Easy comparison of different architectures

- **Model Saving**
  - All models saved in `.keras` format for easy reuse or deployment

---

## 📂 File Summary

- data_classification_and_regression_in_Keras_Tensorflow.ipynb  -->  Jupyter Notebook with code & analysis 
- data_classification_and_regression_in_Keras_Tensorflow.py     -->  Python file with code & analysis
- requirements.txt – Python dependencies
- README.md – project overview and usage guide

---

## 🛠️ Installation & Setup  
To run this project locally, follow these steps:

1. Clone the repository:
    ```bash
   git clone https://github.com/ppaczek04/Machine_Learning_projects.git
   cd Data_Classification_And_Regression_In_Keras_Tensorflow
    ```

2. Install dependencies:
    ```
    pip install -r requirements.txt
    ```

3. Run Jupyter Notebook:
    ```
    jupyter notebook data_classification_and_regression_in_Keras_Tensorflow.ipynb
    ```

## 📊 Results Overview

### 🧥 Fashion MNIST Classification

- Trained with 3 dense layers (300 → 100 → 10 softmax)
- Training accuracy: ~90%
- Validation accuracy: ~88–89%
- ➤ **Conclusion:** The model generalizes well with minimal overfitting.

### 🏠 California Housing Regression

| Architecture     | Epochs (Early Stopping) | Final Validation RMSE |
|------------------|--------------------------|------------------------|
| 100 → 50 → 20     | ~12                      | ~0.555                 |
| 20 → 50 → 100     | ~19                      | ~0.559                 |
| 50 → 50 → 50      | ~15                      | ~0.554                 |

- ➤ **Conclusion:** All architectures performed similarly in terms of RMSE,  
  but the 100/50/20 model converged the fastest and showed more stable learning curves.  
  Balanced structures like 50/50/50 also proved reliable and efficient.


## 💡 Why This Project

This project is designed to provide practical, hands-on experience with deep learning using the **Keras API** within **TensorFlow**.  
It serves as a foundation for understanding how to build and tune neural networks for both **classification** and **regression** tasks.

Key learning goals:
- Understand the structure and training of **Sequential models**
- Apply **data normalization**, **callbacks**, and **TensorBoard**
- Explore how **model architecture** affects training performance
- Learn how to **evaluate and compare** models using validation metrics

By working with real datasets like **Fashion MNIST** and **California Housing**, this project simulates common machine learning workflows used in image analysis and predictive modeling.