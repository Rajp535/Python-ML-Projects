# 💻 Laptop Price Prediction

## 📌 Objective
To predict laptop prices based on specifications such as company, processor, screen resolution, RAM, GPU, and operating system using machine learning models. The goal is to build a model useful for online retail, resale, and price comparison applications.

## 📊 Dataset
- **Source:** Local file – `laptop_data.csv`
- **Features:**
  - `Company`, `TypeName`, `Inches`, `ScreenResolution`, `Cpu`, `Ram`, `Memory`, `Gpu`, `OpSys`, `Weight`
- **Target:** 
  - `Price`

## 🧠 Techniques Used
- Data Cleaning (unit removal, datatype conversion)
- Handling Outliers (IQR method for `Inches`, `Ram`, `Weight`)
- Encoding Categorical Variables (One-Hot Encoding)
- Feature Scaling (MinMaxScaler)
- Train-Test Split (80-20 split)
- Model Building:
  - Decision Tree Regressor
  - Random Forest Regressor
  - Gradient Boosting Regressor
  - Ridge Regression (for regularization)
- Hyperparameter Tuning using RandomizedSearchCV
- Model Evaluation using MSE, MAE, R² Score
- Model Serialization using Pickle

## 📈 Model Performances
| Model | Train R² Score | Test R² Score |
|:------|:--------------:|:-------------:|
| Decision Tree Regressor | 79.43% | 72.49% |
| Random Forest Regressor | 84.54% | 80.18% |
| Gradient Boosting Regressor | 94.61% | 85.92% |
| Ridge Regression | 91.35% | 92.65% |

## 🔍 Key Insights
- Gradient Boosting Regressor achieved the best performance on the test set.
- Ridge Regression performed surprisingly well and avoided overfitting.
- Important features influencing price: company brand, CPU model, RAM size, GPU, screen resolution.

## 📁 Files
- `Laptop Price Prediction.ipynb` – Full notebook for EDA, preprocessing, modeling, and evaluation.
- `laptop_data.csv` – Dataset used for model development.
- `laptop price model.pkl` – Pickle file of the best-trained Gradient Boosting model.

## ✅ Outcome
Developed a powerful price prediction model achieving around **86%-93% accuracy** depending on the model, useful for online e-commerce or resale platforms to suggest fair laptop pricing.

---

# 🚀 Project Badges
![Python](https://img.shields.io/badge/Python-3.8-blue.svg)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Project-brightgreen.svg)
![Regression](https://img.shields.io/badge/Regression-Model-orange.svg)
![E-commerce](https://img.shields.io/badge/Domain-E--commerce-blue.svg)

