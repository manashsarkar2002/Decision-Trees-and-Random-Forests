# Heart Disease Prediction — Decision Tree & Random Forest

## 📌 Project Overview
This project demonstrates the training and evaluation of **Decision Tree** and **Random Forest** classifiers on the `heart.csv` dataset to predict the presence of heart disease.  
We analyze **overfitting**, control **tree depth**, interpret **feature importances**, and evaluate using **cross-validation**.

---

## 📂 Dataset
- **File**: `heart.csv`
- **Rows**: 1025  
- **Columns**: 14 (13 features + 1 target)
- **Target Variable**: `target`  
  - `0` → No Heart Disease  
  - `1` → Heart Disease

**Features include**:
- Age, sex, chest pain type (`cp`), resting blood pressure (`trestbps`), cholesterol level (`chol`), fasting blood sugar (`fbs`), resting ECG (`restecg`), maximum heart rate (`thalach`), exercise-induced angina (`exang`), ST depression (`oldpeak`), slope of peak exercise (`slope`), number of major vessels (`ca`), and `thal` value.

---

## 🔍 Steps Performed
1. **Train a Decision Tree Classifier**  
   - Visualized the tree structure using `plot_tree` from `sklearn.tree`.
   
2. **Analyze Overfitting & Control Tree Depth**  
   - Compared accuracy of full-depth vs depth-limited (`max_depth=4`) decision trees.
   
3. **Train a Random Forest Classifier**  
   - Compared performance with Decision Tree.
   
4. **Interpret Feature Importances**  
   - Ranked features based on their contribution to predictions.
   
5. **Cross-Validation**  
   - Used `cross_val_score` for robust performance evaluation.

---

## 📊 Model Performance (Example Results)
| Model                  | Train Accuracy | Test Accuracy |
|------------------------|---------------|--------------|
| Decision Tree (Full)   | 1.000          | 0.985        |
| Decision Tree (Depth=4)| 0.883          | 0.800        |
| Random Forest          | 1.000          | 0.983        |

---

## 📦 Requirements
```bash
pip install pandas numpy matplotlib scikit-learn
