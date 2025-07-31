## 🕵️‍♂️ Fraud Detection on Financial Transactions

### 📌 **Overview**

A financial company wants to proactively detect fraudulent transactions using historical data. The objective is to build a machine learning model that can identify fraud and help the company prevent losses. This notebook presents the steps taken to clean data, build and evaluate the model, and provide insights for prevention.

### 🎯 **Objectives**

* Identify patterns in fraudulent behavior using historical transaction data.
* Build a supervised classification model to **predict fraud probability**.
* Address **class imbalance** to ensure reliable predictions.
* Interpret key features contributing to fraud.
* Provide **recommendations** to enhance fraud monitoring systems.

---

### 🔍 **Steps Performed**

1. **Business Understanding**

   * Understand the nature of financial fraud and its impact.
   * Define modeling goals and performance expectations.

2. **Data Exploration & Cleaning**

   * Inspected dataset (6.3M+ rows, 10 columns).
   * Checked for null values, duplicates, and inconsistent formats.
   * Performed type conversions and outlier detection.

3. **Exploratory Data Analysis (EDA)**

   * Visualized class imbalance (fraud vs non-fraud).
   * Analyzed transaction amount distribution, time patterns, and customer behavior.

4. **Feature Engineering**

   * Extracted new features like transaction hour and customer frequency.
   * Derived patterns related to account balance before/after transactions.

5. **Class Imbalance Handling**

   * Applied **SMOTE (Synthetic Minority Over-sampling Technique)** to balance the dataset.

6. **Model Building**

   * Trained a **Random Forest Classifier**.
   * Compared performance with baseline Logistic Regression.

7. **Model Evaluation**

   * Evaluated using **AUC-ROC**, **Recall**, **Precision**, **F1-Score**.
   * Optimized for **recall** to reduce false negatives in fraud detection.

8. **Model Interpretation**

   * Used **feature importance** and **SHAP plots** to explain model behavior.
   * Identified top fraud indicators like transaction amount, type, and balance drops.

9. **Insights & Recommendations**

   * Fraud more likely during unusual hours and with sudden balance shifts.
   * Suggest implementing **real-time alerts**, monitoring **transaction types**, and tightening security for high-value transfers.

---

### 📈 **Results**

* Achieved strong **recall and AUC-ROC**, ensuring effective fraud detection.
* Balanced dataset using SMOTE improved minority class detection.
* Delivered **actionable insights** to improve fraud prevention.


---

### 📬 **Future Work**

* Deploy the model using Flask or Streamlit for real-time fraud detection.
* Integrate with a dashboard (Power BI / Streamlit) for monitoring KPIs.
* Explore time-based models like LSTM for transaction sequences.

---

### 📎 **Disclaimer**

*Due to privacy constraints, the original dataset is not included in this repo.*



 
 
 
