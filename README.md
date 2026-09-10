# OIBSIP
# Data Analytics - Level 1 - Task 3: Cleaning Data

## Project Overview
This project demonstrates professional-level data cleaning skills using the Titanic Passenger Dataset. The goal was to take a messy dataset and systematically transform it into a clean, analysis-ready dataset while documenting every decision.

## Dataset
- **Source**: Titanic Dataset
- **Original File**: `Titanic-Dataset.csv`
- **Cleaned File**: `Titanic-Cleaned.csv`

## Cleaning Steps Performed

| Step                        | Action Taken                          | Justification                                      |
|----------------------------|---------------------------------------|----------------------------------------------------|
| Missing Age                | Median imputation                     | Age is skewed; median is robust to outliers        |
| Missing Embarked           | Mode imputation                       | Only 2 missing values; mode is suitable for categorical data |
| Cabin                      | Dropped entire column                | 77% missing values — not useful for analysis       |
| Duplicates                 | Checked (0 found)                     | No duplicate rows present                          |
| Sex & Embarked             | Standardised (lower/upper + strip)    | Ensured consistency in categorical values          |
| PassengerId                | Converted to string                   | Identifier, not a numerical feature                |
| Age & Fare Outliers        | Capped using IQR method               | Preserved all rows while reducing extreme impact   |

## Tools Used
- Python
- Pandas
- NumPy
- Jupyter Notebook

## How to Run
1. Open `cleaning_data.ipynb` in Jupyter Notebook / JupyterLab
2. Run all cells sequentially
3. The cleaned dataset will be saved as `Titanic-Cleaned.csv`

## Results
- **Before Cleaning**: 891 rows × 12 columns (with significant missing values)
- **After Cleaning**: 891 rows × 11 columns (clean and consistent)

## Author
Pranjal Gupta  
Oasis Infobyte Internship - Data Analytics Track
