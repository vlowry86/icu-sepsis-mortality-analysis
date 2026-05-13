# icu-sepsis-mortality-analysis
Healthcare data analysis project on ICU sepsis mortality

# ICU Sepsis Mortality Analysis

## Project Overview

This project analyzes ICU sepsis patient data to identify factors associated with patient mortality. The dataset includes demographic variables, vital signs, laboratory results, comorbidities, and ICU admission pathways.

The objective is to clean and preprocess real-world clinical data, engineer relevant health indicators, and perform exploratory analysis to understand key drivers of ICU mortality.

---

## Dataset

- Source: ICU sepsis clinical dataset (Kaggle)
- Number of records: ~2,800 patients
- Target variable: Mortality (0 = survived, 1 = deceased)
- Data includes:
  - Demographics (age, gender)
  - Clinical measurements (vitals, lab results)
  - Comorbidities
  - ICU admission characteristics

---

## Data Cleaning and Preprocessing

The following steps were performed to prepare the dataset:

- Handled missing values in laboratory and clinical variables
- Standardized categorical encodings (gender, admission type)
- Removed invalid mortality encoding (value = 3)
- Converted binary variables to consistent 0/1 format
- Ensured consistent data types across features

---

## Feature Engineering

The following features were created to support analysis:

- Comorbidity score (sum of chronic disease indicators)
- Missing value indicators for key laboratory tests
- Admission pathway categorization (Emergency vs Non-Emergency ICU)

---

## Exploratory Data Analysis

Key analyses performed include:

- Mortality rate calculation across patient subgroups
- Comparison of mortality by gender
- Comparison of mortality by ICU admission type
- Relationship between comorbidity burden and mortality
- Distribution analysis of key clinical variables

---

## Key Findings

- Overall ICU mortality rate was approximately 47.5%
- Older patients showed higher mortality rates
- Gender showed minimal difference in mortality outcomes
- Non-emergency ICU admissions were associated with higher mortality compared to emergency admissions
- Comorbidity score showed a non-linear relationship with mortality

---

## Tools and Technologies

- Python
- Pandas
- NumPy

---

## Repository Structure
icu-sepsis-mortality-analysis/
│
├── notebooks/
│ ├── 01_data_cleaning.ipynb
│ ├── 02_eda_analysis.ipynb
│
├── data/
├── images/
└── README.md


---

## Future Work

- Build predictive models for ICU mortality risk
- Perform feature importance analysis
- Develop dashboard for clinical visualization (Power BI or Tableau)
