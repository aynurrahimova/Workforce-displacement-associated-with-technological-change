README

**Author:** Aynur Rahimova

# Workforce Displacement & Technological Change
###  Project Title:

**Evaluating the Impact of Semiconductor Adoption and Technological Change on Occupational Shifts and Workforce Displacement Across Major Industries**


##  Project Overview

This project integrates trade-based semiconductor adoption metrics, innovation indicators, and occupational data to assess the effects of technological change on labor markets across major industries. I built a supervised regression machine learning model that predicts occupational shifts and workforce displacement in relation to semiconductor trade patterns and innovation intensity.


## Problem Statement
Rapid technological progress can automate tasks, transform job roles, and reshape labor demand.

The objectives of this project are to:
- Measure the relationship between semiconductor adoption and employment growth
- Identify occupations and industries most sensitive to technological change
- Build predictive models that explain workforce displacement patterns

## Data Sources
This project integrates three global datasets:

1. **UN Comtrade – Semiconductor Trade Data (2000–2024)**  
   Measures semiconductor adoption through trade values, quantities, and flow directions.

2. **ILOSTAT – Employment by Occupation (2000–2023)**  
   Provides employment levels by country, occupation, and gender (target variable).

3. **World Bank – R&D Expenditure (% of GDP)**  
   Represents national innovation intensity and technological capacity.

> ⚠️ Datasets are not included in this repository due to size.

## Tools & Technologies
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Random Forest
- LightGBM
- FLAML AutoML
- H2O AutoML

## Project Structure
workforce-displacement-technological-change/
├── Data/
│ ├── Raw/
│ └── Processed/
├── Notebooks/
│ ├── Preprocessing.ipynb
│ ├── EDA_Feature_Engineering.ipynb
│ └── Modeling.ipynb
├── README.md
├── requirements.txt
└── .gitignore


## Methodology
### 1. Data Preparation
- Cleaned and merged semiconductor trade, employment, and R&D datasets
- Applied quality filters to retain reliable labor market estimates
- Engineered semiconductor adoption indicators and employment growth target

### 2. Exploratory Data Analysis & Feature Engineering
- Analyzed employment growth patterns by country, occupation, and industry
- Created adoption shock indices and missing-value signal flags
- Applied log transformations and outlier handling
- Used Phik correlation to capture non-linear relationships

### 3. Modeling
- Trained and evaluated multiple models:
  - Ridge Regression
  - Random Forest
  - Gradient Boosting
  - Histogram GB
  - LightGBM
  - XGBoost
  - CatBoost
  - AutoML (FLAML, H2O)
- Addressed overfitting through feature selection, cross-validation, and model comparison
- Evaluated models using R², RMSE, and MAE

## Key Results
- Identified occupations and industries most sensitive to semiconductor adoption
- Observed stronger technology–employment relationships in tech-leading countries
- Best-performing model: **H2O AutoML GBM**
  - Test R² ≈ **0.96**
  - Overfitting ≈ **2–3%**

## Model Interpretation
- Compared top-performing models using:
  - Predicted vs Actual plots
  - Residual analysis
  - Error distributions
- Analyzed prediction errors across employment deciles to assess robustness

## Conclusion
This project demonstrates how global technology adoption—proxied through semiconductor trade and innovation investment—relates to workforce transformation. The final model captures employment growth patterns with high accuracy while highlighting that extreme or rare country–occupation combinations remain more difficult to predict. Overall, the results provide meaningful insights into workforce displacement during periods of rapid technological change.

## Key Learnings
- Integrating heterogeneous global datasets
- Handling non-linear and real-world data
- Managing overfitting in tree-based models
- Communicating socio-economic insights from machine learning results
- 
## Contact Me
- 💼 [LinkedIn](https://www.linkedin.com/in/aynur-rahimova-839078225)  
- 🐙 [GitHub](https://github.com/aynurrahimova/bank-transaction-fraud-detection-ml)
- 📧 Email: raynur.ar@gmail.com
