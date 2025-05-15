# Machine_Learning_projects
This repository contains all the ML projects ive been currently working on, each directory contains a single project (in which you can find its own readme file).  

## 1. Handwritten Digit Recognition

This project is a machine learning experiment focused on handwritten digit recognition using the **Stochastic Gradient Descent (SGD) classifier**. The dataset is split into training and testing sets, highlighting the importance of shuffling data before training. Additionally, the model is evaluated using **cross-validation and a confusion matrix**.

## 2. Basic Regression Models With Noise

This project processes data with added noise and applies various regression models to it. The data is visualized on a scatter plot to evaluate model performance.
This project **helps understand the impact of noise on model accuracy and the importance of selecting appropriate regression techniques.**

## 3. Breast Cancer Classification with SVM models

This project demonstrates the application of **Support Vector Machine (SVM)** models for both classification and regression using real-world and synthetic datasets. It uses the `scikit-learn` library to train, evaluate, and visualize model performance under various preprocessing conditions, including feature scaling and hyperparameter tuning.

## 4. Decision Tree Classification and Regression
This project explores the use of **Decision Trees** for both classification and regression tasks. Decision Trees are easy to use and adapt well to data, making them an attractive choice for many machine learning problems. However, they are **prone to overfitting** — especially when the model becomes too complex. To address this, we regularize the model by tuning hyperparameters such as `max_depth` to ensure that the tree generalizes well on new, unseen data. 

## 5. Ensamble Learning and Random Forests - Democracy in ML
This project is a machine learning experiment focused on **ensemble learning** methods, particularly **Bagging**, **Random Forests**, and **Boosting**. The primary goal is to classify samples into different categories using various ensemble techniques, demonstrating how combining multiple weak models can lead to stronger and more reliable predictions compared to individual models.

## 6. Unsupervised Learning K-Means and DBscan (NOT FINISHED)
This project explores unsupervised learning by applying **K-Means** and **DBSCAN** clustering algorithms to the **MNIST** dataset of handwritten digits.  The goal is to evaluate how well these algorithms can group digit images without using any labels and to experiment with clustering metrics such as **silhouette score** and **confusion matrix**.

## 7. Data Dimensionality Reduction with PCA
This project demonstrates how to reduce the dimensionality of datasets using **Principal Component Analysis (PCA)**.  
We apply PCA to the **breast cancer** and **iris** datasets from scikit-learn, aiming to preserve at least **90% of the original data variance** while minimizing the number of features.

## 8. Image Classification & Regression with Neural Networks in Keras
This project demonstrates how to apply **neural networks using Keras and TensorFlow** to two key machine learning tasks:

1. **Image Classification** – using the Fashion MNIST dataset.
2. **Regression** – predicting California housing prices based on multiple input features.

The models are trained and evaluated using the `Sequential` API in Keras, and their performance is visualized using **TensorBoard**. We also explore how different model architectures impact training outcomes.