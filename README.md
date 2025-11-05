# Optuna Hyperparameter Tuning on Diabetes Dataset

This project demonstrates how to use **Optuna** for hyperparameter tuning on the classic **Diabetes dataset** from scikit-learn.  
The task is a **regression problem**: predicting diabetes progression using patient health features.

## 📊 Model
- **RandomForestRegressor** from scikit-learn
- Tuned hyperparameters: 
  - `n_estimators`
  - `max_depth`

## ⚙️ Workflow
1. Load and split the dataset into train/test sets.
2. Define an Optuna objective function with cross-validation.
3. Optimize hyperparameters using **TPESampler**.
4. Evaluate the best model on the test set using **R² score**.

## 🔍 Results
- **Best cross-validation R²** ≈ 0.41  
- **Test R² with best parameters** ≈ 0.47  
  (This is expected for the diabetes dataset, which is known to be challenging.)

## 🛠️ Tech Stack
- Python
- scikit-learn
- Optuna
- NumPy

---

### 🚀 How to Run
```bash
pip install -r requirements.txt
jupyter notebook "optuna in regression.ipynb"
