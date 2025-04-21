Here’s a complete and well-structured `README.md` file for your **Life Expectancy Prediction** project on GitHub:

---

# 🌍 Life Expectancy Prediction

This repository presents a machine learning project focused on predicting **life expectancy** using a regression-based approach. The entire analysis, from data exploration to model optimization, is performed in a Jupyter Notebook: `Life_Expectancy.ipynb`.

---

## 🧠 Project Overview

The goal is to predict life expectancy based on several socio-economic and health-related indicators. The project includes:

- Data loading and preprocessing  
- Correlation analysis and visualization  
- Regression model development and evaluation  
- Feature selection and model optimization

---

## 📁 Dataset

The dataset (not included in this repo) should be placed at:

```
/content/drive/MyDrive/AI-Assignment1/
```

> 🔹 Source: External dataset  
> 🔹 Accessed via Google Drive in the notebook  

### 🧬 Key Features

- `alcohol`: Alcohol consumption  
- `polio`: Polio immunization coverage  
- `thinness 1-19 years`, `thinness 5-9 years`: Malnutrition indicators  
- `income composition of resources`: Economic development index  
- `life expectancy`: 🎯 **Target variable**

---

## ✅ Tasks Performed

### 1. Data Loading & Exploration
- Loaded CSV from Google Drive  
- Checked dimensions, data types, and missing values  

### 2. Data Preprocessing
- Handled missing data  
- Standardized and cleaned column names  

### 3. Correlation Analysis
- Created a correlation heatmap  
- Found strong negative correlation between `adult mortality` and `life expectancy` (−0.70)

### 4. Model Building
- Developed and trained two models:
  - Linear Regression
  - Random Forest Regression
- Split data: **80% training / 20% testing**

### 5. Model Evaluation

| Model                | MSE   | R² Score |
|----------------------|-------|----------|
| Linear Regression     | 38.98 | 0.55     |
| Random Forest         | 7.90  | 0.91     |

### 6. Hyperparameter Tuning
- Used **GridSearchCV** to fine-tune:
  - `n_estimators = 100`
  - `max_depth = 30`

### 7. Feature Selection
- Applied **Recursive Feature Elimination (RFE)**  
- Top 5 predictors:
  - `alcohol`
  - `polio`
  - `thinness 1-19 years`
  - `thinness 5-9 years`
  - `income composition of resources`

### 8. Final Model
- Re-trained both models on selected features  
- **Random Forest** confirmed as the superior model

---

## 📦 Repository Contents

```plaintext
📁 Life-Expectancy-Prediction
│
├── Life_Expectancy.ipynb    # Complete notebook with analysis
├── heatmap_beautiful.png           # Correlation heatmap output
└── README.md                       # Project documentation
```

---

## 📊 Key Findings

- Random Forest Regression significantly outperformed Linear Regression:
  - **MSE**: 7.90 (vs. 38.98)
  - **R²**: 0.91 (vs. 0.55)
- **Cross-validation** and **feature selection** enhanced model performance and reduced overfitting
- Features like `alcohol` and `income composition of resources` are strong predictors of life expectancy

---

## 🛠️ Requirements

- **Python 3.x**
- Required Libraries:
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `seaborn`
  - `scikit-learn`
  - `google.colab`

---

## 🚀 Getting Started

To run this notebook:

1. Upload the dataset to your Google Drive under `/content/drive/MyDrive/AI-Assignment1/`
2. Open `Life_Expectancy.ipynb` in [Google Colab](https://colab.research.google.com/)
3. Execute each cell in order

---

## 👨‍🎓 Author

**Sujan Khatiwoda**  
Assignment – Machine Learning | 2025

---

## 📬 Contact

For queries or suggestions, feel free to open an issue or fork this repository.

---
