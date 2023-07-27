# Energy Data Analysis and Machine Learning

This repository contains Jupyter Notebooks that perform data analysis, preprocessing, and machine learning tasks on energy data. The goal is to explore, visualize, and predict energy usage and greenhouse gas emissions for different buildings.

## Notebooks

1. **Data Exploration and Preprocessing**
   This notebook, `Data_Exploration_and_Preprocessing.ipynb`, focuses on the initial exploration and preprocessing of the energy dataset. It performs the following tasks:
   - Load the raw energy data from a CSV file.
   - Handle missing values and duplicates in the dataset.
   - Explore and visualize the distribution of energy usage and greenhouse gas emissions.
   - Identify and remove irrelevant features from the dataset.
   - Convert data types and handle categorical variables.
   - Save the preprocessed data to a new CSV file, `energy_explored.csv`, for further analysis and machine learning tasks.

2. **Machine Learning for Energy Prediction (Using ENERGYSTARScore)**
   In `Machine_Learning_with_EnergyScore.ipynb`, we use the `ENERGYSTARScore` as one of the features for predicting `SiteEnergyUse(kBtu)` and `TotalGHGEmissions`. The notebook includes the following steps:
   - Load the preprocessed energy data from `energy_explored.csv`.
   - Prepare the feature matrix `X` (including `ENERGYSTARScore`) and target vectors `y` and `y0`.
   - Implement various regression models for the predictions, including Linear Regression, Lasso Regression, Ridge Regression, Elastic Net, Random Forest Regressor, XG Boost, Support Vector Machines (SVR), and Decision Tree Regressor.
   - Optimize the models using hyperparameter tuning with GridSearchCV.
   - Evaluate the models' performance using Root Mean Squared Error (RMSE) and cross-validation.
   - Make predictions for `SiteEnergyUse(kBtu)` and `TotalGHGEmissions` and transform the results back to their original unit.
   - Concatenate the predicted values to the original DataFrame.

3. **Machine Learning for Energy Prediction (Without ENERGYSTARScore)**
   In `Machine_Learning_without_EnergyScore.ipynb`, we exclude the `ENERGYSTARScore` feature from the predictions of `SiteEnergyUse(kBtu)` and `TotalGHGEmissions`. The notebook follows similar steps as the previous one, but without `ENERGYSTARScore` in the feature matrix `X`.

## Requirements

The following libraries are required to run the notebooks:

- pandas
- numpy
- seaborn
- matplotlib
- scikit-learn

You can install them using the following command:

pip install pandas numpy seaborn matplotlib scikit-learn

## Usage

To run the notebooks, clone the repository and open Jupyter Notebook on your local machine. Then, navigate to the directory containing the notebooks and open each notebook using Jupyter. Make sure to have the required libraries installed.

## License

This project is licensed under the MIT License. Feel free to use, modify, and distribute the code for your purposes.

## Acknowledgments

If you have any questions or feedback, feel free to contact me. 
