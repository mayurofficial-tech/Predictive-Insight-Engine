# 🏠 Predictive Insight Engine

**Supervised Learning for House Price Prediction — Regression, Model Evaluation & Gradient Descent from Scratch**

A end-to-end regression project built as a Junior Data Scientist working for a real estate analytics firm: predict house prices from property features, compare model families, and explain *why* one model outperforms another.

📹 **[Watch the video walkthrough](https://drive.google.com/file/d/1g7JMIvaslyv5zHR1pPWz3B6KY2qL4Px7/view?usp=drive_link)**

---

## 📌 Overview

| | |
|---|---|
| **Task** | Predict `house_price_inr` from property features |
| **Dataset** | 4,200 rows · 12 columns (`RealEstate_HousePrice_Dataset_4200.xlsx`) |
| **Models** | Simple Linear Regression · Multiple Linear Regression · Polynomial Regression (degree 2) |
| **Optimization** | Batch Gradient Descent · Stochastic Gradient Descent · Mini-Batch Gradient Descent (implemented from scratch) |
| **Best Result** | Polynomial Regression — **R² = 0.966**, RMSE ≈ ₹2.27M |

---

## 🎯 Objective

Understand, implement, and evaluate supervised regression algorithms — from a single-feature baseline through multiple and polynomial regression — while reasoning about **bias–variance trade-off**, **overfitting/underfitting**, and how **gradient descent** optimizes a model's parameters under the hood.

---

## 🗂️ Repository Structure

```
Predictive-Insight-Engine/
├── Predictive_Insight_Engine.ipynb   # Main notebook — Parts A to I
├── Part_A_Conceptual_Understanding.pdf   # Theory answers (Part A)
├── Dataset/
│   └── RealEstate_HousePrice_Dataset_4200.xlsx
├── screenshots/
│   └── ...                            # Notebook run screenshots
└── README.md
```

---

## 🧠 Project Breakdown

| Part | Topic |
|---|---|
| **A** | Conceptual Understanding — supervised learning, regression vs. classification, bias–variance, over/underfitting |
| **B** | Dataset Understanding & Preparation — EDA, feature identification, train/test split |
| **C** | Simple Linear Regression + assumption validation (residual analysis) |
| **D** | Model Evaluation Metrics — MAE, MSE, RMSE, R², Adjusted R² |
| **E** | Multiple Linear Regression |
| **F** | Polynomial Regression (degree 2) |
| **G** | Gradient Descent — Batch, Stochastic, and Mini-Batch, implemented from scratch |
| **H** | Bias–Variance & Model Diagnostics (train vs. test error gap) |
| **I** | Final Analysis, Business Interpretation & Reporting |

---

## 📊 Results Summary

| Model | MAE (₹) | RMSE (₹) | R² Score | Adjusted R² |
|---|---:|---:|---:|---:|
| Simple Linear Regression | 6,294,594 | 8,184,697 | 0.563 | 0.563 |
| Multiple Linear Regression | 2,604,991 | 3,548,650 | 0.918 | 0.929 |
| Polynomial Regression (deg. 2) | 1,656,923 | 2,267,045 | 0.966 | 0.978 |

**Key takeaway:** price cannot be reliably estimated from area alone — adding relevant features (location, age, distance to city, lot size, etc.) drives the largest jump in accuracy, and controlled polynomial complexity adds a further, smaller gain without discarding interpretability.

---

## ⚙️ Tech Stack

- **Python 3**
- `pandas`, `numpy` — data handling
- `matplotlib`, `seaborn` — visualization
- `scikit-learn` — `LinearRegression`, `PolynomialFeatures`, `StandardScaler`, evaluation metrics
- `scipy.stats` — residual normality checks (Q-Q plot)
- Gradient Descent (Batch / SGD / Mini-Batch) — implemented from scratch in NumPy

---

## ▶️ How to Run

```bash
# 1. Clone the repository
git clone https://github.com/<your-username>/Predictive-Insight-Engine.git
cd Predictive-Insight-Engine

# 2. Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn scipy openpyxl jupyter

# 3. Launch the notebook
jupyter notebook Predictive_Insight_Engine.ipynb
```

Run all cells top to bottom (**Kernel → Restart & Run All**) to reproduce every result, plot, and metric.

---

## 🧾 Conclusion

Polynomial Regression achieved the strongest test performance, but the bias–variance analysis (Part H) checks its train/test error gap before declaring it the production choice over Multiple Linear Regression — since a model that generalizes predictably matters more in practice than a marginally higher R². Full reasoning, plots, and the final write-up are in **Part I** of the notebook.

---

## ✍️ Author

Built as part of the **Predictive Insight Engine** project — Supervised Learning track.

**BRING ON YOUR CODING ATTITUDE** 🚀
