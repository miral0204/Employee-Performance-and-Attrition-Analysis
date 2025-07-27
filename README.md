# Employee Performance & Attrition Analysis 📈

## Overview
Training model for attrition prediction:
- Data cleaning, feature encoding, imbalance handling (SMOTE)
- Comparison of Logistic Regression, KNN, SVC, Random Forest, XGBoost

## Key Highlights
- Label vs Ordinal/One‑hot encoding
- Use of Standard Scaler for scaling numeric features
- SMOTE to synthesize minority class
- Model comparison with metrics: Accuracy, Precision, Recall, F1‑score

## Must-know Technical Points
- Why encoding matters and when to choose label vs OHE
- Understanding scaling and model compatibility
- Model strengths: interpretability vs performance vs speed
- Use case scenarios: when to pick logistic regression vs tree models
- Visualization of model performance and feature importance

## FAQ (Interview-ready)
- Why use SMOTE? → To balance minority class while retaining majority class data.
- When is random forest preferred over logistic regression? → For complex patterns and missing data; less scaling needed.
- Why scale inputs for SVC/KNN? → Because they rely on distance metrics.
- What plots were used for EDA? → (Add your notebook visuals: histograms, boxplots, scatter correlation, etc.)

---

### ✅ How to Prepare for Interview:
- Revise each model’s assumptions & pros/cons
- Practice explaining boxplot/IQR, encoding decisions, and SMOTE
- Be ready to justify model selection based on data size, feature types, explainability, and performance

Let me know if you’d like to dive deeper into any specific part!
