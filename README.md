# Data Science Internship — Oasis Infobyte (AICTE OIB-SIP)

This repository contains all five machine learning projects completed during my **Data Science Internship at Oasis Infobyte**, under the AICTE OIB-SIP program (05/05/2026 – 15/06/2026).

Each project is a complete, self-contained ML workflow — from data exploration to model evaluation — documented with its own notebook and README.

I was recognized as a **Star Performer** for the program and received a Certificate of Completion, Certificate of Appreciation, and Letter of Recommendation.

---

## 📌 About the Internship

**Organization:** [Oasis Infobyte](https://www.oasisinfobyte.com/)
**Program:** AICTE OIB-SIP (Summer Internship Program)
**Domain:** Data Science
**Duration:** 1 month (05/05/2026 – 15/06/2026)
**Intern ID:** OIB/M1/IP149

---

## 🗂️ Projects

| # | Project | Type | Key Techniques |
|---|---------|------|-----------------|
| 1 | [Iris Flower Classification](./Task-1-Iris-Flower-Classification) | Classification | Logistic Regression, Decision Tree, KNN, SVM |
| 2 | [Unemployment Analysis (India)](./Task-2-Unemployment-Analysis) | EDA / Visualization | pandas, matplotlib, seaborn, time-series trends |
| 3 | [Car Price Prediction](./Task-3-Car-Price-Prediction) | Regression | Feature engineering, Random Forest Regressor |
| 4 | [Sales Prediction](./Task-4-Sales-Prediction) | Regression | Multiple Linear Regression, correlation analysis |
| 5 | [Email Spam Detection](./Task-5-Email-Spam-Detection) | NLP / Classification | TF-IDF, Multinomial Naive Bayes, Linear SVM |

---

## 1️⃣ Iris Flower Classification

Built and compared multiple classification models to predict iris species (Setosa, Versicolor, Virginica) from sepal/petal measurements.

- **Dataset:** Classic Iris dataset (150 samples, 4 features)
- **Models used:** Logistic Regression, Decision Tree, K-Nearest Neighbors, SVM
- **Highlights:** Full EDA with pairplots, decision boundary visualization, accuracy comparison across models

---

## 2️⃣ Unemployment Analysis in India

Exploratory data analysis on unemployment rate data across Indian regions, with a focus on trends during the COVID-19 period.

- **Dataset:** Region-wise unemployment rate data (India)
- **Techniques:** Time-series visualization, regional comparison, trend analysis
- **Highlights:** Identified the sharp unemployment spike during COVID-19 and regional disparities through clear visual storytelling

---

## 3️⃣ Car Price Prediction

End-to-end regression pipeline to predict used car selling prices.

- **Dataset:** Used car listings dataset
- **Model:** Random Forest Regressor
- **Feature engineering:** Derived `Car_Age` from manufacture year, encoded categorical features (fuel type, transmission, seller type)
- **Key finding:** Present price emerged as the dominant predictor of selling price
- **Highlights:** Strong R² score, feature importance analysis

---

## 4️⃣ Sales Prediction

Predicted product sales based on advertising spend across TV, radio, and newspaper channels.

- **Dataset:** Advertising spend vs. sales dataset
- **Model:** Multiple Linear Regression
- **Highlights:** Coefficient-based interpretation of channel effectiveness, ~0.90 R² on test data

---

## 5️⃣ Email Spam Detection

NLP-based classifier to detect spam emails from message content.

- **Dataset:** Labeled spam/ham email dataset
- **Pipeline:** Text preprocessing → TF-IDF vectorization → classification
- **Models used:** Multinomial Naive Bayes, Linear SVM
- **Highlights:** ~98% classification accuracy on test data

---

## 🛠️ Tech Stack

- **Language:** Python
- **Libraries:** pandas, NumPy, scikit-learn, matplotlib, seaborn, plotly
- **Tools:** Jupyter Notebook, Git, GitHub

---

## 📁 Repository Structure

```
├── Task-1-Iris-Flower-Classification/
│   ├── iris_classification.ipynb
│   └── README.md
├── Task-2-Unemployment-Analysis/
│   ├── unemployment_analysis.ipynb
│   └── README.md
├── Task-3-Car-Price-Prediction/
│   ├── car_price_prediction.ipynb
│   └── README.md
├── Task-4-Sales-Prediction/
│   ├── sales_prediction.ipynb
│   └── README.md
├── Task-5-Email-Spam-Detection/
│   ├── spam_detection.ipynb
│   └── README.md
└── README.md   ← you are here
```

---

## 🏆 Recognition

- ✅ Certificate of Completion — AICTE OIB-SIP Data Science Internship
- ⭐ Certificate of Appreciation — **Star Performer**
- 📄 Letter of Recommendation

---

## 📫 Connect

**Dhyan Shah**
Data Science Intern, Oasis Infobyte

---

*This repository documents my learning journey through the Oasis Infobyte Data Science internship — built one project, one model, one insight at a time.*