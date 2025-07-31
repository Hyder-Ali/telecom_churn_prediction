# 📞 Telecom Customer Churn Prediction

This project aims to predict whether a telecom customer is likely to churn using machine learning techniques. It includes exploratory data analysis, model building (Logistic Regression and Random Forest), hyperparameter tuning, and final report generation in PowerPoint.

---

## 📊 Problem Statement

Customer churn is a major concern for telecom companies. Identifying customers at risk of leaving enables businesses to take proactive retention measures. This project focuses on predicting churn using historical customer data.

---

## 🧰 Tools & Technologies Used

- Python (Google Colab)
- pandas, numpy, matplotlib, seaborn
- scikit-learn (Logistic Regression, Random Forest, Hyperparameter Tuning)
- joblib (for model saving)
- scikit-learn metrics (confusion matrix, ROC-AUC, classification report)
- python-pptx (PowerPoint generation)

---

## 🧪 Project Workflow

### 1. **Data Preprocessing**
- Loaded mock telecom customer dataset
- Handled missing values and categorical encoding
- Feature selection and scaling

### 2. **Exploratory Data Analysis (EDA)**
- Visualized churn distribution
- Correlation heatmaps and bar plots to identify churn drivers

### 3. **Model Building & Comparison**
- **Logistic Regression** with L1 penalty
- **Random Forest Classifier**
- Hyperparameter tuning using `GridSearchCV`
- Evaluation via:
  - Confusion Matrix
  - Classification Report
  - ROC Curve and AUC

### 4. **Model Performance**
| Metric                | Logistic Regression | Random Forest       |
|----------------------|---------------------|---------------------|
| Accuracy             | 56%                 | 79%                 |
| ROC-AUC Score        | 0.52                | 0.50                |
| Precision (Churn=1)  | 0.16                | 0.15                |
| Recall (Churn=1)     | 0.52                | 0.11                |

✅ **Best Model Selected:** Random Forest (higher overall accuracy)

### 5. **Model Saving**
- Best model saved as `best_model.pkl` using `joblib`.

### 6. **Presentation**
- A PowerPoint file (`churn_presentation.pptx`) summarizing:
  - Objectives
  - Model performance
  - Key churn drivers
  - Recommended business actions

---

## 🔍 Key Insights

- **Churn Rate:** High imbalance in target variable (Churn=1 is rare)
- **Top Drivers:** Contract type, monthly charges, and customer tenure
- **Class Imbalance Challenge:** Performance for churners is low due to imbalance

---

## 💡 Business Recommendations

- Offer incentives to long-term customers
- Encourage switching from month-to-month to long-term contracts
- Target high monthly charge customers with loyalty programs

---
