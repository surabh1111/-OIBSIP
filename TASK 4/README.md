# Email Spam Detection with Machine Learning

This project is a Jupyter Notebook implementation of an email spam detection system. It uses text preprocessing, TF-IDF feature extraction, and multiple machine learning classifiers to classify messages as spam or ham.

## Project Overview

The notebook performs the full machine learning workflow:

- Loads an email dataset from `spam.csv` or `mail_data.csv`
- Falls back to generated sample data if no CSV dataset is available
- Cleans and preprocesses email text
- Performs exploratory data analysis
- Converts text into TF-IDF features
- Trains and compares multiple classification models
- Selects the best model using F1 score
- Generates visualizations and demo predictions

## Files

- `EMAIL_SPAM_DETECTION_WITH_MACHINE_LEARNING.ipynb` - Main notebook containing data preparation, model training, evaluation, and prediction examples.
- `README.md` - Project documentation.

Generated output files may include:

- `spam_model_results.png`
- Additional visualization images created by the notebook

## Models Used

The notebook compares the following models:

- Multinomial Naive Bayes
- Bernoulli Naive Bayes
- Logistic Regression
- Linear Support Vector Machine
- Random Forest Classifier

## Requirements

Install the required Python libraries before running the notebook:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

## Dataset

The notebook supports either of these dataset files placed in the same folder as the notebook:

- `spam.csv`
- `mail_data.csv`

Expected columns:

- For `spam.csv`: `v1` for label and `v2` for message
- For `mail_data.csv`: label/category column and message column

If no dataset file is found, the notebook automatically creates a sample dataset for demonstration.

## How to Run

1. Open the project folder.
2. Start Jupyter Notebook:

```bash
jupyter notebook
```

3. Open `EMAIL_SPAM_DETECTION_WITH_MACHINE_LEARNING.ipynb`.
4. Run all cells from top to bottom.

## Output

The notebook prints:

- Dataset information
- Cleaning and preprocessing status
- Model performance metrics
- Best model based on F1 score
- Classification report
- Demo predictions for sample email messages

It also displays and saves visualizations for exploratory analysis and model evaluation.

## Purpose

This project was created as Task 4 for an AICTE Oasis Infobyte Internship and demonstrates how machine learning can be used to detect spam emails using natural language processing techniques.
