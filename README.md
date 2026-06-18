# Heart Failure Diagnostic Prediction Model

An end-to-end machine learning project utilizing patient clinical data to predict heart failure risk. This notebook avoids data leakage by utilizing stratified splitting and implements cross-validation for evaluation.

## Dataset Insight
The dataset is loaded dynamically via a public raw URL stream, sourcing the `fedesoriano` Heart Failure Prediction dataset. It includes 11 clinical features such as Age, Sex, ChestPainType, Cholesterol, and MaxHR.

##  Tech Stack & Workflow
- **Languages/Libraries:** Python, Pandas, NumPy, Scikit-Learn
- **Exploratory Data Analysis (EDA):** Correlation matrix computations evaluated exclusively on training splits to prevent data leakage.
- **Validation Strategy:**  Cross-Validation targeting maximum **Recall** (minimizing false negatives in medical diagnostics).
- **Models Evaluated:** Random Forest Classifier vs. Logistic Regression.
