# Sales Prediction Using Python

This project predicts product sales from advertising spend using Python machine learning techniques. It was created for **Task 5: Sales Prediction Using Python** as part of the **AICTE Oasis Infobyte Internship**.

The main work is contained in the Jupyter notebook:

- `SALES_PREDICTION_USING_PYTHON.ipynb`

## Project Overview

The notebook analyzes advertising data and trains multiple regression models to estimate sales based on marketing spend. If a CSV dataset is not available, the notebook automatically creates a realistic sample advertising dataset so the project can still run end to end.

## Features

- Loads `advertising.csv` or `sales_data_sample.csv` when available
- Generates sample advertising data if no dataset file is found
- Cleans and preprocesses the dataset
- Performs exploratory data analysis with visualizations
- Engineers useful features such as total spend and interaction terms
- Trains and compares multiple regression models
- Evaluates models using MAE, RMSE, R-squared, and cross-validation
- Identifies the best-performing model
- Visualizes prediction results and feature importance
- Provides simple ad budget optimization insights

## Models Used

The notebook compares the following models:

- Linear Regression
- Ridge Regression
- Lasso Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor
- Support Vector Regressor

## Requirements

Install the required Python libraries before running the notebook:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

## How to Run

1. Open the project folder.
2. Start Jupyter Notebook:

```bash
jupyter notebook
```

3. Open `SALES_PREDICTION_USING_PYTHON.ipynb`.
4. Run all cells from top to bottom.

Optional: place an `advertising.csv` file or `sales_data_sample.csv` file in the same folder as the notebook to use your own dataset.

## Expected Outputs

When the notebook runs successfully, it prints model evaluation results and saves several visualization files:

- `sales_eda.png`
- `sales_correlation.png`
- `sales_model_results.png`
- `sales_feature_importance.png`
- `sales_budget_optimization.png`

## Dataset

The notebook looks for these files in order:

1. `advertising.csv`
2. `sales_data_sample.csv`

If neither file exists, it creates a synthetic dataset with advertising channels such as TV, Radio, Newspaper, customer segment, platform, and sales.

## Evaluation Metrics

Model performance is measured using:

- **MAE**: Mean Absolute Error
- **RMSE**: Root Mean Squared Error
- **R-squared**: Proportion of sales variance explained by the model
- **Cross-validation score**: Average R-squared across validation folds

## Conclusion

This project demonstrates a complete machine learning workflow for sales prediction, including data loading, cleaning, visualization, feature engineering, model training, evaluation, and business-oriented budget optimization.
