# Loan Default Prediction using Machine Learning

## Project Overview

This project focuses on predicting loan default risk using machine learning techniques. A Random Forest classifier is trained on financial data such as income, debt, and credit information to classify whether a borrower is likely to default on a loan.

The project also includes explainability using SHAP and fairness analysis across age groups to evaluate ethical considerations in the model.

---

## Dataset

The dataset used is `bank-loan.csv`, which contains the following features:

- age  
- ed (education)  
- employ (years employed)  
- address (years at current address)  
- income  
- debtinc (debt-to-income ratio)  
- creddebt (credit card debt)  
- othdebt (other debt)  
- default (target variable)

---

## ⚙️ Project Workflow

### 1. Data Analysis & Cleaning
- Checked for missing values
- Performed exploratory data analysis (EDA)
- Visualized distributions and correlations

### 2. Feature Engineering
- Created additional features such as total debt and debt ratios
- Scaled numerical features using StandardScaler

### 3. Model Building
- Trained a Random Forest classifier
- Evaluated using accuracy, confusion matrix, and classification report

### 4. Explainability (SHAP)
- Used SHAP to interpret model predictions
- Identified key drivers such as debt-to-income ratio and income

### 5. Fairness Analysis
- Evaluated model performance across age groups
- Compared predicted default rates across demographic segments

---

## Model Performance

- Model: Random Forest Classifier  
- Evaluation Metrics: Accuracy, Precision, Recall, F1-score  
- Feature Importance: Debt-related variables were most influential  

---

## Explainability

SHAP analysis showed that:
- Higher debt increases likelihood of default
- Higher income reduces default risk
- Debt-to-income ratio is a key predictive factor

---

## Fairness Analysis

Fairness was evaluated using age groups due to lack of gender or ethnicity data.

Findings:
- Younger individuals tend to have higher predicted default rates
- Some variation exists across age groups

This highlights potential bias risks in the model.

---

## Ethical Considerations

- **Fairness:** Limited by lack of demographic attributes  
- **Transparency:** Improved using SHAP explainability  
- **Privacy:** No personal identifiers included in dataset  
- **Bias Risk:** Model may reflect patterns in historical data  

---

## Tools & Technologies

- Python  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn  
- SHAP  

---

## Conclusion

This project demonstrates how machine learning can be used for loan default prediction while incorporating explainability and fairness analysis. Although the model performs well, ethical considerations such as bias and fairness must be addressed before real-world deployment.

---

## How to Run

1. Clone the repository  
2. Install dependencies: pip install -r requirements.txt
3. Run the Jupyter Notebook

---

## Author: Alyssa I

