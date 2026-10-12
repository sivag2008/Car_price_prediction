# 🚗 Used Car Price Prediction

Predicts the price of used cars using **Linear Regression**.

---

## 📂 Dataset

**File:** `used_cars.csv`

**Columns:** `brand`, `model`, `model_year`, `milage`, `fuel_type`, `engine`, `transmission`, `ext_col`, `int_col`, `accident`, `clean_title`, `price`

**Target:** `price`

---

## 🧹 Data Preprocessing

- **Cleaning:** Removed `$`, commas and "mi." from `price` and `milage`
- **Missing values:** Filled `fuel_type`, `accident`, `clean_title` with "Unknown"
- **Frequency encoding:** `brand`, `model`, `engine`, `ext_col`, `int_col`
- **One-hot encoding:** `fuel_type`, `transmission`, `accident`, `clean_title`
- **Scaling:** `StandardScaler`

---

## 🤖 Model

- **Algorithm:** Linear Regression
- **Train/Test split:** 80/20 (`random_state=42`)

---

## ▶️ How to Run

1. Install libraries:
```bash
   pip install pandas numpy scikit-learn
```
2. Keep `used_cars.csv` in the same folder
3. Run the notebook / script

---

## 🚀 Future Work

- Extract **horsepower** and **engine size** from `engine`
- Add a **car_age** feature
- Try **Random Forest / XGBoost**

---

## 🛠️ Requirements

`pandas`, `numpy`, `scikit-learn`
