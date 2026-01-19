# 📉 Customer Churn Prediction

## 📌 Project Overview
Customer churn refers to customers discontinuing a service, which directly impacts business revenue and growth.  
This project focuses on predicting customer churn using machine learning techniques to enable proactive customer retention strategies.

The primary objective of this project is to **maximize churn detection (recall)** rather than overall accuracy, aligning with real-world business priorities where missing a churn customer is more costly than false positives.

---

## 🎯 Business Objective
- Identify customers at high risk of churn
- Enable early intervention through targeted retention strategies
- Minimize revenue loss using data-driven decision-making

---

## 📊 Dataset Description
- Dataset contains customer demographics, service usage, contract details, and billing information
- Target variable: **Churn (Yes / No)**
- Feature categories include:
  - Customer tenure and contract type
  - Payment method and billing behavior
  - Service subscriptions and usage patterns

---

## 🔍 Exploratory Data Analysis (EDA)
- Analyzed churn distribution across different customer segments
- Identified key churn drivers such as:
  - Month-to-month contracts
  - Short customer tenure
  - Electronic check payment method
  - Higher monthly charges
- Used visualizations to understand churn behavior across categorical and numerical variables

---

## 🧹 Data Preprocessing
- Handled missing values and inconsistent records
- Encoded categorical variables
- Scaled numerical features
- Ensured proper train–test separation to prevent data leakage

---

## ⚖️ Handling Class Imbalance
- Used **Stratified Train–Test Split** to preserve class distribution
- Applied **SMOTE** only on training data
- Ensured realistic evaluation on unseen test data

---

## 🤖 Model Building
Trained and evaluated multiple classification models:
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- Decision Tree
- Random Forest
- AdaBoost
- Gradient Boosting
- XGBoost

---

## 📈 Model Evaluation
Models were evaluated using business-relevant metrics:
- Recall (primary metric)
- Precision
- F1-score
- ROC-AUC

**AdaBoost** was selected as the final model based on:
- **92% recall for churn customers**
- Strong balance between recall and false positives
- Consistent performance across evaluation metrics

---

## 📊 Results
- Final Model: **AdaBoost**
- Churn Recall: **92%**
- Model effectively identifies high-risk churn customers
- Suitable for deployment in retention-focused business workflows

---

## 💼 Business Interpretation
- High recall ensures most churn-prone customers are detected early
- Enables targeted retention actions such as discounts, offers, or service improvements
- Supports revenue protection by prioritizing proactive intervention

---

## ⚠️ Limitations
- Model performance depends on historical churn patterns
- Does not incorporate real-time behavioral data
- SMOTE may introduce synthetic patterns that may not fully represent real customer behavior

---

## 🛠️ Tech Stack
- Python
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
- imbalanced-learn (SMOTE)

---

## 📁 Project Structure
