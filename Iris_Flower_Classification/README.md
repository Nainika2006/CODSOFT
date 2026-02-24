
# 🌸 Iris Flower Classification

## 📌 Project Overview

This project focuses on building a Machine Learning classification model using the famous Iris dataset. The objective is to classify iris flowers into their respective species based on sepal and petal measurements.

The model predicts one of the following species:
- Iris Setosa
- Iris Versicolor
- Iris Virginica

---

## 🎯 Objective

- Perform Exploratory Data Analysis (EDA)
- Visualize feature relationships
- Preprocess the dataset
- Train a classification model
- Evaluate model performance

---

## 📊 Dataset Information

The Iris dataset contains:

- 150 samples
- 4 features:
  - Sepal Length (cm)
  - Sepal Width (cm)
  - Petal Length (cm)
  - Petal Width (cm)
- 3 classes (50 samples each)

The dataset is balanced and widely used for introductory classification tasks.

---

## 🔎 Exploratory Data Analysis (EDA)

The following visualizations were performed:

- Pairplot to analyze feature separation
- Correlation heatmap to identify relationships between features
- Boxplots to understand distribution
- Scatter plots for feature comparison

### Key Insights:
- Petal length and petal width are highly correlated.
- Iris Setosa is clearly separable from the other two species.
- Slight overlap exists between Versicolor and Virginica.

---

## ⚙️ Data Preprocessing

- Checked for missing values (none found)
- Split dataset into training and testing sets (80/20)
- Applied feature scaling using StandardScaler

---

## 🤖 Model Used

**Logistic Regression**

The model was trained on the training dataset and evaluated on the test dataset.

---

## 📈 Model Performance

- Accuracy: **96.67%**
- Evaluation Metrics:
  - Precision
  - Recall
  - F1-Score
- Confusion Matrix Visualization

The high accuracy is due to the clean and well-separated nature of the dataset.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## 🚀 Future Improvements

- Compare with Random Forest or SVM
- Perform Cross-Validation
- Deploy using Streamlit
- Create a simple prediction web application

---

## 📌 Conclusion

This project demonstrates the complete workflow of a classification problem:
- Data Exploration
- Data Visualization
- Preprocessing
- Model Training
- Model Evaluation
  
---
