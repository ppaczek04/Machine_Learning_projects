# Neural Network Hyperparameters Tuning

## 📌 Overview  
This project demonstrates the process of **hyperparameter tuning** for a neural network model applied to the **California Housing** dataset. It explores how different hyperparameters affect model training and prediction accuracy. Two popular approaches are used: **RandomizedSearchCV** from scikit-learn with a Keras wrapper, and **Keras Tuner** for automated hyperparameter optimization.

## 🧭 Introduction  
The project is structured into the following parts:

1. **Data Preparation** – loading, splitting, and normalizing the California Housing dataset.  
2. **Hyperparameter Search using scikit-learn** – manual hyperparameter search with a `KerasRegressor` wrapped model, utilizing `RandomizedSearchCV` to tune the number of hidden layers, neurons per layer, learning rate, and optimizer.  
3. **Hyperparameter Search using Keras Tuner** – automated search with Keras Tuner’s `RandomSearch` tuner, using similar hyperparameter ranges.  
4. **Model Evaluation and Saving** – selecting the best hyperparameters, saving models and search results for later analysis.

## 🔍 Key Features  
- **Dataset**: California Housing regression dataset for predicting housing prices.  
- **Model Architecture**:
  - Variable number of hidden layers (0 to 3).  
  - Variable neurons per hidden layer (1 to 100).  
  - Choice of optimizer (`sgd`, `adam`, `nesterov`).  
  - Learning rate tuning over a continuous range.  
- **scikit-learn Integration**:
  - Wrapping Keras models with `scikeras.wrappers.KerasRegressor`.  
  - Hyperparameter tuning with `RandomizedSearchCV`.  
- **Keras Tuner**:
  - Defining model-building functions with hyperparameters.  
  - Running automated search with `RandomSearch`.  
- **Early Stopping**:
  - Use of callbacks to stop training early when validation performance plateaus.  
- **Visualization**:
  - Training loss curves for different hyperparameter settings.  
- **Saving Artifacts**:
  - Best hyperparameters and models saved as `.pkl` and `.keras` files.

## 📂 Project Structure  
- neural_network_hyperparameters_tuning.ipynb  -->  Jupyter Notebook with code & analysis 
- neural_network_hyperparameters_tuning.py     -->  Python file with code & analysis   
- readme.md                            -->  Project description  
- requirements.txt                     -->  Dependencies (if applicable)

## 🛠️ Installation & Setup  
To run this project locally, follow these steps:

1. Clone the repository:
    ```bash
   git clone https://github.com/ppaczek04/Machine_Learning_projects.git
   cd Neural_Network_Hyperparameters_Tuning
    ```

2. Install dependencies:
    ```
    pip install -r requirements.txt
    ```

3. Run Jupyter Notebook:
    ```
    jupyter notebook neural_network_hyperparameters_tuning.ipynb
    ```


## 📊 Results  

### RandomizedSearchCV Hyperparameter Tuning:  
- Explored learning rates from 3e-4 to 3e-2, number of hidden layers from 0 to 3, neurons per layer from 1 to 100, and optimizers including SGD variants and Adam.  
- Achieved significant improvements in validation loss compared to default parameters.  
- Example of best found parameters:
  ```json
  {
    "model__optimizer": "adam",
    "model__n_neurons": 42,
    "model__n_hidden": 3,
    "model__learning_rate": 0.004
  }

## 💡 Why This Project  
Hyperparameter tuning is a crucial step in building effective machine learning models, especially neural networks. Choosing the right combination of hyperparameters—such as learning rate, number of hidden layers, number of neurons, and optimizer—can greatly impact model performance, training stability, and generalization to new data.

This project demonstrates practical techniques for hyperparameter optimization using both traditional scikit-learn tools (`RandomizedSearchCV` with Keras wrappers) and modern Keras Tuner approaches. By applying these methods to the California Housing dataset—a realistic regression task—it highlights how systematic tuning can lead to significant improvements in prediction accuracy and model robustness.

Ultimately, this project helps develop a deeper understanding of how hyperparameters influence neural network training and provides hands-on experience with popular tools to automate and streamline the tuning process.
