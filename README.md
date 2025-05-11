# 🫀 Heart Disease Prediction using Machine Learning

This project predicts the presence of heart disease based on various clinical parameters using multiple machine learning algorithms. It uses a multivariate dataset with 14 features and converts a multi-class classification problem into a binary classification task for simplicity and higher accuracy.

---

## 📊 Dataset Description

- The dataset consists of **14 features** and a target column `num`.
- Target `num` originally has 5 classes:  
  - 0 = No heart disease  
  - 1 = Mild  
  - 2 = Moderate  
  - 3 = Severe  
  - 4 = Critical

✅ **Binary Classification Conversion**:
- `0` → No Heart Disease  
- `1, 2, 3, 4` → Heart Disease

---

## 🧪 Features

- Age
- Sex
- Chest Pain Type
- Resting Blood Pressure
- Serum Cholesterol
- Fasting Blood Sugar
- Resting ECG Results
- Max Heart Rate Achieved
- Exercise Induced Angina
- Oldpeak (ST Depression)
- Slope of the Peak ST Segment
- Number of Major Vessels
- Thalassemia

---

## 🔧 Data Preprocessing

- **Missing Values**: Imputed using a **Random Forest Regressor** for higher accuracy.
- **Outliers**: Removed using **Z-score method** (`Z > 3` or `Z < -3`).
- **Encoding**: Categorical variables were encoded.
- **Scaling**: StandardScaler used for normalization.

---

## 📈 Models Used

| Model |  Accuracy |
|-------|----------|
| **Random Forest** | **87.0%** ✅ |
| SVM |  87.0% |
| Logistic Regression | 83.2% |
| K-Nearest Neighbors |  84.3% |
| Decision Tree | 80.5% |

**🏆 Best Model**: `RandomForestClassifier(max_depth=10)`  
- Precision: 0.84–0.89  
- Recall: 0.86–0.88  
- F1-score: ~0.87
