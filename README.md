# 🩺 Diabetes Dataset Preprocessing

This repository contains a Jupyter Notebook that demonstrates **data preprocessing techniques** on the [Pima Indians Diabetes Dataset](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database).  
The goal is to prepare the dataset for further **data mining and machine learning** tasks.

---

## 📊 Dataset

- **Original Dataset**: [Pima Indians Diabetes (Kaggle)](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)  
- **Preprocessed Dataset**: Generated after running this notebook. It contains:
  - Missing values handled
  - Outliers removed
  - Age and Glucose binned
  - Normalized (scaled) features

You can use the preprocessed dataset as input for ML models.

---

## ⚙️ Preprocessing Steps

### 1. Handle Missing Data
- Replaced invalid zeros (`0`) in medical columns with `NaN`
- Applied **median imputation** using `SimpleImputer`

### 2. Feature Binning
- **Age** → 4 equal-frequency bins: `Young`, `Adult`, `Middle`, `Senior`  
- **Glucose** → 4 equal-width bins: `Low`, `MedLow`, `MedHigh`, `High`

### 3. Outlier Removal
- Implemented **IQR method** to drop extreme values
- Applied to: `Glucose`, `BloodPressure`, `SkinThickness`, `Insulin`, `BMI`

### 4. Feature Scaling
- Applied **Min-Max Scaling** to normalize numerical features  
- Created additional scaled columns with suffix `_scaled`

---


---

## ▶️ Usage

1. Clone this repository:
   ```bash
   git clone https://github.com/Ravidujee19/diabetes_data_preprocessing.git
   cd diabetes-data-preprocessing
   ```

2. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

3. Open `data_preprocessing.ipynb` and run all cells.

---

## 📈 Results

- Missing values replaced successfully
- Outliers removed
- New binned and scaled features added for downstream ML tasks

---

