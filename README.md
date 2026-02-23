# Mobile Customer Churn Prediction & Fairness Analysis

This repository contains a comprehensive Machine Learning project focused on predicting customer churn for a mobile phone operator. Beyond predictive accuracy, the project places a significant emphasis on **Algorithmic Fairness**, ensuring that the model's decisions are equitable across demographic groups.

## 👥 Authors
* **Luca Betti** (UEVE - M2QF)
* **Ettore Davide Brignoli** (UEVE - M2QF)

---

## 📊 Project Overview
The goal is to provide actionable insights to management by identifying customers at risk of leaving the service. The workflow includes:

1.  **Exploratory Data Analysis (EDA):** Anomaly detection, feature engineering, and data cleaning of the `celldata.csv` dataset.
2.  **Statistical & Machine Learning Modeling:** A comparative study of multiple architectures:
    * **Linear/Quadratic Discriminant Analysis (LDA/QDA)**
    * **Logistic Regression**
    * **Ensemble Methods:** Random Forest, Extra Trees, AdaBoost, Gradient Boosting.
    * **Advanced Boosting:** XGBoost, CatBoost, and LightGBM.
3.  **Fairness Assessment:** Evaluation of model bias using metrics like Independence, Separation, and Sufficiency, specifically focusing on the `Gender` attribute.



## ⚖️ Key Focus: Algorithmic Fairness
A standout feature of this research is the intervention to mitigate bias:
* **The Problem:** Initial models showed a lack of statistical independence, meaning the prediction was influenced by the customer's gender.
* **The Solution:** Implementation of "Fairness through Unawareness" by removing the sensitive attribute.
* **The Result:** We successfully improved the fairness metrics (Independence ratio increased from **0.58** to **0.86**) while maintaining a high **AUC Score of ~0.858**.



## 🛠️ Tech Stack
* **Language:** Python
* **Libraries:** `pandas`, `numpy`, `scikit-learn`, `xgboost`, `catboost`, `lightgbm`, `matplotlib`, `seaborn`.

---

## 📂 Repository Structure
* `Churn.ipynb`: The complete Python workflow, from data loading to model evaluation.
* `Report.pdf`: A detailed technical report explaining the methodology, statistical theory, and final results.
* `celldata.csv`: The dataset containing customer features (Credit Score, Geography, Gender, Age, Balance, etc.).

## 🚀 Getting Started
1. **Clone the repo:**
   ```bash
   git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
