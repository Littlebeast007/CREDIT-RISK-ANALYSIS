# CREDIT-RISK-ANALYSIS
Credit Risk Analysis using Random Forest

# Project Overview

Credit risk analysis is a critical function in banking and financial services, aimed at evaluating a borrower’s ability to repay a loan.
This project uses the German Credit Dataset to build a machine learning–based credit risk classification system using a Random Forest model.

The objective is to classify loan applicants as Good Credit Risk or Bad Credit Risk by analyzing demographic, financial, and credit history attributes. The project demonstrates a complete end-to-end credit analytics workflow, aligned with real-world responsibilities of a Credit Analyst / Risk Analyst.


#Business Objective

Assess creditworthiness of loan applicants

Minimize default risk

Support loan approval, rejection, or risk-based pricing decisions

Provide interpretable insights for credit decision-making

#Step-by-Step Data Analysis & Modeling
1️⃣ Data Loading & Initial Inspection

Load dataset into Pandas DataFrame

Inspect:

Shape of data

Column names and data types

Sample records

Check class balance between good and bad credit applicants

📌 Purpose: Understand structure, size, and target distribution before analysis.

2️⃣ Data Cleaning & Preprocessing

Verified dataset completeness (German Credit has no missing values)

Converted target variable into binary numeric format

Separated:

Numerical features

Categorical features

📌 Why this matters: Machine learning models require clean, numeric input.

3️⃣ Encoding Categorical Variables

Applied One-Hot Encoding for categorical features

Avoided ordinal assumptions for nominal variables

Ensured no information leakage from target variable

📌 Business relevance: Preserves real-world meaning of categorical borrower attributes.

4️⃣ Feature Scaling

Applied scaling to numerical variables where required

Ensured fair contribution of all numeric features

📌 Note: Random Forest is less sensitive to scaling, but preprocessing maintains consistency.

5️⃣ Exploratory Data Analysis (EDA)

Performed EDA to identify patterns influencing credit risk:

Distribution of credit amount and loan duration

#Machine Learning Model – Random Forest
6️⃣ Train-Test Split

Split data into:

80% Training

20% Testing

X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.2, random_state=42
)

7️⃣ Model Building

Used Random Forest Classifier due to:

High predictive accuracy

Ability to handle non-linear relationships

Built-in feature importance

Robustness to outliers



Credit risk variation by age group

Relationship between credit
