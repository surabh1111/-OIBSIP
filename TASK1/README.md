# Iris Flower Classification

This project contains a Jupyter Notebook for classifying Iris flowers into three species:

- Setosa
- Versicolor
- Virginica

The notebook uses the built-in Iris dataset from `scikit-learn`, explores the data visually, trains multiple machine learning models, compares their performance, tunes a Random Forest classifier, and demonstrates predictions on sample flower measurements.

## Project File

- `IRIS_FLOWER_CLASSIFICATION.ipynb` - Main notebook containing data loading, visualization, model training, evaluation, tuning, and prediction demo.

## Dataset

The project uses the classic Iris dataset available through `sklearn.datasets.load_iris()`.

The dataset contains 150 flower samples with four numerical features:

- Sepal length
- Sepal width
- Petal length
- Petal width

Each sample belongs to one of three Iris species.

## Features of the Notebook

- Loads and prepares the Iris dataset
- Performs exploratory data analysis
- Checks class distribution and missing values
- Creates visualizations for feature relationships and correlations
- Splits the dataset into training and testing sets
- Standardizes feature values using `StandardScaler`
- Trains and compares multiple classifiers:
  - Logistic Regression
  - Decision Tree
  - Random Forest
  - Support Vector Machine
  - K-Nearest Neighbors
  - Gradient Boosting
- Evaluates models using accuracy, cross-validation, classification report, and confusion matrix
- Displays feature importance using Random Forest
- Performs hyperparameter tuning with `GridSearchCV`
- Predicts species for sample flower measurements

## Generated Outputs

When the notebook is run, it saves the following visualization files:

- `iris_correlation.png`
- `iris_model_results.png`
- `iris_feature_importance.png`

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

3. Open `IRIS_FLOWER_CLASSIFICATION.ipynb`.
4. Run the notebook cells from top to bottom.

## Model Workflow

1. Load the Iris dataset.
2. Explore the dataset using summary statistics and visualizations.
3. Split the data into training and testing sets.
4. Scale the input features.
5. Train multiple classification models.
6. Compare model accuracy and cross-validation scores.
7. Select the best-performing model.
8. Tune the Random Forest model using grid search.
9. Use the trained model to make sample predictions.

## Conclusion

The Iris Flower Classification notebook demonstrates a complete beginner-friendly machine learning workflow, from data exploration to model evaluation and prediction. It is suitable for learning the basics of supervised classification using Python and scikit-learn.
