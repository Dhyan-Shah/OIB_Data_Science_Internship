# Task 5: Sales Prediction Using Python

## Overview

Sales prediction means predicting how much of a product people will buy based on factors such as the amount spent on advertising. This project uses the **Advertising dataset** to build a **Multiple Linear Regression** model that predicts sales based on TV, Radio, and Newspaper advertising budgets.

---

## Dataset

**File:** `Advertising.csv`

| Column | Description |
|--------|-------------|
| TV | Advertising budget spent on TV (in thousands) |
| Radio | Advertising budget spent on Radio (in thousands) |
| Newspaper | Advertising budget spent on Newspaper (in thousands) |
| Sales | Units of product sold (target variable) |

- **Rows:** 200 records
- **Columns:** 4 (3 features + 1 target)
- **Missing Values:** None

---

## Project Structure

```
Task5_Sales_Prediction/
│
├── Advertising.csv               # Dataset
├── Sales_Prediction_Task5.ipynb  # Main Jupyter Notebook (executed)
└── README.md                     # Project documentation
```

---

## Requirements

Make sure you have Python 3.7+ installed. Install the required libraries using:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

---

## How to Run

1. Clone or download the project folder.
2. Place `Advertising.csv` in the same directory as the notebook.
3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook Sales_Prediction_Task5.ipynb
   ```
4. Run all cells: **Kernel → Restart & Run All**

---

## Notebook Walkthrough

### Step 1 — Import Libraries
Imports NumPy, Pandas, Matplotlib, Seaborn, and Scikit-learn modules.

### Step 2 — Load Dataset
Reads `Advertising.csv` into a Pandas DataFrame and previews the data.

### Step 3 — Exploratory Data Analysis (EDA)
- Dataset shape, data types, and missing value check
- Statistical summary (mean, std, min, max)
- Distribution histograms for all features
- Correlation heatmap
- Pairplot of advertising channels vs Sales

### Step 4 — Feature Selection & Data Splitting
- Features (X): `TV`, `Radio`, `Newspaper`
- Target (y): `Sales`
- Train/Test Split: **80% training / 20% testing** (random_state=42)

### Step 5 — Model Training
Trains a **Multiple Linear Regression** model using Scikit-learn and prints the intercept and coefficients for each feature.

### Step 6 — Model Evaluation
Evaluates the model using:
| Metric | Description |
|--------|-------------|
| MAE | Mean Absolute Error |
| MSE | Mean Squared Error |
| RMSE | Root Mean Squared Error |
| R² Score | Proportion of variance explained |

Also includes:
- Actual vs Predicted scatter plot
- Residual plot
- Distribution of residuals

### Step 7 — Feature Importance
Bar chart of regression coefficients showing which advertising channel has the most influence on Sales.

### Step 8 — Predict on New Data
Demonstrates prediction of Sales for custom advertising budget inputs.

---

## Results

| Metric | Value |
|--------|-------|
| R² Score | ~0.90 |
| RMSE | ~1.65 |
| Best Feature | TV |
| Algorithm | Multiple Linear Regression |

The model explains approximately **90% of the variance** in Sales, indicating a strong fit.

---

## Key Findings

- **TV** advertising has the strongest positive impact on Sales.
- **Radio** also contributes significantly to Sales.
- **Newspaper** has the least impact among the three channels.

---

## Technologies Used

- **Python 3.x**
- **Pandas** — Data manipulation
- **NumPy** — Numerical computations
- **Matplotlib & Seaborn** — Data visualization
- **Scikit-learn** — Machine learning model

---

## Author

Task 5 — Sales Prediction Using Python  
*Internship | Oasis InfoByte | Data_Science