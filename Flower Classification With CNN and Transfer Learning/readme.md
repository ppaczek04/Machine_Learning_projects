# 🌼 Flower Classification with CNN and Transfer Learning

## 📌 Overview  
This project demonstrates the use of **Convolutional Neural Networks (CNNs)** for image classification, applied to the `tf_flowers` dataset.  
Two approaches are compared: a custom CNN trained from scratch and a model based on **transfer learning using the Xception architecture**.  
The project is implemented using **TensorFlow/Keras** and includes data preprocessing, training, evaluation, and result visualization.

## 🧭 Introduction  
The project is divided into two main sections:

1. **Custom CNN Model** – A relatively simple convolutional network built and trained from scratch to classify flower images into five categories.
2. **Transfer Learning with Xception** – An advanced approach using the Xception model pretrained on ImageNet. A custom classification head is added and trained in two stages: freezing the base model, then fine-tuning the full network.

Both models are trained and evaluated on the `tf_flowers` dataset using a standard split: 75% training, 15% validation, and 10% testing.

## 🔍 Key Features  
- **CNN from Scratch**:
  - Manual architecture with 3 convolutional blocks followed by dense layers.
  - Used as a baseline to evaluate performance without pretrained features.
- **Transfer Learning**:
  - Leveraging pretrained Xception weights as a feature extractor.
  - Two-phase training: frozen base + fine-tuning.
- **Data Pipeline**:
  - Efficient preprocessing using `tf.data.Dataset`: resizing, batching, shuffling, and normalization.
- **Evaluation**:
  - Accuracy measured on training, validation, and test sets.
  - Result comparison between baseline and transfer learning model.
- **Model Saving**:
  - Trained models saved as `.keras` files.
  - Accuracy scores stored using `pickle` for later use.

## 📂 **Project Structure**
- flower_classification_with_CNN_and_transfer_learning.ipynb  -->  Jupyter Notebook with code & analysis 
- flower_classification_with_CNN_and_transfer_learning.py   -->  Python file with code & analysis   
- readme.md                            -->  Project description  
- requirements.txt                     -->  Dependencies (if applicable)


## 🛠️ **Installation & Setup**
To run this project locally, follow these steps:

1. Clone the repository:
    ```bash
   git clone https://github.com/ppaczek04/Machine_Learning_projects.git
   cd Flower Classification With CNN and Transfer Learning
    ```

2. Install dependencies:
    ```
    pip install -r requirements.txt
    ```

3. Run Jupyter Notebook:
    ```
    jupyter notebook flower_classification_with_CNN_and_transfer_learning.ipynb
    ```

## 📒 **Why This Project?**
This project provides an opportunity to apply regression analysis to data that simulates real-world scenarios, where noise and uncertainty are common. By generating data from a polynomial function with added noise, this project mirrors the challenges encountered when fitting models to imperfect, noisy data. Understanding how well a model can fit such data is crucial in various fields, including machine learning, data science, and engineering. This project helps in building a deeper understanding of the impact of noise on model accuracy and the importance of selecting and evaluating appropriate regression techniques.