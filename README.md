# Titanic Survival Analysis & Prediction

## 📌 Project Description
This project analyzes the Titanic passenger dataset from the famous Kaggle competition.  
The aim is to explore the data, perform univariate and bivariate analysis, handle missing values, and prepare the dataset for further modeling.

---

## 📂 Repository Structure
- `train.csv` → Training dataset with passenger details and survival labels.
- `test.csv` → Test dataset with passenger details (without survival labels).
- `gender_submission.csv` → Example submission file from Kaggle.
- `titanic_analysis.ipynb` → Main Jupyter Notebook with analysis steps and visualizations.
- `README.md` → Project documentation.

---

## 🛠 What I Did
### 1. Data Loading & Overview
- Loaded `train.csv`, `test.csv`, and `gender_submission.csv` into Pandas DataFrames.
- Inspected datasets using `.info()` and `.describe()`.

### 2. Missing Value Handling
- Checked missing values for all columns.
- Imputed missing `Age` values with median.
- Filled missing `Embarked` values with mode.
- Replaced missing `Fare` in test set with median.
- Kept `Cabin` column as-is for now (too many missing values).

### 3. Descriptive Statistics
- Generated `.describe(include='all')` for numerical and categorical columns.
- Obtained value counts for categorical features in `train`, `test`, and `gender_submission`.

### 4. Univariate Analysis
- Analyzed distributions for `Age`, `Fare`, and `Pclass`.
- Created count plots for `Survived` in training and gender_submission datasets.

### 5. Bivariate Analysis
- Boxplots: `Age` vs `Pclass`, `Fare` vs `Pclass`.
- Scatterplot: `Age` vs `Fare` colored by `Pclass`.
- Correlation matrix for numeric features in both train and test datasets (displayed as numbers, not only heatmaps).

### 6. Gender Submission Insights
- Counted survival values and calculated percentages for 0 (Did not survive) and 1 (Survived).

---

## 📊 Key Insights (Summary)
- Higher survival rates were observed in certain passenger groups (e.g., higher classes, females).
- Fare and Pclass are negatively correlated.
- Age has a varied distribution across different Pclasses.

---

## 🚀 Next Steps
- Feature engineering (e.g., extracting title from Name, creating family size feature).
- Model training with Logistic Regression, Random Forest, etc.
- Cross-validation and hyperparameter tuning.

---
