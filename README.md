#  Customer Churn Prediction

This project predicts customer churn using a dataset from a telecom company. A web app was also developed using Streamlit to allow user-friendly predictions.

---

##  Problem Statement

Customer churn occurs when customers stop doing business with a company. The goal is to predict which customers are likely to churn so that retention strategies can be applied proactively.

---

##  Dataset

- **Source**: Telco Customer Churn (Kaggle)
- **File**: `WA_Fn-UseC_-Telco-Customer-Churn.csv`
- **Features**: Demographics, services, and account info
- **Target**: `Churn` (Yes/No)

---

 ## Data Preprocessing

- Handled missing values in `TotalCharges`
- Converted `Churn` column to binary (Yes → 1, No → 0)
- Encoded categorical variables using One-Hot Encoding
- Scaled numerical features using `StandardScaler`

---

##  Models Used

- **Logistic Regression**
- **Random Forest Classifier**
    - With and without class balancing

---

##  Evaluation Metrics

- **Accuracy Score**
- **Classification Report**
- **Confusion Matrix**
- **Feature Importance Visualization (for Random Forest)**

---

##  Streamlit App

A web application is built using **Streamlit** to:

- Input customer details
- Predict if the customer is likely to churn
- Display model results interactively

To run the app locally:
```bash
streamlit run app.py


**Requirements**

Copy code
pandas
numpy
scikit-learn
streamlit
matplotlib
seaborn
joblib
