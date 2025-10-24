# 🩺 Liver Disease Prediction Project

A Machine Learning project aimed at predicting the presence of liver disease using the **Indian Liver Patient Dataset**.  
The project involves data preprocessing, exploratory data analysis, model comparison, and hyperparameter tuning to identify the best-performing model.

---

## 📘 Summary

### Data Analysis Key Findings

- The project aims to predict liver disease using the Indian Liver Patient Dataset.  
- The dataset contains 11 attributes, including demographic and clinical features, and a target variable (`Selector`) indicating the presence (1) or absence (0) of liver disease.  
- Missing values were found only in the **A/G Ratio** column and were handled by dropping the 4 rows with missing data.  
- Initial model evaluation showed that **Random Forest** and **Gradient Boosting** (with adjusted class weights) achieved the highest accuracy of around **76%**.  
- Hyperparameter tuning was performed using **GridSearchCV** and **Optuna** for Random Forest and XGBoost models.  
- After tuning, the **XGBoost model optimized with GridSearchCV (for f1_macro)** demonstrated improved balanced performance across both classes, making it the preferred model.

---

### 🔍 Insights and Next Steps

- The class imbalance in the dataset was handled through class weights and evaluated using the **F1-macro** score for better reliability across both classes.  
- Future improvements could involve **oversampling**, **undersampling**, or **synthetic data generation (SMOTE)** to further improve minority class prediction.  
- Further exploration can include ensemble stacking or neural network models for performance enhancement.

---

## 📊 Data Description

The dataset includes medical and demographic information of patients, labeled according to the presence or absence of liver disease.

| Feature | Description |
|----------|-------------|
| Age | Age of the patient |
| Gender | Gender of the patient (Male or Female) |
| TB (Total Bilirubin) | Total Bilirubin level in the blood |
| DB (Direct Bilirubin) | Direct Bilirubin level in the blood |
| Alkphos (Alkaline Phosphatase) | Alkaline Phosphatase level in the blood |
| Sgpt (Alamine Aminotransferase) | SGPT level in the blood |
| Sgot (Aspartate Aminotransferase) | SGOT level in the blood |
| TP (Total Proteins) | Total Proteins level in the blood |
| ALB (Albumin) | Albumin level in the blood |
| A/G Ratio (Albumin and Globulin Ratio) | Ratio of Albumin to Globulin |
| Selector | Class label — 1 for liver disease, 0 for no liver disease |

**Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/ILPD+(Indian+Liver+Patient+Dataset))

---

## ⚙️ Tools and Technologies

- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- XGBoost, Random Forest, Gradient Boosting  
- GridSearchCV, Optuna  

---

## 🧑‍💻 Author

**Upanya Chennoju**
Project: Liver Disease Prediction using Machine Learning  
Dataset: Indian Liver Patient Dataset (UCI Repository)

---

## 📜 License

This project is open-source and available under the MIT License.
