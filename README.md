# Energy Data Analysis and Machine Learning

This repository contains three Jupyter Notebooks that perform data analysis and machine learning tasks on energy data. The goal is to explore, visualize, and predict energy usage and greenhouse gas emissions for different buildings.

## Notebooks

1. **Data Exploration and Preprocessing**
   This notebook, `Data_Exploration_and_Preprocessing.ipynb`, focuses on the initial exploration and preprocessing of the energy dataset. It performs the following tasks:
   - Load the raw energy data from a CSV file.
   - Handle missing values and duplicates in the dataset.
   - Explore and visualize the distribution of energy usage and greenhouse gas emissions.
   - Identify and remove irrelevant features from the dataset.
   - Convert data types and handle categorical variables.
   - Save the preprocessed data to a new CSV file, `energy_explored.csv`, for further analysis and machine learning tasks.

2. **Data Visualization and Analysis**
   The notebook `Data_Visualization_and_Analysis.ipynb` builds upon the preprocessed data from the first notebook. It aims to gain insights into energy usage patterns and explore relationships between different variables. The tasks include:
   - Visualizing energy usage and greenhouse gas emissions using various plots (histograms, box plots, scatter plots, etc.).
   - Analyzing the correlation between different features and the target variables.
   - Exploring the relationship between ENERGY STAR Score and energy usage.
   - Investigating the energy usage patterns across different building types and locations.
   - Drawing actionable insights from the visualizations for energy conservation and efficiency.

3. **Machine Learning for Energy Prediction**
   In `Machine_Learning_for_Energy_Prediction.ipynb`, the focus shifts to machine learning tasks for predicting `SiteEnergyUse(kBtu)` and `TotalGHGEmissions`. The notebook includes the following steps:
   - Load the preprocessed energy data from `energy_explored.csv`.
   - Prepare the feature matrix `X` and target vectors `y` and `y0`.
   - Implement various regression models for the predictions, including Linear Regression, Lasso Regression, Ridge Regression, Elastic Net, Random Forest Regressor, XG Boost, Support Vector Machines (SVR), and Decision Tree Regressor.
   - Optimize the models using hyperparameter tuning with GridSearchCV.
   - Evaluate the models' performance using Root Mean Squared Error (RMSE) and cross-validation.
   - Make predictions for `SiteEnergyUse(kBtu)` and `TotalGHGEmissions` and transform the results back to their original unit.
   - Concatenate the predicted values to the original DataFrame.

## Requirements

The following libraries are required to run the notebooks:

- pandas
- numpy
- seaborn
- matplotlib
- scikit-learn

You can install them using the following command:

```
pip install pandas numpy seaborn matplotlib scikit-learn
```

## Usage

To run the notebooks, clone the repository and open Jupyter Notebook on your local machine. Then, navigate to the directory containing the notebooks and open each notebook using Jupyter. Make sure to have the required libraries installed.

## License

This project is licensed under the MIT License. 

## Acknowledgments

Special thanks to the dataset source for providing the energy data used in this analysis.

If you have any questions or feedback, feel free to contact me.
