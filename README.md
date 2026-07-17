# 💳 Credit Card Fraud Detection System

A machine learning project that detects fraudulent credit card transactions from a real-world highly imbalanced dataset.

---

## 📌 Project Description

This project identifies fraudulent credit card transactions from a dataset of 284,807 transactions where only 0.17% are fraud. It covers the complete ML pipeline including EDA, preprocessing, model training, hyperparameter tuning, and evaluation using proper metrics for imbalanced data.

---

## 📁 Project Structure
final-project-credit-card-fraud-detection/
│
├── AI_ML_FinalProject_Credit_Card_Fraud_Detection.ipynb
├── best_model.pkl
├── scaler.pkl
├── requirements.txt
└── README.md

---

## 📊 Dataset

- **Source:** [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Total Transactions:** 284,807
- **Fraud Cases:** 492 (0.17%)
- **Features:** 30 (V1-V28 PCA features + Time + Amount)
- **Target:** Class (0 = Legitimate, 1 = Fraud)

> Dataset not included in this repo due to file size. Download from Kaggle link above.

---

## 🛠️ Tech Stack

- Python
- pandas
- NumPy
- scikit-learn
- matplotlib
- seaborn
- joblib

---

## 🔄 ML Pipeline

1. Exploratory Data Analysis (EDA)
2. Feature Scaling (StandardScaler)
3. Train-Test Split (stratified)
4. Model Training
5. Overfitting Detection
6. Cross-Validation (5-Fold)
7. Hyperparameter Tuning (GridSearchCV)
8. Model Evaluation
9. Feature Importance Analysis

---

## 🤖 Models Used

| Model | Description |
|-------|-------------|
| Logistic Regression | Baseline model with class weights |
| Decision Tree | Non-linear classifier with class weights |
| Random Forest | Best performing ensemble model |

---

## 📈 Evaluation Metrics

| Metric | Why Used |
|--------|----------|
| Precision | Avoid false alarms |
| Recall | Catch maximum fraud cases |
| F1 Score | Balance Precision and Recall |
| ROC-AUC | Overall discrimination ability |

> Accuracy is NOT used as the primary metric — it is misleading on imbalanced datasets.

---

## 📉 Results

| Model | Precision | Recall | F1 Score | AUC |
|-------|-----------|--------|----------|-----|
| Logistic Regression | - | - | - | - |
| Decision Tree | - | - | - | - |
| Random Forest (Tuned) | - | - | - | - |

> Fill in your actual results after running the notebook.

---

## 🚀 How to Run

```bash
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/final-project-credit-card-fraud-detection.git

# 2. Install dependencies
pip install -r requirements.txt

# 3. Download dataset from Kaggle and place creditcard.csv in the project folder

# 4. Open the notebook in VS Code and run all cells
```

---

## 💡 Key Learnings

- Accuracy is misleading on imbalanced datasets
- Recall is the most critical metric for fraud detection
- Class weights effectively handle class imbalance
- Random Forest outperforms simpler models on complex fraud patterns
- GridSearchCV finds optimal hyperparameters systematically

---

## 🔮 Future Improvements

- Try SMOTE oversampling technique
- Implement XGBoost or LightGBM
- Build a real-time prediction API using Flask
- Deploy the model on a web interface
