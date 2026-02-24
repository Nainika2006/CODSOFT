# 🚢 Titanic Survival Prediction

## 📌 Project Overview

This project focuses on building a Machine Learning classification model to predict whether a passenger survived the Titanic disaster.

The model uses passenger information such as age, gender, ticket class, fare, cabin details, and family relationships to identify patterns that influenced survival.

The prediction output determines:
- Survived
- Not Survived

---

## 🎯 Objective

- Perform Exploratory Data Analysis (EDA)
- Handle missing and inconsistent data
- Visualize survival patterns
- Engineer meaningful features
- Train a classification model
- Evaluate model performance

---

## 📊 Dataset Information

The Titanic dataset contains passenger details including:

- Passenger demographics (Age, Gender)
- Ticket information (Fare, Class, Cabin)
- Family relations (SibSp, Parch)
- Port of embarkation
- Survival status

The dataset includes missing values and mixed data types, making it suitable for real-world preprocessing practice.

---

## 🔎 Exploratory Data Analysis (EDA)

The following visualizations were performed:

- Survival distribution plot
- Gender vs survival comparison
- Passenger class vs survival analysis
- Age distribution boxplots
- Correlation heatmap

### Key Insights:
- Female passengers had significantly higher survival rates.
- First-class passengers were more likely to survive.
- Younger passengers showed higher survival probability.
- Fare and class influenced survival chances.

---

## ⚙️ Data Preprocessing

- Handled missing Age values using median imputation
- Filled Embarked with mode
- Replaced missing Cabin values with "Unknown"
- Encoded categorical variables (Sex, Embarked)
- Created new feature **FamilySize**
- Split dataset into training and testing sets (80/20)

---

## 🤖 Model Used

**Random Forest Classifier**

The model was trained to capture nonlinear relationships and improve prediction accuracy.

---

## 📈 Model Performance

- Accuracy: **82.1%**
- Evaluation Metrics:
  - Confusion Matrix
  - ROC Curve
  - Feature Importance

The model successfully identified gender, passenger class, and fare as the most influential survival factors.

---

## 📊 Visualizations Included

- Survival distribution charts
- Boxplots for Age and Fare
- Confusion Matrix heatmap
- ROC Curve
- Feature Importance chart

These visualizations help interpret both data patterns and model behavior.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

---

## 🚀 Future Improvements

- Try Logistic Regression and XGBoost
- Perform hyperparameter tuning
- Apply cross-validation
- Deploy as a simple prediction web app

---

## 📌 Conclusion

This project demonstrates a complete machine learning workflow including data cleaning, visualization, feature engineering, model training, and evaluation.

It highlights how machine learning can uncover meaningful insights from historical data and make reliable survival predictions.

---

