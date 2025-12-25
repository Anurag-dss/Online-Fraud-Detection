🛡️ Online Fraud Detection System

The Online Fraud Detection System is my first machine learning project, developed to understand how machine learning can be used to detect fraudulent online transactions.
In this project, I analyze transaction data, explore different patterns, and build a basic machine learning model to classify transactions as fraudulent or legitimate.

This project helped me learn important concepts such as data preprocessing, exploratory data analysis (EDA), handling imbalanced datasets, and evaluating classification models.
---

## 📌 Introduction

With the rapid expansion of digital payments, online fraud has become a serious challenge for financial institutions. Fraudulent transactions are rare but highly damaging, making detection difficult due to:

* Extreme class imbalance
* High transaction volumes
* Evolving fraud patterns

This project focuses on **detecting fraud with high recall**, ensuring that most fraudulent transactions are successfully identified.

---

## 🎯 Project Objectives

| Objective               | Explanation                                                       |
| ----------------------- | ----------------------------------------------------------------- |
| Fraud Identification    | Detect fraudulent transactions accurately                         |
| Pattern Analysis        | Understand how fraud varies by transaction type, amount, and time |
| Data Imbalance Handling | Address skewed fraud vs non-fraud distribution                    |
| Model Evaluation        | Analyze precision, recall, and overall reliability                |
| Visualization           | Make fraud behavior interpretable through plots                   |

---

## 🧰 Technology Stack

| Category             | Tools               |
| -------------------- | ------------------- |
| Programming Language | Python              |
| Data Analysis        | Pandas, NumPy       |
| Visualization        | Matplotlib, Seaborn |
| Machine Learning     | Scikit-learn        |
| Environment          | Jupyter Notebook    |



## 📊 Dataset Description

The dataset consists of **millions of online transaction records**, containing both legitimate and fraudulent transactions.

| Feature        | Description                                    |
| -------------- | ---------------------------------------------- |
| type           | Type of transaction (TRANSFER, CASH_OUT, etc.) |
| amount         | Transaction value                              |
| step           | Time unit of the transaction                   |
| isFraud        | Fraud indicator (1 = Fraud, 0 = Legitimate)    |
| balance fields | Sender and receiver account balances           |

---

## 🔍 Exploratory Data Analysis (EDA)

### Transaction Types Distribution

<img width="763" height="665" alt="image" src="https://github.com/user-attachments/assets/cd9e6607-d2c0-4af3-bebf-b60133d96efe" />


**Insight:**
The dataset is dominated by a few transaction types, while fraud is concentrated in specific categories.

---

### Fraud Rate by Transaction Type

<img width="744" height="649" alt="image" src="https://github.com/user-attachments/assets/6458c041-e579-44cd-999d-faa6a4bbfcc8" />


**Insight:**
Certain transaction types show **significantly higher fraud rates**, making them high-risk operations.

---

### Transaction Amount Distribution (Log Scale)

<img width="748" height="575" alt="image" src="https://github.com/user-attachments/assets/e99a5745-dbdd-4263-91a0-b80df56fb51e" />


**Insight:**
Transaction amounts are highly skewed, with most transactions being small and few extremely large values.

---

### Amount vs Fraud Comparison

<img width="748" height="569" alt="image" src="https://github.com/user-attachments/assets/0ceff1d9-56fa-49c9-bada-72821518e730" />


**Insight:**
Fraudulent transactions typically involve **higher monetary values** compared to legitimate ones.

---

### Fraud Occurrence Over Time

<img width="709" height="575" alt="image" src="https://github.com/user-attachments/assets/10334762-2476-4d6c-a084-8b01eba4dcce" />


**Insight:**
Fraud activity fluctuates over time, indicating possible **temporal fraud patterns**.

---

### Correlation Matrix

<img width="793" height="687" alt="image" src="https://github.com/user-attachments/assets/3e1c29b2-24b8-4448-8d95-f6dc85d43965" />


**Insight:**
Balance-related features show strong relationships with fraud behavior.

---

## 🧠 Machine Learning Model

### Algorithm Used

**Logistic Regression**

### Why Logistic Regression?

* Effective for binary classification
* Scales well for large datasets
* Easy to interpret
* Works well with class-imbalanced data

---

## 🔄 Data Preprocessing

The following steps were applied before model training:

* Removal of irrelevant or identifier columns
* Handling missing values
* Encoding categorical variables
* Scaling numerical features
* Stratified train-test split to preserve fraud ratio

A **pipeline approach** was used to ensure consistent preprocessing and training.

---

## 📈 Model Evaluation

### Classification Performance Summary

| precision    recall  f1-score   support

           0       1.00      0.95      0.97   1270881
           1       0.02      0.94      0.04      1643

    accuracy                           0.95   1272524
   macro avg       0.51      0.94      0.51   1272524
weighted avg       1.00      0.95      0.97   1272524


**Overall Accuracy:** ~95%

---

### Confusion Matrix

<img width="652" height="590" alt="image" src="https://github.com/user-attachments/assets/95ce4213-e016-4206-83ba-df72c5a3db14" />


**Key Observation:**
The model achieves **high fraud recall**, which is crucial in fraud detection systems where missing a fraud is costlier than a false alarm.

---

## ▶️ How to Run the Project

1. Clone the repository
2. Install required Python libraries
3. Open `Fraud_Detection.ipynb` in Jupyter Notebook
4. Run all cells to reproduce analysis and results

---

## 🚀 Future Enhancements

* Use advanced models like Random Forest or XGBoost
* Apply SMOTE or anomaly detection techniques
* Real-time fraud detection using Flask or FastAPI
* Deploy model using cloud platforms
* Improve precision through threshold optimization

---

## 📚 References (Reputable Sources)

* Kaggle Credit Card Fraud Dataset
  [https://www.kaggle.com/mlg-ulb/creditcardfraud](https://www.kaggle.com/mlg-ulb/creditcardfraud)

* IEEE Research on Fraud Detection
  [https://ieeexplore.ieee.org/document/9416851](https://ieeexplore.ieee.org/document/9416851)

* IBM Logistic Regression Guide
  [https://www.ibm.com/topics/logistic-regression](https://www.ibm.com/topics/logistic-regression)


---

## 👤 Author

**Anurag Das**
Machine Learning Project – Online Fraud Detection System


