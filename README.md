# 💳 Credit Card Fraud Detection using Machine Learning

## 🚀 Overview
This project focuses on detecting fraudulent credit card transactions using machine learning techniques.

Due to the highly imbalanced nature of the dataset, the main challenge is to accurately identify fraud cases while minimizing false positives.

The goal is to build and evaluate models that can effectively distinguish between legitimate and fraudulent transactions.

---

## 📂 Dataset
The dataset contains anonymized credit card transactions.

- Features are numerical (transformed using PCA)
- Highly imbalanced dataset:
  - Fraud cases represent a very small percentage of total transactions

---

## ⚙️ Approach

The project follows a complete machine learning pipeline:

- Data preprocessing and cleaning  
- Exploratory Data Analysis (EDA)  
- Handling class imbalance (e.g., SMOTE / undersampling)  
- Model training and comparison  

---

## 🤖 Models Used

- Logistic Regression  
- Decision Tree  
- Random Forest  

---

## 📊 Evaluation Metrics

Since accuracy is not reliable for imbalanced datasets, the following metrics were used:

- Precision  
- Recall  
- F1-score  
- Confusion Matrix  
- ROC-AUC Score  

---

## 📈 Results

- Best performing model: (write your best model here)
- Key insight:
  - High recall is critical for detecting fraud cases
  - There is a trade-off between precision and false positives

---

## 🛠️ Tech Stack

- Python  
- Pandas  
- NumPy  
- Matplotlib / Seaborn  
- Scikit-learn  

---

## ▶️ How to Run

```bash
git clone <your-repo-link>
cd credit-card-fraud-detection
pip install -r requirements.txt
jupyter notebook 
