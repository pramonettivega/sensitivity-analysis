# ENLACE Summer Research Program 2025

**Workflows for Wildfire Management**

**Authors:**  
Luis Angel Castaneda Barron (CETYS Universidad)  
Said Carbot Cruz Trejo (Instituto Politécnico Nacional)  
Grecia Paola Siono Gutierrez (UC San Diego)  

---

## Explanation of Workflow

### 1. Exploratory Data Analysis (EDA)

- **Input:** `250710_bp3d_db_data.csv` (the raw dataset)  
- **Process:**  
  - Explore the dataset to understand its variables, types, and contents.  
  - Identify data distribution, potential issues, and variables of interest.  
- **Output Notebook:** `EDA.ipynb` (documents the exploratory analysis)

---

### 2. Data Cleaning

- **Input:** `250710_bp3d_db_data.csv` (same raw dataset)  
- **Process:**  
  - Remove duplicates, outliers, and null values.  
  - Prepare a cleaned dataset suitable for modeling.  
- **Output:** `df_cleaned.csv` (cleaned dataset)  
- **Associated Notebook:** `data_preprocessing.ipynb` (handles the data cleaning steps)

---

### 3. Sensitivity Analysis (SA) using Machine Learning and SHAP Analysis

- **Input:** `df_cleaned.csv` (cleaned dataset)  
- **Process:**  

#### a. Model Training  
- Train a **Random Forest Regressor**  
- Train an **XGBoost Model**

#### b. SHAP Analysis  
- Compute **SHAP (SHapley Additive exPlanations)** values to determine the importance of each input variable for the three target variables:  
  - *Surface consumed*  
  - *Midstory consumed*  
  - *Canopy consumed*  
- Generate SHAP summary plots to visualize feature impacts.

#### c. Important Notes  
- Some data cleaning also occurs in these notebooks to test SHAP sensitivity.  
- After discussions with Leticia and Pedro, the final data cleaning included:  
  - Eliminating: *side to start ignition, blackline width, wind height, firing technique, dash length*  
  - Removing NaN values  

- **Outputs:**  
  - `SA_RF_SHAP.ipynb` (Random Forest SHAP analysis)  
  - `SA_XGBoost_SHAP.ipynb` (XGBoost SHAP analysis)

---

The previously described process is shown visually in **Figure 1**.
