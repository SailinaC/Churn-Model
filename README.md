# Customer Churn Prediction

## Overview
Predictive model to identify customers at high risk of churning for a retail e-commerce platform. Uses Random Forest classifier on customer behavioral and transactional data.

## Dataset
- **Target:** Churn flag (binary classification)
- **Features:** 19 variables including tenure, satisfaction score, order history, payment preferences, and device usage
- **Format:** Excel file with customer transaction data

## Methodology
1. **Data Preprocessing:** Handle missing values, encode categorical variables, scale features
2. **Model Training:** Random Forest with 100 estimators
3. **Evaluation:** Classification report, confusion matrix, ROC-AUC score
4. **Feature Analysis:** Identify key churn drivers

## Key Features
- Customer tenure and satisfaction scores
- Order frequency and payment preferences
- Device usage and app engagement
- Geographic and demographic factors

## Business Impact
- Proactive customer retention strategies
- Personalized offers and communications
- Improved customer lifetime value
- Reduced churn rates and increased profitability

## Usage
```python
# Load and preprocess data
df = pd.read_excel('data.xlsx')
# Train model
clf = RandomForestClassifier(n_estimators=100, random_state=42)
# Evaluate performance
print(classification_report(y_test, y_pred))
```

## Requirements
- pandas, numpy, matplotlib, seaborn
- scikit-learn
- Excel data file
