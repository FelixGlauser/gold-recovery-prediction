# gold-recovery-prediction
Machine Learning project for predicting gold recovery rates

## Project Overview

This project focuses on predicting the amount of gold recovered from gold ore during the industrial purification process.

The goal is to develop machine learning models that can predict gold recovery rates at different stages of the production process.

## Business Objective

The mining company needs accurate predictions of gold recovery to optimize production and improve operational efficiency.

## Dataset

The project uses historical process data containing information about:
- Ore characteristics
- Flotation process parameters
- Purification process parameters
- Metal concentrations at different production stages

The datasets were provided as part of the TripleTen Data Science Bootcamp.

## Project Workflow

1. **Data Preparation**
   - Loaded and inspected the datasets
   - Checked data quality and handled missing values
   - Removed anomalous observations

2. **Exploratory Data Analysis**
   - Analyzed metal concentrations throughout the process
   - Examined particle size distributions
   - Compared feed characteristics between training and test datasets

3. **Model Development**
   - Linear Regression
   - Decision Tree
   - Random Forest
   - Cross-validation for model selection

4. **Model Evaluation**
   - Used sMAPE (Symmetric Mean Absolute Percentage Error)
   - Compared model performance against a baseline model

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Key Skills Demonstrated

- Data preprocessing and cleaning
- Exploratory Data Analysis (EDA)
- Feature analysis
- Machine Learning
- Model selection and hyperparameter tuning
- Cross-validation
- Model evaluation

## Conclusion

The project demonstrates an end-to-end machine learning workflow for predicting gold recovery rates using industrial process data.
