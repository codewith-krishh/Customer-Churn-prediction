# Customer Churn Prediction (Machine Learning)

This project predicts whether a telecom customer will churn using historical customer data.

The goal is to identify customers likely to leave so businesses can take retention actions.

---

## Problem Type

Binary Classification

Target variable:

Churn  
0 → Customer stays  
1 → Customer leaves

---

## Dataset

Telco Customer Churn Dataset

Contains customer information such as:

- tenure
- contract type
- monthly charges
- internet services
- payment methods

---

## Project Workflow

1. Data Loading & Inspection
2. Data Cleaning
3. Exploratory Data Analysis (EDA)
4. Feature Encoding
5. Train/Test Split
6. Model Training
7. Cross Validation
8. Model Comparison

---

## Models Used

### Logistic Regression
Baseline interpretable model.

### Balanced Logistic Regression

Handled class imbalance using:
class_weight='balanced'


### Random Forest
Non-linear ensemble model.

---

## Model Performance

| Model | Accuracy | Recall (Churn) | Precision | F1 |
|------|------|------|------|------|
| Logistic Regression | 0.81 | 0.56 | 0.66 | 0.61 |
| Balanced Logistic | 0.74 | **0.78** | 0.51 | **0.61** |
| Random Forest | 0.79 | 0.50 | 0.62 | 0.55 |

---

## Key Insight

Balanced Logistic Regression significantly improved **recall for churn customers**.

Recall increased from **0.56 → 0.78**, meaning the model detects more customers likely to leave.

This is important because missing churn customers can directly impact revenue.

---

## Tools Used

- Python
- Pandas
- NumPy
- Seaborn / Matplotlib
- Scikit-learn

---

## Next Improvements 

To make this project closer to an industry ML workflow:

- Implement full **ML pipeline**
- Apply **GridSearchCV** for hyperparameter tuning
- Add **ROC-AUC evaluation**
- Analyze **feature importance**
- Improve model evaluation metrics

---

## Project Structure

```
customer-churn-ml/
│
├── dataset/
│ └── Telco-Customer-Churn.csv
│
├── notebook/
│ └── churn_analysis.ipynb
│
├── requirements.txt
│
├── .gitignore
│
└── README.md
```

---

## 📎 Author
Created by: **Krish**