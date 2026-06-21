# Wine Quality Prediction | Machine Learning Classification Model

## 📌 Project Overview
A machine learning classification model that predicts red wine quality using chemical properties and advanced ML techniques. This project demonstrates full ML pipeline implementation from data exploration to model deployment.

**Result:** Successfully built and evaluated multiple classification algorithms, achieving robust predictions using XGBoost/LightGBM with class imbalance handling.

---

## 🎯 Objective
Predict wine quality ratings (6-8 scale) based on physicochemical properties using supervised machine learning classification techniques.

---

## 📊 Dataset
- **Source:** UCI Machine Learning Repository (Red Wine Quality Dataset)
- **Size:** 1,599 samples | 11 features
- **Target:** Wine quality (discrete, 6-8 range)
- **Challenge:** Class imbalance in target variable

### Features Used:
- Fixed acidity, volatile acidity, citric acid, residual sugar
- Chlorides, free sulfur dioxide, total sulfur dioxide
- Density, pH, sulphates, alcohol content

---

## 🛠️ Technical Stack
**Languages & Libraries:**
- **Python 3.8+**
- **Data Processing:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn
- **ML Algorithms:** Scikit-learn, XGBoost, LightGBM
- **Data Balancing:** imbalanced-learn (SMOTE)

---

## 🔄 ML Workflow Implemented

### 1. **Data Loading & Exploration**
- Loaded dataset directly from GitHub repository
- Exploratory Data Analysis (EDA) with statistical summaries
- Distribution analysis and correlation assessment

### 2. **Data Preprocessing**
- Handling missing/duplicate values
- Outlier detection and treatment (Z-score method)
- Feature scaling using StandardScaler for algorithm compatibility

### 3. **Class Imbalance Handling**
- Applied **SMOTE** (Synthetic Minority Over-sampling Technique)
- Balanced training dataset to prevent model bias toward majority class
- Improved model generalization on minority classes

### 4. **Feature Engineering & Selection**
- Statistical correlation analysis
- Feature importance evaluation
- Train-test split (80-20 ratio)

### 5. **Model Development - Multiple Algorithms**
Trained and evaluated:
- ✅ Logistic Regression
- ✅ Support Vector Machine (SVM)
- ✅ Decision Tree Classifier
- ✅ Random Forest Classifier
- ✅ Extra Trees Classifier
- ✅ K-Nearest Neighbors (KNN)
- ✅ **XGBoost** (Gradient Boosting)
- ✅ **LightGBM** (Light Gradient Boosting)

### 6. **Hyperparameter Tuning**
- GridSearchCV for optimal parameter selection
- Cross-validation scoring
- Model comparison and benchmarking

### 7. **Model Evaluation**
- **Metrics:** Accuracy, Precision, Recall, F1-Score, ROI
- **Confusion Matrix:** Visualized prediction accuracy vs. misclassifications
- **Classification Report:** Detailed per-class performance

### 8. **Model Persistence**
- Serialized final best model using **joblib**
- Saved as `winekeep.pkl` for production deployment

---

## 📈 Key Results
- Successfully handled imbalanced dataset using SMOTE
- Tested 8+ classification algorithms
- Optimized hyperparameters via GridSearchCV
- Generated confusion matrix for error analysis
- Saved deployable model artifact

---

## 💡 Skills Demonstrated
✅ Machine Learning Pipeline Design  
✅ Classification Modeling  
✅ Class Imbalance Handling (SMOTE)  
✅ Hyperparameter Optimization  
✅ Model Evaluation & Selection  
✅ Data Preprocessing & Scaling  
✅ Algorithm Comparison  
✅ Python Data Science Stack  
✅ Model Serialization & Deployment  

---

## 🚀 How to Use This Project

```python
# Load the trained model
import joblib

model = joblib.load('winekeep.pkl')

# Make predictions on new wine samples
predictions = model.predict(X_new)
```

---

## 📁 Project Structure
```
WineQuality_Prediction/
├── winekeep_new_file.ipynb     # Full Jupyter notebook with all code
├── winekeep.pkl                 # Serialized trained model
└── README.md                    # This file
```

---

## 🔮 Future Enhancements
- API deployment (Flask/FastAPI) for real-time predictions
- Feature engineering with domain expertise (wine chemistry)
- Ensemble methods combining multiple best models
- Cross-validation for robust performance metrics
- Model explanation (SHAP, LIME) for interpretability

---

## 📌 Key Takeaways
This project showcases:
1. **End-to-end ML workflow** from raw data to deployable model
2. **Handling real-world challenges** (class imbalance)
3. **Algorithm selection & optimization** best practices
4. **Production-ready code** with model persistence
5. **Professional data science workflow** using industry-standard tools

---

## 👨‍💻 Author
**Yashvi** | Data Analyst & AI Specialist  
*Building data-driven solutions with Python, ML, and Data Visualization*

---

## 📚 References
- UCI Machine Learning Repository
- Scikit-learn Documentation
- XGBoost & LightGBM Official Docs
- SMOTE Research Paper (Chawla et al., 2002)

---

**Last Updated:** June 2026  
**Status:** ✅ Complete & Deployable
