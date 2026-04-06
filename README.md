# SaaS Customer Retention Engine
### Churn Prediction, Segmentation, and Explainability

A business-focused machine learning project that predicts customer churn, segments users by risk, explains churn drivers, and turns model outputs into actionable retention strategies.

## Business Problem

Customer churn is one of the most expensive problems in subscription-based businesses. Predicting churn is not enough. Teams need to know:

- Who is likely to leave
- Why are they at risk
- What action to take next

This project builds an end-to-end retention system to answer those questions.

## What This Project Does

- Predicts churn probability using machine learning
- Segments customers into high, medium, and low risk groups
- Explains the main drivers of churn using SHAP
- Maps each segment to a practical retention action
- Lays the foundation for a recommendation layer using NeuMF

## Why This Project Matters

Most churn projects stop at model accuracy. This one goes further by translating predictions into business decisions.

That makes it useful for:
- Product teams
- Customer success teams
- Growth teams
- SaaS retention strategy

## Dataset

This project uses the Telco Customer Churn dataset.

Typical fields include:
- Customer tenure
- Contract type
- Monthly charges
- Internet service
- Payment method
- Churn label

## Project Workflow

1. Data cleaning and preprocessing
2. Exploratory data analysis
3. Churn prediction modeling
4. Customer risk segmentation
5. Explainability with SHAP
6. Retention action mapping
7. App/dashboard development
8. Future recommendation system integration

## Modeling Approach

### Baseline Models
- Logistic Regression
- Random Forest

### Final Model
- XGBoost

### Evaluation Metrics
- ROC AUC
- Precision
- Recall

## Customer Segmentation Logic

Customers are grouped into:

- High Risk
- Medium Risk
- Low Risk

Example:
- High Risk: churn probability >= 0.60
- Medium Risk: churn probability between 0.30 and 0.59
- Low Risk: churn probability < 0.30

## Explainability

To understand why customers churn, the project uses SHAP to identify the most influential features.

Typical churn drivers:
- Month-to-month contracts
- Short tenure
- High monthly charges

## Business Recommendations

Based on the model output:

- High-risk customers receive immediate retention outreach
- Medium Risk customers enter an engagement campaign
- Low-risk customers are targeted for upsell or long-term retention

## Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Matplotlib
- Seaborn
- Gradio
- GitHub

## Repository Structure

```text
.
├── notebooks/
│   └── telco-churn-eda.ipynb
├── app/
│   └── gradio_app.py
├── data/
│   └── raw/
├── models/
├── visuals/
├── README.md
└── requirements.txt
