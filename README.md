
# 🚀 Employee Performance Analysis

## 📌 Project Summary
This project addresses critical challenges faced by **INX Future Inc.**, a leading provider of data analytics and automation solutions. The company experienced:
- Declines in employee performance  
- Increased service delivery escalations  
- An 8 percentage point drop in client satisfaction  

This analysis uncovers the key factors behind performance issues and attrition rates to help INX take data-driven actions.

---

## 🎯 Project Scope and Objectives
Our solution focuses on providing a comprehensive analysis of employee performance data to:
- 🔍 Identify indicators of non-performing employees  
- 📊 Deliver actionable insights for management  
- 🛠️ Enable targeted interventions  
- 🌟 Maintain high morale and INX’s employer reputation  

---

## 📋 Project Outline
We addressed two main objectives:
1. **Predicting Employee Attrition** – Who is likely to leave the company?
2. **Predicting Employee Performance Ratings** – Who is likely to perform exceptionally or need support?

We leveraged several machine learning models to analyze behavior, improve workforce management, and enhance performance outcomes.

---

## 📊 Data Preprocessing & EDA

### 🔎 Exploratory Data Analysis (EDA) Highlights
- **Gender Distribution:** 60/40 Male to Female  
- **Education:** Predominantly Life Sciences & Marketing backgrounds  
- **Job Roles:** R&D and Sales are mission-critical  
- **Job Satisfaction:** Generally high, but small dissatisfied segment requires attention  
- **Performance Ratings:** Only 11% rated “Outstanding” – improvement possible  
- **Attrition:** Influenced by job satisfaction, work environment, and education background

### 🧹 Data Cleaning & Processing
- **Encoding:**  
  - Label Encoding for nominal categorical features (e.g., Gender, Department)  
  - Ordinal Encoding for ranked features (e.g., Job Level, Satisfaction)  
- **Outliers:** Removed or replaced with mean/median  
- **Scaling:** Used `StandardScaler` for feature normalization  
- **SMOTE:** Balanced class distribution for attrition prediction

### 🧾 Code Snippets
```python
# Encoding
label_encoder = LabelEncoder()
ordinal_encoder = OrdinalEncoder()

# Scaling
scaler = StandardScaler()
X_train_scaled = scaler.fit_transform(X_train)
X_test_scaled = scaler.transform(X_test)

# SMOTE
smote = SMOTE()
X_train_smote, y_train_smote = smote.fit_resample(X_train_scaled, y_train)
```

---

## 🧠 Model Training and Evaluation

### ✅ Attrition Prediction Models

| Model                | Accuracy | Summary |
|---------------------|----------|---------|
| Logistic Regression | 0.88     | Simple, interpretable, effective for binary classification |
| Neural Network      | 0.71     | Captures complex patterns; requires tuning |
| KNN                 | 0.85     | Non-parametric, sensitive to feature scaling |
| SVC                 | 0.87     | Effective with high-dimensional data |
| **Random Forest**   | **0.94** | Robust, reduces overfitting, best performance |
| XGBoost             | 0.86     | High-performance boosting, handles outliers well |

### ✅ Performance Rating Prediction Models

| Model                | Accuracy | Summary |
|---------------------|----------|---------|
| **LightGBM**        | **0.95** | Fast, scalable, best for large datasets |
| XGBoost             | 0.93     | Robust and efficient |
| Neural Network      | 0.86     | Learns complex relationships |
| Random Forest       | 0.82     | Balanced performance and interpretability |
| KNN                 | 0.78     | Simpler but less accurate |

---

## 💡 Recommendations

- **Attrition Prediction:**  
  - ✅ Use **Random Forest** for robustness and interpretability  
  - ⚙️ Use **XGBoost** for large-scale, performance-sensitive deployments  

- **Performance Rating Prediction:**  
  - ✅ Use **LightGBM** for speed, accuracy, and scalability  
  - ⚙️ Use **XGBoost** when feature interactions are more complex  

---

## ✅ Conclusion

This project equips **INX Future Inc.** with data-driven insights into employee performance and attrition. The deployed models enable:
- 🎯 Targeted interventions  
- 🙌 Improved employee satisfaction  
- 📉 Reduced attrition  
- 📈 Enhanced company-wide performance  

> By leveraging robust models like **Random Forest** and **LightGBM**, INX can ensure continuous monitoring and proactive HR strategies.

---

## 👤 Project Contributor
**Miral Katpara**  
_Data Science & Machine Learning Enthusiast_  


---

## 📂 Tech Stack
- Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)  
- Machine Learning (Logistic Regression, KNN, SVC, Random Forest, XGBoost, LightGBM, Neural Networks)  
- SMOTE for imbalance handling  
- StandardScaler for feature scaling  
- Jupyter Notebook for development

---

## 📌 License
MIT License – feel free to use, modify, and distribute.
