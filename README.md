# 📉 Telco Customer Churn Prediction

### 📌 Project Overview
Customer retention is critical for the telecommunications industry. This project utilizes **Machine Learning (Random Forest)** to predict customer churn and identify key drivers of attrition. 

**Goal:** Identify high-risk customers and provide strategic recommendations to improve retention.

---

### 🛠️ Tech Stack
* **Language:** R (v4.x)
* **Libraries:** `tidyverse`, `caret`, `randomForest`, `corrplot`
* **Model:** Random Forest Classifier (100 Trees)

---

### 📊 Key Insights & Visualizations

#### 1. Contract Type is the #1 Driver of Churn
Customers on **Month-to-Month contracts** (Red) are significantly more likely to leave than those on 1-year or 2-year contracts.
![Contract Chart](graph_contract.png)

#### 2. Feature Importance (Why are they leaving?)
Using the Random Forest algorithm, we identified that **Contract**, **Tenure**, and **Total Charges** are the most important predictors.
![Feature Importance](graph_feature_imp.png)

---

### 🧠 Model Performance
The model was trained on 75% of the data and tested on a 25% hold-out set.

* **Accuracy:** 78.6%
* **Sensitivity:** 0.88 (High ability to detect loyal customers)
* **Specificity:** 0.51 (Moderate ability to detect churners)

![Confusion Matrix](confusion_matrix.png)

---

### 📂 How to Run
1.  Clone the repo.
2.  Open `churn_analysis.R` in RStudio.
3.  Ensure `churn_data.csv` is in the working directory.
4.  Run the script to reproduce the analysis.
