# 💳 Credit Card Fraud Detection

## 📌 Project Overview

This project aims to build a Machine Learning model to detect fraudulent credit card transactions. The dataset is highly imbalanced, making fraud detection a challenging real-world classification problem.

The objective is to accurately identify fraudulent transactions while minimizing false negatives.

---

## 🎯 Objective

- Perform Exploratory Data Analysis (EDA)
- Handle extreme class imbalance
- Train a robust classification model
- Evaluate performance using appropriate metrics
- Focus on fraud detection recall and F1-score

---

## 📊 Dataset Information

Dataset used: Credit Card Fraud Detection Dataset (European cardholders)

- Total transactions: 284,807
- Fraud cases: 492 (~0.17%)
- Features:
  - V1 to V28 (PCA transformed features)
  - Time
  - Amount
- Target variable:
  - 0 → Genuine transaction
  - 1 → Fraud transaction

This dataset is highly imbalanced, making accuracy alone an unreliable metric.

---

## 🔎 Exploratory Data Analysis (EDA)

The following visualizations were performed:

- Class distribution plot
- Fraud vs Genuine percentage pie chart
- Transaction amount distribution
- Fraud vs Genuine boxplot comparison
- Correlation heatmap
- Confusion matrix visualization
- Feature importance analysis

### Key Insights:

- Fraud transactions represent less than 0.2% of total data.
- Severe class imbalance required special handling.
- Some PCA components contribute more significantly to fraud detection.

---

## ⚙️ Data Preprocessing

- Scaled `Time` and `Amount` using StandardScaler
- Split data into training and testing sets (80/20)
- Used `stratify=y` to maintain class distribution
- Applied SMOTE (Synthetic Minority Oversampling Technique) to handle imbalance

---

## 🤖 Model Used

**Random Forest Classifier**

Random Forest was chosen because:

- It handles non-linear relationships well
- It performs better on imbalanced datasets
- It improves recall for minority classes

---

## 📈 Model Performance

Test Set Results:

- Accuracy: 99.97%
- Fraud Precision: 94%
- Fraud Recall: 88%
- Fraud F1-Score: 91%

### Confusion Matrix:

- True Negatives: 48,632
- False Positives: 5
- False Negatives: 11
- True Positives: 77

### Interpretation:

The model successfully detected 88% of fraudulent transactions while maintaining a very low false positive rate.

Recall was prioritized to reduce financial loss from missed fraud cases.

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

- Hyperparameter tuning
- Threshold adjustment to improve recall
- Try XGBoost or LightGBM
- Deploy using Streamlit or Flask
- Implement real-time fraud detection simulation

---

## 📌 Conclusion

This project demonstrates handling of real-world challenges such as extreme class imbalance and evaluation beyond accuracy.

The Random Forest model achieved strong fraud detection performance with high precision and recall, making it suitable for financial risk detection scenarios.

---


