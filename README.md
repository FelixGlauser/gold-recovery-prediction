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

## Model Selection and Cross-Validation Results

Five-fold cross-validation was used to compare the performance of different regression models.

| Model | Rougher sMAPE | Final sMAPE | Weighted sMAPE |
|---|---:|---:|---:|
| Random Forest (100 trees, depth 20) | 2.60 | 5.84 | **5.03** |
| Random Forest (100 trees, depth 10) | 3.05 | 6.55 | 5.68 |
| Decision Tree (depth 10) | 3.68 | 7.52 | 6.56 |
| Decision Tree (depth 5) | 4.51 | 8.03 | 7.15 |
| Linear Regression | 4.69 | 8.20 | 7.33 |

The Random Forest with 100 trees and a maximum depth of 20 achieved the best cross-validation result, with a weighted sMAPE of 5.03.

The weighted sMAPE is calculated using 25% for rougher recovery and 75% for final recovery. Lower values indicate better model performance.

## Final Test Results

The selected Random Forest model was evaluated on the independent test dataset and compared with a baseline model using median predictions.

| Model | Rougher sMAPE | Final sMAPE | Weighted sMAPE |
|---|---:|---:|---:|
| Random Forest | 4.33 | 8.14 | **7.19** |
| Median Baseline | 4.82 | 8.21 | 7.36 |

The Random Forest achieved a weighted sMAPE of 7.19, slightly outperforming the baseline model (7.36).

This demonstrates that the selected model provides a measurable, although moderate, improvement over a simple baseline approach.
