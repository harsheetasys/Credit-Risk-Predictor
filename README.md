# 💼 Credit Risk Predictor

## 📌 Overview

This project is a Jupyter Notebook (`Credit_Risk_Predictor.ipynb`) that demonstrates the development of a machine learning model to predict credit risk using a dataset of loan applicants. The model is built using **LightGBM**, a gradient boosting framework, and includes **SHAP** (SHapley Additive exPlanations) for model interpretability. The project also integrates **Gradio** for creating a simple user interface to interact with the model.

---

## ✨ Features

- ✅ Data Preprocessing: Handles missing values, encodes categorical features, and splits the dataset.
- ⚙️ Model Training: Uses LightGBM optimized for binary classification (loan default risk).
- 📊 Model Evaluation: Assesses performance with AUC and accuracy.
- 🔍 SHAP Analysis: Offers explainability through feature importance visuals.
- 🌐 Gradio Interface: Simple and interactive UI for testing predictions.

---

## 📦 Requirements

Install required libraries using:

```bash
pip install lightgbm shap pandas numpy streamlit gradio scikit-learn matplotlib

📂 Dataset
File: credit_risk_dataset.csv

Key features include:
person_age: Age of the applicant
person_income: Monthly income
person_home_ownership: Home ownership (encoded)
loan_intent: Purpose of the loan
loan_grade: Credit grade
loan_amnt: Loan amount
loan_int_rate: Interest rate
loan_status: Target variable (1 = default, 0 = no default)
Plus: employment length, credit history length, etc.

🧠 Model Performance
AUC: 0.9494
Accuracy: 0.9232
These results indicate strong model performance for predicting high-risk applicants.

🚀 How to Use
Run the Notebook: Open Credit_Risk_Predictor.ipynb in Jupyter/Colab.
Data Prep: Ensure credit_risk_dataset.csv is in the same directory or update the path.
Train the Model: Execute all cells for preprocessing, training, and evaluation.
SHAP Analysis: View SHAP summary and force plots.
Launch Gradio: Use the Gradio interface for live prediction testing.

🧪 Example Usage
Using the Gradio Interface
Input:
Age
Income
Home ownership status
Loan intent
Loan amount
Interest rate
Credit history length

🟢 Output: Risk probability (chance of default).

🔎 SHAP Interpretation
SHAP values reveal the influence of each feature on model predictions.
Examples:
🔺 High interest rate ⟶ ↑ Default risk
🔻 Long credit history ⟶ ↓ Default risk
🔺 Low income ⟶ ↑ Default risk

📈 Future Improvements
🔬 Additional feature engineering
🎯 Hyperparameter tuning (GridSearchCV/Bayesian methods)

🌐 Deployment using Streamlit or Flask

📡 Integration with real-time loan applicant data

