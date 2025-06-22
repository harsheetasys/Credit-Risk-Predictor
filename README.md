# 💼 Credit Risk Predictor

## 📌 Overview

This project is a Jupyter Notebook (`Credit_Risk_Predictor.ipynb`) that demonstrates the development of a machine learning model to predict credit risk using a dataset of loan applicants. The model is built using **LightGBM**, a gradient boosting framework, and includes **SHAP** (SHapley Additive exPlanations) for model interpretability. The project also integrates **Gradio** for creating a simple user interface to interact with the model.

---

## ✨ Features

- ✅ **Data Preprocessing**: Handles missing values, encodes categorical features, and splits the dataset.
- ⚙️ **Model Training**: Uses LightGBM optimized for binary classification (loan default risk).
- 📊 **Model Evaluation**: Assesses performance with AUC and accuracy.
- 🔍 **SHAP Analysis**: Offers explainability through feature importance visuals.
- 🌐 **Gradio Interface**: Simple and interactive UI for testing predictions.

---

## 📦 Requirements

Install required libraries using:

```bash
pip install lightgbm shap pandas numpy streamlit gradio scikit-learn matplotlib

---
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
Additional: employment length, credit history length, etc.

🧠 Model Performance
AUC: 0.9494
Accuracy: 0.9232
These results indicate strong model performance for predicting high-risk applicants.

🚀 How to Use
Run the Notebook: Open Credit_Risk_Predictor.ipynb in Jupyter or Google Colab.
Data Prep: Make sure credit_risk_dataset.csv is in the same folder or update the path.
Train the Model: Execute all cells to preprocess, train, and evaluate the model.
SHAP Analysis: Run cells to visualize SHAP summary and feature contributions.
Launch Gradio: Use the Gradio interface to input applicant details and get predictions.

🧪 Example Usage
🎛️ Using the Gradio Interface
Input:
Age
Income
Home ownership status
Loan intent
Loan amount
Interest rate
Credit history length
🟢 Output: Probability of default (credit risk score)

🔎 SHAP Interpretation
SHAP values explain the model’s decision by highlighting the impact of each feature.
Examples:
🔺 High interest rate ⟶ ↑ Default risk
🔻 Long credit history ⟶ ↓ Default risk
🔺 Low income ⟶ ↑ Default risk

📈 Future Improvements
🔬 Additional feature engineering
🎯 Hyperparameter tuning (e.g., GridSearchCV, Bayesian optimization)
🌐 Deployment using Streamlit or Flask
📡 Real-time data pipeline integration
