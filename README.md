

---

# 📘 **Customer Churn Prediction Notebook**

This repository contains a **Jupyter Notebook** project that builds a **Customer Churn Prediction System** using the **Telco Customer Churn Dataset**. The focus is on visual exploration, explainability, and comparison of baseline vs production-grade ML pipelines.

---

## 📂 **Project Notebook**

**Notebook file:**

```
Customer_Churn_Prediction.ipynb
```

The notebook walks through the entire lifecycle of the churn prediction workflow.

---

## 🎯 **Goal of the Project**

Churn prediction helps telecom & subscription businesses:

* Identify customers likely to churn
* Reduce revenue loss
* Improve customer retention
* Optimize customer lifetime value (CLV)

This notebook demonstrates how churn can be modeled using real-world ML techniques.

---

## 🧰 **Dataset Used**

Dataset: **Telco Customer Churn (IBM)**
Target column: **Churn (Yes/No)**

Core feature domains:

* **Customer Demographics**
* **Service Subscriptions**
* **Contract & Billing Details**
* **Monthly/Total Charges**
* **Tenure**

---

## 🔍 **Exploratory Data Analysis (EDA)**

The notebook includes visual analysis:

✔ Churn class imbalance
✔ Tenure distribution + churn relationship
✔ Monthly charges vs churn
✔ Contract patterns
✔ Paperless billing analysis

Goal: understand **drivers of churn** before modeling.

---

## 🧪 **Modeling Approach**

The project uses a **two-phase training strategy**:

### **Phase 1 — Baseline Model**

* Logistic Regression
* No scaling
* No encoding pipelines
* No imbalance handling

Purpose: establish a benchmark

---

### **Phase 2 — Professional Model**

Improved pipeline including:

✔ One-Hot Encoding (Categorical)
✔ Standard Scaling (Numerical)
✔ Class imbalance handled via **SMOTE**
✔ Model used: **XGBoost**

This reflects real industry churn modeling workflows.

---

## 📊 **Evaluation Metrics**

Models compared using:

* **Accuracy**
* **Precision**
* **Recall**
* **F1 Score**

Output plots include:

📈 **Side-by-side performance comparison**
🧠 **Feature Importance (XGBoost)**
📉 **Confusion Matrix**
📑 **Classification Report**

---

## 🧠 **Key Business Insights**

From feature importance:

* **Month-to-Month contracts** show highest churn
* **Paperless Billing customers** churn more often
* **Tech support reduces churn**
* **Short-tenure customers** have high churn risk
* **Higher Monthly Charges** correlates with churn

These insights can drive retention strategies.

---

## 🛠 **Tech Stack**

**Notebook environment:**
✔ Jupyter / VS Code / Colab

**Libraries used:**

```
pandas
numpy
matplotlib
seaborn
scikit-learn
imbalanced-learn
xgboost
```

---

## 🚀 **How to Run the Notebook**

1️⃣ Clone or download this repo
2️⃣ Install dependencies:

```
pip install -r requirements.txt
```

3️⃣ Open the notebook:

```
jupyter notebook Customer_Churn_Prediction.ipynb
```

(or open directly in **VS Code** using Jupyter extension)

---

## 🏁 **Results Summary**

The professional pipeline improved performance, especially on **Recall**, which is critical for churn use cases (better to identify churn-risk customers even at slight precision cost).

---

