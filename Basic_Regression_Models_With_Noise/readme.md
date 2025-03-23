# **Polynomial Regression with Noise - Project (Updated Version)**

## **Overview**
This project involves generating data using a fourth-degree polynomial function with added noise. The goal is to perform regression analysis to fit a model to the generated data. The data is saved in a CSV file and also visualized on a scatter plot, which allows for the evaluation of how well the model fits the data.

## **Analysis**
- **Input Data**: 300 samples of the independent variable \( x \) in the range from -2.5 to 2.5.
- **Regression Model**: A fourth-degree polynomial function is used to fit the model to the data. Random noise is added to the results to introduce variability and make the regression process more challenging.
- **Data Saving**: The data is saved to the file `dane_do_regresji.csv`, which can be used for further analysis.

## **Project Goals**
- Generate data using the polynomial function with added noise.
- Perform regression analysis to fit the appropriate model.
- Visualize the data and analyze the results of the model fitting.

## **Requirements**
To run the project, the following libraries need to be installed:
- Python>=3.11
- numpy==1.26.0
- pandas==2.2.2
- matplotlib==3.9.0

You can install them using the following command:

```bash
pip install numpy pandas matplotlib
```