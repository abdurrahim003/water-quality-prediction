# Water Quality Prediction Using Machine Learning

## Overview
This project develops machine learning models to classify water samples as **safe** or **unsafe** for drinking based on physicochemical parameters, guided by WHO drinking water guidelines. Accurate water quality prediction is essential for public health and environmental monitoring.

## Dataset
- **Name:** Water Quality Prediction Dataset
- **Source:** [Kaggle](https://www.kaggle.com/datasets)
- **Size:** 2,000 water samples (1,797 after cleaning)
- **Features:** 6 physicochemical parameters
- **Target:** Binary classification (Safe vs Unsafe)

## Models and Results

| Model | Accuracy | Precision (macro) | Recall (macro) | F1-Score (macro) |
|-------|----------|-------------------|----------------|------------------|
| Logistic Regression | 84.7% | 0.73 | 0.63 | 0.65 |
| **Random Forest** | **99.2%** | **1.00** | **0.98** | **0.98** |
| Gradient Boosting | 100.0% | 1.00 | 1.00 | 1.00 |

**Best Model:** Random Forest (99.2% accuracy, AUC = 1.00)

**Cross-Validation:** 5-Fold Mean Accuracy = 99.1% ± 0.84%

## Feature Importance (Random Forest)
1. pH — 0.3907
2. Turbidity (NTU) — 0.3833
3. Dissolved Oxygen (mg/L) — 0.1209
4. Temperature (°C) — 0.0496
5. TDS (mg/L) — 0.0294
6. Conductivity — 0.0261

## Key Findings
- **pH** and **Turbidity** together account for ~77% of prediction importance
- Dissolved Oxygen is the third most important parameter (12.1%)
- Non-linear models (Random Forest, Gradient Boosting) vastly outperform Logistic Regression
- The model can reliably classify water samples for potability screening

## Tools Used
- **Language:** Python
- **Libraries:** pandas, NumPy, Matplotlib, Seaborn, scikit-learn
- **Platform:** Kaggle Notebooks

## Kaggle Notebook
[View the full notebook on Kaggle](https://www.kaggle.com/abdurrahim003)

## Author
**Abdur Rahim**
B.Sc. in Chemistry, Gopalganj Science and Technology University (GSTU), Bangladesh

- Kaggle: [abdurrahim003](https://www.kaggle.com/abdurrahim003)
- GitHub: [abdurrahim003](https://github.com/abdurrahim003)
