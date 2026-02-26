# 💳 Credit Card Fraud Detection

## 📌 Project Overview

This project builds a Machine Learning model to detect fraudulent credit card transactions. Fraud detection is a real-world classification problem with extremely imbalanced data, making it more complex than regular prediction tasks.

The goal is to identify fraudulent transactions accurately while minimizing false negatives.

---

## 🎯 Objectives

- Perform Exploratory Data Analysis (EDA)
- Handle extreme class imbalance
- Train a robust classification model
- Evaluate performance using proper classification metrics
- Focus on improving fraud recall and F1-score

---

## 📊 Dataset Information

Dataset: Credit Card Fraud Detection Dataset (European cardholders)

- Total transactions: 284,807
- Fraud cases: 492 (~0.17%)
- Features:
  - V1 to V28 (PCA transformed features)
  - Time
  - Amount
- Target variable:
  - 0 → Genuine transaction
  - 1 → Fraud transaction

⚠️ The dataset is highly imbalanced, so accuracy alone is not a reliable metric.

---

## 📥 Dataset Download

Due to GitHub file size limitations, the dataset is not included in this repository.

You can download the dataset from Kaggle:

https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

After downloading:

1. Place `creditcard.csv` inside the project folder.
2. Run the notebook.

---

## 🔎 Exploratory Data Analysis (EDA)

The following visualizations were performed:

- Class distribution countplot
- Fraud vs Genuine percentage pie chart
- Transaction amount distribution
- Fraud vs Genuine boxplot comparison
- Correlation heatmap
- Confusion matrix visualization
- Feature importance plot

### Key Insights

- Fraud transactions represent less than 0.2% of total data.
- Severe class imbalance required special handling.
- Certain PCA components contribute more significantly to fraud detection.

---

## ⚙️ Data Preprocessing

- Scaled `Time` and `Amount` using StandardScaler
- Split dataset into training and testing sets (80/20)
- Used stratified sampling to preserve class distribution
- Applied SMOTE (Synthetic Minority Oversampling Technique) to handle imbalance

---

## 🤖 Model Used

### Random Forest Classifier

Random Forest was selected because:

- Handles non-linear relationships effectively
- Performs well on imbalanced datasets
- Provides feature importance insights
- Improves recall for minority class

---

## 📈 Model Performance

### Test Set Results

- Accuracy: 99.97%
- Fraud Precision: 94%
- Fraud Recall: 88%
- Fraud F1-Score: 91%

### Confusion Matrix

|               | Predicted Genuine | Predicted Fraud |
|--------------|------------------|----------------|
| Actual Genuine | 48,632 | 5 |
| Actual Fraud   | 11 | 77 |

### Interpretation

- The model detected 88% of fraudulent transactions.
- Very low false positive rate (only 5 genuine transactions misclassified).
- Recall was prioritized to minimize financial risk.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn (SMOTE)

---

## 🚀 Future Improvements

- Hyperparameter tuning using GridSearchCV
- Threshold optimization to improve fraud recall
- Try advanced models like XGBoost or LightGBM
- Deploy using Streamlit
- Real-time fraud detection simulation

---

## 📌 Conclusion

This project demonstrates handling of real-world data challenges such as extreme class imbalance and evaluation beyond accuracy.

The Random Forest model achieved strong fraud detection performance with high precision and recall, making it suitable for financial risk detection scenarios.

---
