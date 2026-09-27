# ML Practice Notebooks

A set of beginner machine learning practice notebooks covering classification (heart disease prediction) and regression (house price prediction) using `scikit-learn`.

## 📁 Contents

| File | Task | Techniques Used |
|------|------|------------------|
| `heart disease.ipynb` | Heart disease classification | Logistic Regression, KNN, train/test split, accuracy/precision/recall/F1, confusion matrix heatmap |
| `hearrt.ipynb` | Heart disease classification (extended) | Decision Tree, Random Forest, feature importance, hyperparameter tuning (`max_depth`, `n_estimators`), model comparison (Logistic Regression vs KNN vs Decision Tree vs Random Forest) |
| `houseprices.ipynb` | House price prediction | Linear Regression, missing value handling, MAE/MSE/RMSE/R² evaluation, actual vs predicted scatter plot, feature comparison (3 vs 5 features) |

## 🧠 Overview

### heart disease.ipynb — Heart Disease Prediction (Baseline)
- Loads `heartdisease.csv` and checks class balance.
- Splits data into train/test sets.
- Trains a **Logistic Regression** model and evaluates it with accuracy, precision, recall, and F1-score.
- Visualizes results using a **confusion matrix heatmap** (Seaborn).
- Compares **KNN** performance across different values of `K` (1, 3, 5, 7, 9).

### heart.ipynb — Heart Disease Prediction (Advanced)
- Loads `heartdisease1.csv`.
- Trains a **Decision Tree Classifier** and visualizes the tree structure.
- Tests different `max_depth` values to study overfitting vs underfitting.
- Trains a **Random Forest Classifier** and plots **feature importance**.
- Tunes Random Forest with different `n_estimators` and `max_depth` combinations.
- Compares all four models (Logistic Regression, KNN, Decision Tree, Random Forest) side by side.

### houseprices.ipynb — House Price Prediction
- Loads `houseprices.csv`, explores data with `.info()`, `.describe()`, and null-value checks.
- Handles missing values (`dropna`, `fillna`).
- Trains a **Linear Regression** model using `area`, `bedroom`, `bathroom`, `age`, and `location` as features.
- Evaluates with **MAE, MSE, RMSE, and R²**.
- Plots **Actual vs Predicted price**.
- Compares model performance using 3 features vs 5 features.

## ⚙️ Requirements

```bash
pip install pandas scikit-learn matplotlib seaborn numpy
```

## ▶️ How to Run

1. Clone this repository.
2. Place the required CSV files (`heartdisease.csv`, `heartdisease1.csv`, `houseprices.csv`) in the same folder as the notebooks.
3. Open the notebook with Jupyter:
```bash
   jupyter notebook day7.ipynb
```
4. Run all cells in order (`Cell → Run All`).

## 📌 Notes

- These are learning/practice notebooks — the datasets are small, so accuracy scores may look low or unstable.
