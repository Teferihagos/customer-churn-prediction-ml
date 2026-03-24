# Customer Churn Prediction (End-to-End ML Project)

## Project Overview

Customer churn is a major business problem. It is much cheaper to retain existing customers than to acquire new ones.

This project builds a machine learning model to predict which customers are likely to leave (churn), using real customer data. The goal is to help businesses act early and reduce churn.

---

## Business Problem

Can we identify customers who are likely to churn before they leave?

If yes, companies can:

* Offer discounts
* Improve service
* Target high-risk customers

---

## Dataset

IBM Telco Customer Churn Dataset

* ~7,000 customers
* Features:

  * Demographics (age, gender)
  * Account info (tenure, contract type)
  * Services (internet, phone)
  * Billing (monthly charges, payment method)

---

## Project Workflow

1. Data Cleaning
2. Exploratory Data Analysis (EDA)
3. Feature Engineering
4. Model Training
5. Model Evaluation
6. Business Insights

---

## Models Used

* Logistic Regression (baseline)
* Decision Tree
* Random Forest

---

## Model Performance

| Model               | Accuracy | Recall (Churn) | ROC-AUC |
| ------------------- | -------- | -------------- | ------- |
| Logistic Regression | 0.81     | 0.57           | 0.84    |
| Random Forest       | 0.79     | 0.51           | ~0.84   |
| Decision Tree       | 0.72     | 0.48           | 0.65    |

---

## Key Insight (Important)

The model can help businesses identify high-risk customers early, allowing targeted retention strategies that can reduce revenue loss.

---

## Why Logistic Regression Won

* Best balance of performance + interpretability
* Easy to explain to business stakeholders
* Stable results on this dataset

---

## Limitations

* Dataset is imbalanced (fewer churn cases)
* Recall is moderate → some churn customers are missed
* Model trained on public dataset (may not generalize fully)

---

## Visualizations

### Churn Distribution

![Churn](images/churn_distribution.png)

### Monthly Charges vs Churn

![Charges](images/monthly_charges_vs_churn.png)

### Tenure vs Churn

![Tenure](images/tenure_vs_churn.png)

---

## Model Evaluation

### Confusion Matrix (Explain Simply)

* True Positive → correctly predicted churn
* False Negative → missed churn (very important problem)

* ![Confusion Matrix](images/confusion_matrix.png)

### ROC Curve

* Shows how well the model separates churn vs non-churn
* AUC = 0.84 → good performance

![ROC Curve](images/roc_curve.png)

---

## Key Business Insights

* Customers with short tenure churn more
* Month-to-month contracts have highest churn
* Higher monthly charges increase churn risk

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib

---

## Project Structure

customer-churn-prediction-ml/

* notebooks/ → analysis notebook
* images/ → charts
* README.md → project summary

---

## How to Run

Clone the repo:

```bash
git clone https://github.com/your-username/customer-churn-prediction-ml.git
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run notebook:

```bash
notebooks/01_customer_churn_analysis.ipynb
```

---

## Future Improvements

* Handle imbalance using SMOTE or class weighting
* Hyperparameter tuning
* Deploy model (Streamlit / FastAPI)
* Build a real-time prediction pipeline

---

## Author

Teferi Hagos
Machine Learning Engineer | Data Scientist

GitHub: https://github.com/Teferihagos
Kaggle: https://www.kaggle.com/teferihagos

---
