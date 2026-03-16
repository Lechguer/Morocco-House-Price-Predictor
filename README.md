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


## 🚀 Quick Start



---

## 🌐 Web App


---

## 📚 What You'll Learn


---

## 🛠️ Tech Stack


---

## 📝 Author

**ZIKO** — Data & Software Engineering Student @ INSEA, Rabat  
*Built as part of a supervised machine learning course.*

---
