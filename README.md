# Scikit Learn Regression: Analysis of Diabetes Data Set

## Purpose of Analysis
This analysis was conducted using Python and Scikit Learn in order to predict the progression of diabetes from a dataset that comes included with Scikit Learn. Three different models were built using the training data in order to find the best model to represent this health related dataset.
## Class Design and Implementation
The Analysis of the Diabetes dataset is done using an Object Oriented Programming (OOP) method through an OOP Class named DiabetesRegressionAnalysis which creates a clean, reusable machine learning pipeline.

**Attributes:** Hyper-parameters (test_size, random_state), Data Arrays such as (X_train, X_test, etc.), a Dictionary of initialized Models through Scikit-Learn and a Dictionary to store the results of the various metrics.
***Methods:*** 
  * prepare_data(): Load Dataset, Split Dataset Into Training/Test Datasets, Apply StandardScaler
  * train_and_evaluate(): Iterate over the List of Models and Train Each Model on the Training Data, Generate Predictions for Each Model, Calculate and Save the Metrics for Each Model (MSE, RMSE, MAE, R2).
  * display_results(): Print Out the Formatted Metrics from train_and_evaluate() and Automatically Identify the Best Model.
   
  ***Address Limitations:*** 
  Implemented StandardScaler so that models that are sensitive to feature scales such as Ridge use the same scale. Used Ridge Regression instead of Standard Linear Regression to reduce risk of overfitting and eliminate any potential multicollinearity with the Medical Features.
