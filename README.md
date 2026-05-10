# 💳 Credit Card Fraud Detection — Classification Project

This project focuses on detecting fraudulent credit card transactions using machine learning.  
The main challenge is dealing with **highly imbalanced data**, where fraudulent transactions represent only a very small fraction of the dataset.

The goal is to build models that can accurately identify fraud while minimizing false positives.

---

## 📌 Problem Statement

Classify transactions as:
- `0` → Legitimate  
- `1` → Fraudulent  

The dataset is highly imbalanced, making standard accuracy an unreliable metric.

---

## 📊 Dataset

- Transactions: ~284,000  
- Fraud cases: ~0.17%  
- Features: 30  

### Feature Types:
- `V1 – V28`: PCA-transformed numerical features  
- `Time`, `Amount`: original features  
- `Class`: target variable  

---

## ⚠️ Key Challenge

- Extreme class imbalance  
- Model bias toward majority class (non-fraud)  
- Need for careful evaluation metrics  

---

## 🔍 Exploratory Data Analysis (EDA)

Performed analysis to understand the dataset:

- Checked class distribution (high imbalance)  
- Analyzed `Amount` and `Time` distributions  
- Visualized fraud vs non-fraud patterns  
- Correlation analysis between features  

### Key Insights:
- Fraud cases are extremely rare  
- Some features show different distributions for fraud vs non-fraud  
- `Amount` distribution is highly skewed  

---

## 🧹 Data Preprocessing

### ✔️ Scaling
- Scaled `Amount` using standardization  
- Dropped original `Time` if not informative  

---

### ✔️ Handling Imbalance

Used multiple strategies:

- Undersampling (reducing majority class)  
- Oversampling (increasing minority class)  
- SMOTE (Synthetic Minority Oversampling Technique)  

---

## 🧠 Modeling

Trained and compared multiple classification models:

- Logistic Regression  
- Decision Tree  
- Random Forest  
- Gradient Boosting  
- XGBoost  

---

## 🏗️ Pipeline Design

- Used Scikit-learn pipelines where needed  
- Applied preprocessing consistently  
- Ensured no data leakage  

---

## 🔧 Hyperparameter Tuning

Used **GridSearchCV** to optimize:
- Tree depth  
- Number of estimators  
- Learning rate  
- Regularization parameters  

---

## 📈 Evaluation Metrics

Due to class imbalance, used:

- Precision  
- Recall  
- F1 Score  
- ROC-AUC  

### Focus:
- High **recall** → detect as many fraud cases as possible  
- Balanced **precision** → reduce false alarms  

---

## 🏆 Results

- Baseline models struggled due to imbalance  
- Sampling techniques significantly improved performance  
- Ensemble models (Random Forest, XGBoost) performed best  
- Trade-off observed between precision and recall  

---

## 🛠️ Tech Stack

- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- Imbalanced-learn (SMOTE)  
- XGBoost  

---

## 🚀 How to Run

```bash
git clone <your-repo-link>
cd <repo-name>

pip install -r requirements.txt

jupyter notebook 
