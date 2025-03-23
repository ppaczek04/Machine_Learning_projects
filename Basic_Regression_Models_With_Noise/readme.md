# **Polynomial Regression with Noise**

## 📌 **Overview**
This project processes data with added noise and applies various regression models to it. The data is visualized on a scatter plot to evaluate model performance.
This project **helps understand the impact of noise on model accuracy and the importance of selecting appropriate regression techniques.**

## 🔍 **Analysis**
- **Input Data**: 300 samples of the independent variable \( x \) in the range from -2.5 to 2.5.
- **Regression Model**: A fourth-degree polynomial function is used to fit the model to the data. Random noise is added to the results to introduce variability and make the regression process more challenging.
- **Data Saving**: The data is saved to the file `dane_do_regresji.csv`, which can be used for further analysis.

## 🎯 **Project Goals**
- Generate data using the polynomial function with added noise.
- Perform regression analysis to fit the appropriate model.
- Visualize the data and analyze the results of the model fitting.

## 📂 **Project Structure**
- basic_regression_models_with_noise.ipynb  -->  Jupyter Notebook with code & analysis 
- basic_regression_models_with_noise.py     -->  Python file with code & analysis   
- readme.md                            -->  Project description  
- requirements.txt                     -->  Dependencies (if applicable)


## 🛠️ **Installation & Setup**
To run this project locally, follow these steps:

1. Clone the repository:
    ```bash
   git clone https://github.com/ppaczek04/Machine_Learning_projects.git
   cd Basic_Regression_Models_With_Noise
    ```

2. Install dependencies:
    ```
    pip install -r requirements.txt
    ```

3. Run Jupyter Notebook:
    ```
    jupyter notebook basic_regression_models_with_noise.ipynb
    ```

## 📒 **Why This Project?**
This project provides an opportunity to apply regression analysis to data that simulates real-world scenarios, where noise and uncertainty are common. By generating data from a polynomial function with added noise, this project mirrors the challenges encountered when fitting models to imperfect, noisy data. Understanding how well a model can fit such data is crucial in various fields, including machine learning, data science, and engineering. This project helps in building a deeper understanding of the impact of noise on model accuracy and the importance of selecting and evaluating appropriate regression techniques.