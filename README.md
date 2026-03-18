# 🏠 Morocco House Price Predictor
### Linear Regression — From Scratch · GitHub Portfolio Project

> **Predict house prices in Morocco** using a linear regression model built from scratch with NumPy.  
> A complete end-to-end machine learning project: EDA → OLS theory → implementation → interactive web app.

---

## 🎯 Project Overview

| | |
|---|---|
| **Type** | Supervised Learning — Regression |
| **Algorithm** | Linear Regression (OLS — Ordinary Least Squares) |
| **Dataset** | 500 real-estate properties across 5 Moroccan cities |
| **R² Score** | **0.974** — 97.4% of price variance explained |
| **Stack** | Python · NumPy · Pandas · Scikit-learn · HTML/CSS/JS |

---

## 📁 Project Structure

```
house-price-predictor/
│
├── 📓 notebook/
│   └── linear_regression_housing.ipynb   # Full analysis & model
│
├── 🌐 app/
│   ├── index.html                         # Interactive web predictor
│   └── static/                            # Generated plots
│       ├── eda_prices.png
│       ├── correlation.png
│       ├── evaluation.png
│       └── coefficients.png
│
├── 📊 data/
│   └── morocco_housing.csv               # Dataset (500 samples)
│
├── 🤖 models/
│   ├── model.pkl                          # Trained LinearRegression
│   ├── scaler.pkl                         # StandardScaler
│   └── feature_names.pkl                 # Feature order
│
└── requirements.txt
```

---

## 🧮 The Math — OLS Linear Regression

The model finds coefficients **β** that minimize the **Sum of Squared Residuals**:

$$\hat{y} = \beta_0 + \beta_1 x_1 + \beta_2 x_2 + \cdots + \beta_n x_n$$

**Closed-form solution (Normal Equation):**

$$\hat{\beta} = (X^T X)^{-1} X^T y$$

This project implements this formula **from scratch in NumPy**, then verifies against scikit-learn.

---

## 🏙️ Dataset — Features

| Feature | Type | Description |
|---|---|---|
| `area_m2` | Numerical | Surface area (40–300 m²) |
| `rooms` | Numerical | Number of rooms (1–8) |
| `age_years` | Numerical | Building age (0–50 years) |
| `floor` | Numerical | Floor level (1–15) |
| `distance_center_km` | Numerical | Distance from city center |
| `has_garage` | Binary | Parking garage (0/1) |
| `has_garden` | Binary | Garden (0/1) |
| `city` | Categorical | Casablanca, Rabat, Marrakech, Tanger, Fès |
| `price_mad` | **Target** | Price in Moroccan Dirhams (MAD) |

---

## 📈 Model Performance

| Metric | Value |
|---|---|
| R² (Train) | 0.976 |
| R² (Test) | **0.974** |
| RMSE | ~197,000 MAD |
| MAE | ~152,000 MAD |
| MAPE | ~12% |

---

## 🚀 Quick Start

```bash
# 1. Clone the repo
git clone https://github.com/Lechguer/House_Price_Prediction.git
cd house-price-predictor

# 2. Install dependencies
pip install -r requirements.txt

# 3. Open the notebook
jupyter notebook notebook/Linear_Regression_Housing.ipynb

# 4. Open the web app
open app/index.html    # macOS
# or simply double-click app/index.html
```

---

## 🌐 Web App

The `app/index.html` is a **standalone interactive predictor** — no server needed.  
Just open it in a browser, adjust the sliders, and get instant price estimates.

**Features:**
- 🎛️ Real-time price prediction with sliders
- 📊 Feature impact breakdown (which variables increase/decrease the price)
- 📐 Live OLS equation display
- 📈 EDA & model evaluation charts

---

## 📚 What You'll Learn

This project covers the **full linear regression learning path**:

1. **EDA** — exploring distributions, correlations, outliers
2. **Preprocessing** — StandardScaler, One-Hot Encoding
3. **OLS Theory** — the Normal Equation derivation
4. **From-Scratch Implementation** — NumPy only, no sklearn
5. **Model Evaluation** — R², RMSE, MAE, residual analysis
6. **Hypothesis Testing** — normality (Shapiro-Wilk), homoscedasticity
7. **Deployment** — standalone web app

---

## 🛠️ Tech Stack

```
Python 3.x          → Core language
NumPy               → From-scratch OLS implementation
Pandas              → Data manipulation
Scikit-learn        → Model validation & comparison
Matplotlib/Seaborn  → Visualizations
HTML/CSS/JavaScript → Interactive web app (no framework)
```

---

## 📝 Author

**ZIKO** — Data & Software Engineering Student @ INSEA, Rabat  
*Built as part of a supervised machine learning course.*
