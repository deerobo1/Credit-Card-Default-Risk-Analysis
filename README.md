# Credit Card Default Risk Analysis 💳📊

## Project Overview
Credit card default prediction is a critical problem in the financial industry, where institutions aim to identify customers who are likely to miss future payments. Accurate prediction helps reduce financial risk while enabling more informed and fair credit decisions.

This project formulates the problem as a **binary classification task**, using customer demographic information and historical payment behavior to predict whether a credit card holder will default in the next billing cycle. The project demonstrates an end-to-end **machine learning workflow**, suitable for an undergraduate-level data science project.

---

## Dataset Description
- The dataset contains anonymized customer-level information related to:
  - Demographics (age, gender, education, marital status)
  - Credit limits
  - Repayment history
  - Bill statement amounts
  - Previous payment amounts
- Target variable:
  - **Default Payment** (`1` = default, `0` = non-default)

> The dataset is used strictly for educational purposes and does not contain personally identifiable information.

---

## Approach & Methodology

### Exploratory Data Analysis (EDA)
- Analyzed class distribution to understand imbalance between defaulters and non-defaulters
- Studied feature distributions and correlations
- Identified repayment-related features with strong predictive signals

### Data Preprocessing
- Encoded categorical variables
- Scaled numerical features where appropriate
- Performed train–test split to prevent data leakage

### Feature Engineering
- Selected relevant financial and repayment features
- Reduced redundancy by removing weakly informative features

### Modeling
- Established a baseline classification model
- Trained additional machine learning models
- Compared model performance using multiple evaluation metrics

---

## Models Used
- **Logistic Regression** (baseline model)
- **Random Forest Classifier** (captures non-linear relationships)

---

## Evaluation Metrics
Due to the **imbalanced nature** of credit default data, multiple metrics were used:
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC score
- Confusion Matrix

These metrics provide a more reliable evaluation than accuracy alone.

---

## Key Insights & Findings
- Repayment history features were among the strongest predictors of default risk
- Customers with frequent delayed payments showed a significantly higher probability of default
- Tree-based models captured complex patterns better than linear baselines
- ROC-AUC proved to be a more informative metric for this problem than accuracy

---

## Limitations & Future Improvements
- Class imbalance impacts recall for the default class
- Limited hyperparameter tuning
- Feature engineering can be further enhanced

**Future improvements include:**
- Hyperparameter tuning using GridSearchCV
- Trying advanced ensemble models (Gradient Boosting, XGBoost)
- Applying class imbalance techniques (SMOTE, class weighting)
- Deploying the model as a simple web application

---

## How to Run the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/credit-card-default-risk-analysis.git
