# CSI_WEEK6_MS
# 🧠 Model Evaluation & Hyperparameter Tuning

This project builds and tunes classification models to predict the presence of heart disease using a structured dataset. It walks through preprocessing, model training, evaluation, and hyperparameter tuning using **GridSearchCV**.

📈 Final model performance on validation set (Logistic Regression):
- 🧮 **Accuracy**: *e.g., 84%*  
- 📏 **AUC Score**: *e.g., 0.91*  

---

## 📦 Project Files

| File Name                                          | Description                                       |
| -------------------------------------------------- | ------------------------------------------------- |
| `Model_Evaluation_and_Hyperparameter_Tuning.ipynb` | Main notebook for data prep, modeling, and tuning |
| `heart_disease_model.pkl`                          | Saved trained model (for deployment or reuse)     |
| `README.md`                                        | Project documentation                             |


---

## 🚀 How to Use

1. **Open in Google Colab or Jupyter**  
   Upload the notebook and dataset (extracted or zipped CSV format)

2. **Run all cells** to:
   - Clean and preprocess the dataset
   - Encode features and scale inputs
   - Train multiple classification models
   - Evaluate models with confusion matrix, ROC-AUC
   - Perform hyperparameter tuning with `GridSearchCV`

---

## 🧪 Workflow Overview

### 1. Data Handling
- Dropped irrelevant columns: `id`, `dataset`, `num`
- Removed high-missing-value features: `ca`, `thal`, `slope`
- Missing value handling:
  - Numerical → median
  - Categorical → mode

### 2. Feature Engineering
- One-hot encoding of categorical features
- Train/test split (80/20)
- Feature scaling using `StandardScaler`

### 3. Model Training
- Models: Logistic Regression, Decision Tree (extendable)
- Evaluation metrics:
  - Accuracy
  - Confusion Matrix
  - ROC Curve & AUC Score

### 4. Hyperparameter Tuning
- `GridSearchCV` used to identify best model parameters

---

## 📊 Results

- ROC Curve visualized to compare model performance
- Best model selected based on AUC and accuracy
- GridSearch results reveal optimal hyperparameters
---

## 👤 Author

- **MANIKA SARKAR**  
