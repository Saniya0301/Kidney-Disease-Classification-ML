# 🩺 Kidney Disease Classification using Machine Learning

## 📌 Overview
This project aims to classify patients as having **Chronic Kidney Disease (CKD)** or **Not CKD** using various medical parameters.  
We use **Exploratory Data Analysis (EDA)**, **data preprocessing**, and multiple machine learning algorithms to build an accurate predictive model.

---

## 📂 Dataset
- **Source**: `kidney_disease.csv`
- **Rows**: 400  
- **Columns**: 25 (medical and demographic features)  
- **Target variable**: `class` (`0` = CKD, `1` = Not CKD)

### Sample Columns:
- Age
- Blood Pressure
- Specific Gravity
- Albumin
- Sugar
- Red Blood Cells
- Pus Cell
- Blood Urea
- Serum Creatinine
- Sodium
- Potassium
- Haemoglobin
- Packed Cell Volume
- White Blood Cell Count
- Red Blood Cell Count
- Hypertension
- Diabetes Mellitus
- Coronary Artery Disease
- Appetite
- Pedal Edema
- Anaemia
- Class

---

## 🛠 Data Preprocessing
1. **Dropped Irrelevant Columns**  
   - Removed `id` column.
   
2. **Renamed Columns**  
   - Converted column names to descriptive, snake_case format.

3. **Handled Inconsistent Data**  
   - Cleaned values like `\tno`, `\tyes` in `diabetes_mellitus` and `coronary_artery_disease`.
   - Standardized target values to `0` (CKD) and `1` (Not CKD).

4. **Data Type Conversion**  
   - Converted numeric columns stored as `object` (e.g., `packed_cell_volume`) to `float`.

5. **Missing Value Handling**  
   - **Numerical**: Random sampling imputation.
   - **Categorical**: Mode imputation.

6. **Encoding Categorical Features**  
   - Label Encoding applied to binary categorical columns.

---

## 📊 Exploratory Data Analysis
- **Univariate Analysis**: Distribution plots for numerical columns, count plots for categorical columns.
- **Correlation Analysis**: Heatmap to identify strong feature relationships.
- **Violin & KDE Plots**: To visualize distribution per class.
- **Scatter Plots**: Feature interactions with respect to the target class.

---

## 🤖 Model Building
- **Features (X)**: All columns except `class`
- **Target (y)**: `class`
- **Algorithms Tested**:
  - Logistic Regression
  - Random Forest
  - XGBoost
  - Support Vector Machine (SVM)
  - K-Nearest Neighbors (KNN)

- **Evaluation Metrics**:
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - Confusion Matrix

---


> Replace `XX` with your actual results.

---
📦 Dependencies

Python 3.x

pandas

numpy

matplotlib

seaborn

plotly

scikit-learn

xgboost


---
🔮 Future Improvements

Hyperparameter tuning for best model performance.

Implement deep learning models for better accuracy.

Deploy model as a web application using Streamlit or Flask.

Add SHAP/feature importance explanations for model interpretability.


---
📜 License

This project is licensed under the MIT License.


---
Author 
SANIYA CHHABRA
