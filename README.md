# 📊 Customer Churn Prediction

A machine learning project that predicts whether a customer will churn (leave the service) based on their usage patterns, payment methods, and demographics. Built using Python, scikit-learn, and Streamlit.

---

## 🧠 Problem Statement

Customer churn is a critical metric for businesses. The earlier a company can predict churn, the better it can act to retain valuable customers. This project uses historical data to build a machine learning model that predicts if a customer is likely to churn.

---

## 📁 Dataset

- **Source**: [Telco Customer Churn - Kaggle](https://www.kaggle.com/blastchar/telco-customer-churn)
- **Size**: 7,043 rows × 21 columns
- Contains information about customer account, service usage, and churn status.

---

## 🔧 Features Used

- Demographics: Gender, Senior Citizen, Dependents, etc.
- Account Info: Tenure, Contract Type, Monthly Charges, Total Charges.
- Services: Internet Service, Phone Service, Streaming, etc.
- Target: `Churn` (Yes/No)

---

## ⚙️ ML Pipeline

1. **Data Cleaning**: Missing values handled, categorical features encoded.
2. **Feature Engineering**: One-hot encoding of non-numeric columns.
3. **Scaling**: StandardScaler used for numerical features.
4. **Model**: Random Forest Classifier.
5. **Evaluation**: Accuracy, confusion matrix, classification report.

---

## 🖥️ Streamlit Web App

A user-friendly web application built with Streamlit to:

- Input customer details
- Predict churn likelihood
- Display results interactively

### 🔄 To Run Locally:

```bash
git clone https://github.com/your-username/customer-churn-prediction.git
cd customer-churn-prediction
pip install -r requirements.txt
streamlit run app.py

## Requirements

pandas
numpy
scikit-learn
matplotlib
seaborn
joblib
streamlit
All dependencies are listed in requirements.txt


## Project Structure

customer-churn-prediction/
│
├── app.py                  # Streamlit web app
├── churn_model.pkl         # Trained model
├── scaler.pkl              # Standard scaler used during training
├── Telco-Customer-Churn.csv  # Dataset
├── churn_notebook.ipynb    # Data exploration, training
├── requirements.txt
└── README.md



