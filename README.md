# Credit Card Fraud Analysis
### Fraud analysis on the ULB credit card dataset, from exploratory SQL to ML models and cost-based thresholds — evaluated on business metrics, not just AUC.

---

## What This Repo Does

End-to-end analysis of credit card fraud detection using the ULB dataset. The pipeline 
covers exploratory analysis, SQL-based fraud pattern exploration, feature engineering, 
supervised modeling with interpretability tools, and cost-based decision rules.

The core focus is on evaluating fraud detection with metrics that matter for the 
business (precision-recall, cost of false negatives) rather than raw accuracy or AUC 
alone.

---

## Repository Structure

    credit-card-fraud-analysis/
    ├── README.md
    ├── requirements.txt
    ├── notebooks/
    │   ├── 01_eda.ipynb                    
    │   ├── 02_sql_analysis.ipynb           (planned)
    │   ├── 03_feature_engineering.ipynb    (planned)
    │   ├── 04_modeling.ipynb               (planned)
    │   └── 05_rules_and_monitoring.ipynb   (planned)
    ├── sql/                                (planned)
    └── data/                               (not tracked in git)

---

## Installation

    git clone https://github.com/TDA-Gabo/credit-card-fraud-analysis.git
    cd credit-card-fraud-analysis
    pip install -r requirements.txt

Download the dataset from Kaggle: [Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) and place creditcard.csv in data/.

---

## Roadmap

- [x] Notebook 01: EDA — dataset structure, class imbalance, PCA-anonymized features
- [ ] Notebook 02: SQL analysis — fraud patterns via SQL queries
- [ ] Notebook 03: Feature engineering — temporal features, transaction aggregates
- [ ] Notebook 04: Modeling — logistic baseline, XGBoost, SHAP interpretability
- [ ] Notebook 05: Decision rules & monitoring — cost-based thresholds, drift monitoring

---

## Dataset

ULB Credit Card Fraud Detection dataset: 284,807 European card transactions from September 2013, 492 fraudulent (0.172%). Features V1-V28 are PCA-transformed to preserve confidentiality; Time and Amount are unmodified.

---

## References

Card testing patterns and typical amounts:

- Fraudlogix, *Card Testing: How to Detect & Prevent It* — [fraudlogix.com/glossary/what-is-card-testing-and-how-to-prevent-it/](https://fraudlogix.com/glossary/what-is-card-testing-and-how-to-prevent-it/)
- Checkout.com, *What is card testing fraud and how to protect your business* — [checkout.com/blog/card-testing-fraud](https://www.checkout.com/blog/card-testing-fraud)

Dataset:

- Machine Learning Group, Université Libre de Bruxelles (ULB), *Credit Card Fraud Detection* — [kaggle.com/datasets/mlg-ulb/creditcardfraud](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

---

## Author

**TDA-Gabo**
