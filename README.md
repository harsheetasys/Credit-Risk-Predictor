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

## 📂 Dataset
The dataset `credit_risk_dataset.csv` contains the following key features:
- **person_age**: Age of the applicant  
- **person_income**: Monthly income  
- **person_home_ownership**: Home ownership status (encoded)  
- **loan_intent**: Purpose of the loan  
- **loan_grade**: Credit grade  
- **loan_amnt**: Loan amount  
- **loan_int_rate**: Interest rate  
- **loan_status**: Target variable (`1` = default, `0` = no default)  
- Additional features: Employment length, credit history length, etc.  

## 🧠 Model Performance
- **AUC**: 0.9494  
- **Accuracy**: 0.9232  
These metrics indicate strong predictive performance for identifying high-risk loan applicants.  

## � How to Use
1. **Run the Notebook**:  
   - Open `Credit_Risk_Predictor.ipynb` in **Jupyter Notebook** or **Google Colab**.  
2. **Data Preparation**:  
   - Ensure `credit_risk_dataset.csv` is in the same directory or update the file path in the notebook.  
3. **Train the Model**:  
   - Execute all cells to preprocess data, train, and evaluate the model.  
4. **SHAP Analysis**:  
   - Run the relevant cells to visualize SHAP summary plots and feature contributions.  
5. **Launch Gradio Interface**:  
   - Use the interactive Gradio app to input applicant details and receive risk predictions.  

## 🧪 Example Usage
### 🎛️ Gradio Interface Inputs:
- Age  
- Income  
- Home ownership status  
- Loan intent  
- Loan amount  
- Interest rate  
- Credit history length  

### 🟢 Output:
- **Probability of default** (credit risk score)  

## 🔎 SHAP Interpretation
SHAP values explain model decisions by quantifying feature impacts:
- 🔺 **High interest rate** → ↑ Default risk  
- 🔻 **Long credit history** → ↓ Default risk  
- 🔺 **Low income** → ↑ Default risk  

## 📈 Future Improvements
- 🔬 **Feature engineering** (e.g., derive new metrics)  
- 🎯 **Hyperparameter tuning** (GridSearchCV, Bayesian optimization)  
- 🌐 **Deployment** via Streamlit or Flask  
- 📡 **Real-time data pipeline** integration  

---

🚀 **Quick Start**:  
```bash
jupyter notebook Credit_Risk_Predictor.ipynb
## 📦 Requirements

Install required libraries using:

```bash
pip install lightgbm shap pandas numpy streamlit gradio scikit-learn matplotlib
