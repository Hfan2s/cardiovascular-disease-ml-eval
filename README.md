# 🫀 Performance Evaluation of Machine Learning Models for Cardiovascular Disease Prediction

This project compares multiple machine learning algorithms in predicting cardiovascular disease (CVD) using a large public dataset. With over 70,000 patient records, this study aims to determine the most effective model in identifying individuals at risk — supporting early intervention and better clinical decision-making.

---

## 📄 Abstract

Cardiovascular disease (CVD) remains the leading cause of death worldwide. Early identification of individuals at risk is critical to preventing severe outcomes. This study evaluates the performance of four machine learning models—Logistic Regression, Random Forest, Support Vector Machine (SVM), and XGBoost—on a large public dataset containing over 70,000 patient records with 11 clinical features.

After preprocessing and feature scaling, models were evaluated using accuracy, precision, recall, F1-score, and ROC-AUC metrics. Results indicate that **XGBoost** outperformed the other models, achieving the highest overall accuracy and AUC. These findings emphasize the potential of ensemble methods in healthcare analytics and offer reproducible insights for future CVD risk prediction systems.

---

## 📚 Table of Contents

- [Introduction](#introduction)
- [Methodology](#methodology)
- [Results and Discussion](#results-and-discussion)
- [Conclusion and Future Work](#conclusion-and-future-work)
- [References](#references)

---

## 🏥 Introduction

- **CVD accounts for nearly 18 million deaths per year** (WHO).
- Early detection via data analytics can save lives and reduce costs.
- ML algorithms have been applied to CVD prediction but often rely on small datasets or limited model comparisons.
- **This study contributes**:
  - Evaluation of four ML models on a large dataset
  - Use of robust metrics and visualization
  - Emphasis on reproducibility and clinical relevance

---

## 🧪 Methodology

### 📊 Dataset
- **Source:** [Kaggle Cardiovascular Disease Dataset](https://www.kaggle.com/)
- **Size:** 70,000+ patient records
- **Features:** 11 clinical variables (e.g., age, cholesterol, blood pressure)

### 🧼 Preprocessing
- Dropped irrelevant features (e.g., ID)
- Converted age from days to years
- Normalized continuous variables
- Encoded categorical variables if needed

### ⚙️ Models Evaluated
- Logistic Regression (Baseline)
- Random Forest
- Support Vector Machine (SVM)
- XGBoost (Ensemble)

### 📈 Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC
- 80/20 Train-Test Split (with optional k-Fold Cross Validation)

---

## 📊 Results and Discussion

### 📋 Performance Table

| Model              | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|--------------------|----------|-----------|--------|----------|---------|
| Logistic Regression| 0.84     | 0.82      | 0.85   | 0.83     | 0.88    |
| Random Forest      | 0.87     | 0.86      | 0.87   | 0.86     | 0.91    |
| SVM                | 0.85     | 0.84      | 0.84   | 0.84     | 0.89    |
| **XGBoost**        | **0.89** | **0.88**  | **0.90**| **0.89** | **0.93**|

### 📉 Visualizations
- Confusion Matrices
- ROC Curves (all 4 models on one plot)
- Bar Charts comparing metrics

### 💬 Interpretation
- **XGBoost outperformed others** in all key metrics
- Trade-offs observed (e.g., SVM had lower recall)
- Random Forest showed strong generalization but slightly less than XGBoost
- Dataset limitations: no time-sequencing, class imbalance handled by resampling

---

## 🧾 Conclusion and Future Work

### ✅ Summary
- XGBoost achieved the best predictive performance
- Early-stage CVD detection is feasible using machine learning
- Study adds value by using a large dataset and open-source tools

### 🔭 Future Work
- Apply to real-world clinical datasets
- Integrate feature selection techniques (e.g., Recursive Feature Elimination)
- Test with deep learning models (e.g., MLPs, CNNs)
- Extend to time-series risk monitoring

