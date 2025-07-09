# 💳 Credit Card Fraud Detection System

This project is a **machine learning-based web application** that detects fraudulent credit card transactions. It uses historical transaction data and classification algorithms to flag potential frauds in real-time.

<div align="center">
  <img src="https://img.shields.io/badge/Machine_Learning-Enabled-green" />
  <img src="https://img.shields.io/badge/Streamlit-UI-blue" />
  <img src="https://img.shields.io/badge/Python-3.10+-yellow" />
</div>

---

## 📌 Overview

Credit card fraud is a major problem for banks and consumers alike. This project analyzes transaction data and applies machine learning to predict whether a transaction is fraudulent.

The model is served using **Streamlit** to make predictions interactively from a simple web UI.

---

## 🧠 Features

- Trained Logistic Regression model with class imbalance handling using SMOTE
- Feature preprocessing using Scikit-Learn pipelines
- Real-time prediction UI with Streamlit
- Fraud probability displayed with alerts

---

## 📂 Project Structure

├── AIML Dataset.csv # Dataset file
├── credit_card_fraud_detection.ipynb # Jupyter notebook for EDA and model building
├── fraud_detection.py # Streamlit web app
├── fraud_detection_pipeline.pkl # Serialized ML pipeline
└── README.md # Project documentation


---

## 📊 Dataset

- **Source:** [Kaggle or AIML dataset] (custom)
- **Columns:**
  - `type`: Transaction type (`TRANSFER`, `CASH_OUT`, etc.)
  - `amount`: Transaction amount
  - `oldbalanceOrg`, `newbalanceOrig`: Sender's balances
  - `oldbalanceDest`, `newbalanceDest`: Receiver's balances
  - `isFraud`: Target variable

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/devansh-sharma15/Fraud_Detection_System.git
cd Fraud_Detection_System


2. Install Dependencies
bash
Copy code
pip install -r requirements.txt
Or manually install:

bash
Copy code
pip install pandas scikit-learn streamlit imbalanced-learn joblib
3. Run the Streamlit App
bash
Copy code
streamlit run fraud_detection.py
📌 How It Works
The model takes the following inputs:

Transaction type

Amount

Sender’s and Receiver’s balances before and after the transaction

It then uses a trained ML pipeline to output:

✅ Not Fraud – Transaction appears legitimate
❌ Fraud – Transaction is suspicious and flagged

📈 Model Info
Algorithm: Logistic Regression

Preprocessing:

StandardScaler for numerical features

OneHotEncoder for categorical (type)

Imbalance Handling: SMOTE

Evaluation Metrics: Accuracy, Precision, Recall, F1-Score, Confusion Matrix


📬 Contact
For queries or collaboration:

📧 devansh.sharma15032002@gmail.com

🔗 LinkedIn https://www.linkedin.com/in/devansh-sharma1503

🌐 GitHub  https://github.com/devansh-sharma15

