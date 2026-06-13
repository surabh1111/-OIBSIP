# Car Price Prediction

This project contains a Jupyter Notebook for predicting used car selling prices with machine learning. It was created for **Task 3: Car Price Prediction with Machine Learning** as part of the AICTE Oasis Infobyte Internship.

## Project Overview

The notebook builds an end-to-end regression workflow for car price prediction. It loads a car dataset when available, cleans and prepares the data, explores important patterns visually, trains multiple machine learning models, compares their performance, and demonstrates sample predictions.

If no CSV dataset is found, the notebook automatically creates a realistic sample dataset so the full workflow can still run.

## Files

| File | Description |
| --- | --- |
| `CAR_PRICE_PREDICTION_.ipynb` | Main notebook containing data preparation, visualization, model training, evaluation, and prediction demo |
| `README.md` | Project documentation |

The notebook may generate these output images after running:

| Output | Description |
| --- | --- |
| `car_eda.png` | Exploratory data analysis plots |
| `car_correlation.png` | Correlation heatmap for numeric features |
| `car_model_results.png` | Actual vs predicted prices and model comparison |
| `car_feature_importance.png` | Top feature importance chart |

## Dataset

The notebook first looks for one of these CSV files in the same folder:

- `car data.csv`
- `CAR DETAILS FROM CAR DEKHO.csv`

If neither file exists, it generates a sample dataset with features such as:

- Car brand
- Manufacturing year
- Kilometers driven
- Fuel type
- Seller type
- Transmission
- Owner type
- Seats
- Mileage
- Engine
- Maximum power
- Selling price

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

3. Open `CAR_PRICE_PREDICTION_.ipynb`.
4. Run all cells from top to bottom.
5. Check the generated plots and printed model evaluation metrics.

## Workflow

The notebook follows these main steps:

1. Import required libraries.
2. Load the car dataset or generate sample data.
3. Clean the data and engineer useful features such as `car_age`.
4. Handle missing values.
5. Create EDA visualizations.
6. Preprocess numerical and categorical features.
7. Split the data into training and testing sets.
8. Train multiple regression models.
9. Compare model performance using MAE, RMSE, and R2 score.
10. Select the best model and show sample predictions.

## Models Used

The notebook trains and compares:

- Linear Regression
- Ridge Regression
- Lasso Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor

## Current Sample Results

Using the generated sample dataset, the best performing model was:

| Model | R2 Score | MAE | RMSE |
| --- | ---: | ---: | ---: |
| Gradient Boosting Regressor | 0.9264 | 23,458 | 34,774 |

These results may change if a real CSV dataset is added or if the notebook is modified.

## Notes

- Place a real car dataset CSV in the same directory to train on real data.
- The notebook expects the target price column to be named `selling_price` or `price`.
- Categorical features are encoded with one-hot encoding.
- Numerical features are scaled before training.
