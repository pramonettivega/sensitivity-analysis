# Data Cleaning and Preprocessing Notebook

This Jupyter Notebook provides a step-by-step approach to cleaning and preprocessing a dataset containing various fuel and ignition-related parameters. The main goal is to prepare the data for further analysis or modeling by ensuring consistency, removing noise, and addressing common data quality issues.

## Features

- Loads and inspects raw dataset from `working_df_v3.csv`.
- Detects and removes outliers using the Interquartile Range (IQR) method.
- Handles missing values and fixes data inconsistencies.
- Encodes categorical variables using `LabelEncoder`.
- Ensures unified formatting and data types across all columns.
- Generates visualizations such as boxplots to inspect distributions.
- Prepares the dataset for further machine learning steps, including training a Random Forest Regressor.

## Cleaning Steps

1. Familiarize with the dataset structure
2. Remove duplicate entries
3. Drop irrelevant or unnecessary columns
4. Ensure consistency in data entries
5. Convert data types to appropriate formats
6. Standardize formatting across records
7. Handle missing values properly
8. Fix data entry errors
9. Remove or flag outliers (via boxplots)
10. Normalize data formats for modeling

## Libraries Used

- `pandas`, `numpy` – Data manipulation and analysis
- `matplotlib`, `seaborn` – Data visualization
- `scikit-learn` – Machine learning tools (e.g., `RandomForestRegressor`, `LabelEncoder`)
- `shap` – Model interpretability using SHAP values

## How to Use

1. Make sure the dataset `working_df_v3.csv` is in the same directory.
2. Open the notebook in Jupyter or JupyterLab.
3. Run each cell sequentially to reproduce the full data cleaning pipeline.

## Output

The notebook outputs a cleaned version of the dataset ready for modeling, along with relevant visualizations and summary statistics that reflect the effectiveness of each preprocessing step.

---

