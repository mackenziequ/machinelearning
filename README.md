# Corporate Performance Analysis and Wage Prediction

This project analyzes the determinants of corporate performance using financial data from the Wharton Research Data Services (WRDS) and predicts wages using demographic and economic data from IPUMS USA. The objective is to uncover meaningful insights using statistical and machine learning methodologies.

---

## Table of Contents
1. [Introduction](#introduction)
2. [Dataset Description](#dataset-description)
3. [Analysis Outline](#analysis-outline)
4. [Reproducibility Steps](#reproducibility-steps)
5. [Results Summary](#results-summary)
6. [Citing the Data](#citing-the-data)

---

## Introduction

### Corporate Performance Analysis
This section focuses on determining the key factors influencing corporate performance from 2010-2020. The analysis uses metrics like Return on Assets (RoA) as the dependent variable and evaluates the influence of various corporate balance sheet characteristics.

### Wage Prediction
The second section of the project predicts individual wages using 2022 ACS sample data from IPUMS USA. Techniques like OLS, Lasso, and Ridge regression are used to identify the most effective model.

---

## Dataset Description

### Corporate Performance Dataset
- **Source**: Wharton Research Data Services (WRDS)
- **Period**: 2010-2020
- **Data Type**: Annual corporate financial data of North American companies.
- **Dependent Variable**: Return on Assets (RoA = Net Income / Total Assets)
- **Other Variables**: Debt-to-Assets Ratio, Current Ratio, Operating Income, and more.

### Wage Prediction Dataset
- **Source**: IPUMS USA
- **Sample**: 2022 ACS
- **Variables**: Wages, age, education, occupation, hours worked, etc.

---

## Analysis Outline

### Part 1: Corporate Performance
1. **Data Cleaning and Exploration**
   - Clean and preprocess the financial data.
   - Describe the dataset: size, type, and summary statistics.
   - Visualize the distribution of the outcome variable (RoA).
2. **Correlation Analysis**
   - Compute and visualize correlations between RoA and predictors.
3. **Modeling with OLS**
   - Specify and estimate an Ordinary Least Squares (OLS) model.
   - Interpret coefficients, R-squared, and key factors influencing RoA.

### Part 2: Wage Prediction
1. **Data Cleaning**
   - Preprocess IPUMS USA data for missing values and inconsistencies.
2. **Model Development**
   - Use OLS to develop an initial wage prediction model.
   - Apply Stepwise Selection, Lasso, and Ridge regression for feature selection.
   - Compare model performance and choose the best approach.

---

## Reproducibility Steps

### 1. Clone the Repository
```bash
git clone https://github.com/your-repo-name.git
cd your-repo-name
```

### 2. Set Up the Environment
```bash
Install dependencies from requirements.txt:
bash
Copy code
pip install -r requirements.txt
```
### 3. Data Acquisition
Download the corporate financial data (2010-2020) from WRDS.
Download the 2022 ACS sample from IPUMS USA.
### 4. Run the Analysis
Execute the provided Jupyter notebooks:
Corporate Performance Analysis: Q1_comp_financial.ipynb
Wage Prediction: Q2_LATEST.ipynb
Results Summary
Corporate Performance Analysis
Significant predictors of RoA include:
Debt-to-Assets Ratio
Operating Income
Current Ratio
Visualizations highlight the distribution and trends in RoA.
Wage Prediction
The best model for wage prediction was achieved using Ridge regression with optimized lambda (λ).
Key predictors included education level, occupation, and hours worked per week.


Citing the Data
WRDS Data
When using WRDS data in your research, cite as follows:

Wharton Research Data Services (WRDS). Wharton School of the University of Pennsylvania.

IPUMS USA Data
When using IPUMS USA data in your research, cite as follows:

Steven Ruggles, Sarah Flood, Miriam King, et al. IPUMS USA: Version 12.0 [dataset]. Minneapolis, MN: IPUMS, 2022.