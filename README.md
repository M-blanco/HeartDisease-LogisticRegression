# Cardiovascular Risk Analysis with Logistic Regression

This project implements a logistic regression model to predict cardiovascular risk based on patient data. It uses a dataset of clinical indicators to preprocess, clean, and train a model that can classify patients into risk categories.

---

## Objectives

- **Feature Engineering**: Process raw data to create meaningful features such as LDL and ApoB from existing columns.
- **Outlier Detection**: Identify and handle outliers using the interquartile range (IQR) method.
- **Predictive Modeling**: Train a logistic regression model to predict whether a patient has a high cardiovascular risk.
- **Evaluation**: Assess the model's performance using metrics like accuracy, classification reports, and model coefficients.

---

## Dataset

The dataset includes the following clinical indicators:
- **Age**: Patient's age.
- **Systolic**: Systolic blood pressure.
- **LDL**: Low-density lipoprotein cholesterol.
- **ApoB**: Apolipoprotein B (calculated).
- **isMale**: Gender.
- **isSmoker**: Smoking status.
- **isDiabetic**: Diabetes status.
- **Risk**: Numerical score representing cardiovascular risk.

---

## Key Features

1. **Data Cleaning**:
   - Dropped irrelevant columns like `isBlack` and `isHypertensive`.
   - Generated new columns (`LDL`, `ApoB`) and dropped redundant ones.

2. **Outlier Handling**:
   - Used the IQR method to identify outliers in numerical features.

3. **Model Training**:
   - Trained a logistic regression model using the `sklearn` library.
   - Split data into training (80%) and testing (20%) sets.

4. **Model Evaluation**:
   - Evaluated model accuracy on the test set.
   - Extracted model coefficients and intercepts to interpret feature contributions.

