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

