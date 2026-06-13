# Unemployment Analysis With Python

This project analyzes unemployment trends in India using Python. It was created for the AICTE Oasis Infobyte Internship task: **Unemployment Analysis With Python**.

The analysis is contained in the Jupyter notebook:

- `UNEMPLOYMENT_ANALYSIS_WITH_PYTHON.ipynb`

## Project Overview

The notebook performs an end-to-end exploratory data analysis of unemployment data. It loads the dataset, cleans and prepares the data, visualizes unemployment trends, compares regional unemployment rates, and studies the impact of COVID-19 on unemployment.

If the real dataset file is not available, the notebook automatically creates a realistic sample dataset so the analysis can still run.

## Features

- Loads unemployment data from CSV
- Generates sample unemployment data if the CSV file is missing
- Cleans column names and parses date fields
- Calculates yearly, monthly, regional, and area-wise unemployment trends
- Compares unemployment rates before, during, and after the COVID-19 period
- Creates multiple visualizations using Matplotlib and Seaborn
- Saves generated charts as PNG image files

## Dataset

The notebook expects the dataset file to be named:

```text
Unemployment in India.csv
```

Place this CSV file in the same folder as the notebook.

The expected dataset should include columns similar to:

- `Region`
- `Date`
- `Estimated Unemployment Rate (%)`
- `Estimated Employed`
- `Estimated Labour Participation Rate (%)`
- `Area`

The code also attempts to handle minor column-name variations such as region/state and date/month fields.

## Requirements

Install the required Python libraries before running the notebook:

```bash
pip install numpy pandas matplotlib seaborn jupyter
```

## How to Run

1. Open the project folder.
2. Add `Unemployment in India.csv` to the folder if you have the real dataset.
3. Start Jupyter Notebook:

```bash
jupyter notebook
```

4. Open `UNEMPLOYMENT_ANALYSIS_WITH_PYTHON.ipynb`.
5. Run all cells from top to bottom.

If the CSV file is not found, the notebook will use generated sample data.

## Generated Output Files

Running the notebook may create the following chart files:

- `unemployment_overview.png`
- `unemployment_regional_boxplot.png`
- `unemployment_vs_participation_scatter.png`
- `unemployment_covid_impact.png`
- `unemployment_regional_heatmap.png`
- `unemployment_urban_rural.png`
- `unemployment_seasonality.png`

## Analysis Sections

The notebook includes the following main sections:

1. Data loading
2. Data cleaning and preprocessing
3. Exploratory data analysis
4. COVID-19 impact analysis
5. Regional unemployment heatmap
6. Urban vs rural unemployment comparison
7. Top and bottom unemployment regions
8. Monthly seasonality analysis
9. Final summary statistics

## Notes

- The notebook suppresses warnings for cleaner output.
- The generated sample data is only for demonstration purposes.
- For accurate results, use the original unemployment dataset.
