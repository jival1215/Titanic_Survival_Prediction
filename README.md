# 🚢 Titanic Survival Prediction

## 📌 Overview
This project predicts whether a passenger survived the Titanic disaster based on demographic and travel information.  
It evaluates multiple models using **accuracy** and **cross-validation**, and saves the best model for future predictions.

## 🎯 Objective
- Predict survival (`1 = Survived`, `0 = Died`) using passenger data.
- Compare model performance with cross-validation.
- Save the trained best model.

## 📂 Dataset
- Source: Kaggle Titanic Dataset (or your provided CSV).
- Features include: passenger class, name, sex, age, siblings/spouses aboard, parents/children aboard, fare, cabin, and embarkation port.
- Target: `Survived`.

## 🛠 Tech Stack
- **Language:** Python 3.x
- **Libraries:** pandas, numpy, scikit-learn, matplotlib, joblib
- **Model Types:** Logistic Regression, Random Forest, Gradient Boosting

## 📊 Methodology
1. **Data Cleaning & Feature Engineering**
   - Handle missing values
   - Create `Title` from passenger names
   - Create `FamilySize` and `IsAlone` features
   - Encode categorical variables
2. **Preprocessing Pipeline**
   - Scaling numeric features
   - One-hot encoding categorical features
3. **Model Training**
   - Logistic Regression
   - Random Forest Classifier
   - Gradient Boosting Classifier
4. **Model Evaluation**
   - 5-fold cross-validation accuracy
   - Test set accuracy
   - Confusion Matrix
5. **Model Saving**
   - Save best model as `.pkl` for reuse

## 📈 Results
- **Best Model:** *(Example: Gradient Boosting — update with your result)*
- **Cross-Val Accuracy (mean ± std):** ~0.84 ± 0.03
- **Test Accuracy:** ~0.85
- **Confusion Matrix Example:**
  ```
  [[96, 14],
   [18, 51]]
  ```

## 🚀 How to Run
```bash
pip install -r requirements.txt
python titanic_survival_prediction.py
```

