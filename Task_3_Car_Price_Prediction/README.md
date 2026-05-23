# 🚗 Car Price Prediction with Machine Learning

A machine learning project that predicts the selling price of used cars using a **Random Forest Regression** model, based on features like present price, kilometers driven, fuel type, transmission, and car age.

---

## 📁 Project Structure

```
car-price-prediction/
│
├── car_data.csv                  # Dataset
├── car_price_prediction.ipynb    # Jupyter Notebook (main file)
├── car_price_prediction.py       # Python script version
└── README.md                     # Project documentation
```

---

## 📊 Dataset

| Column | Description |
|---|---|
| `Car_Name` | Name of the car |
| `Year` | Year of manufacture |
| `Selling_Price` | Price the owner wants to sell at *(target)* |
| `Present_Price` | Current ex-showroom price (in Lakhs) |
| `Driven_kms` | Total kilometers driven |
| `Fuel_Type` | Petrol / Diesel / CNG |
| `Selling_type` | Dealer / Individual |
| `Transmission` | Manual / Automatic |
| `Owner` | Number of previous owners |

- **Total records:** 301
- **No missing values**

---

## ⚙️ Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/car-price-prediction.git
   cd car-price-prediction
   ```

2. **Install dependencies**
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```

3. **Run the notebook**
   ```bash
   jupyter notebook car_price_prediction.ipynb
   ```

---

## 🧠 Methodology

### Feature Engineering
- Created `Car_Age` from `Year` → `2026 - Year`
- Label-encoded categorical columns: `Fuel_Type`, `Selling_type`, `Transmission`

### Model
- **Algorithm:** Random Forest Regressor
- **Trees:** 100 estimators
- **Train/Test Split:** 80% / 20%
- **Random State:** 42

---

## 📈 Results

| Metric | Value |
|---|---|
| R² Score | **0.9593** |
| Mean Absolute Error | **0.64 Lakhs** |
| RMSE | **~1.1 Lakhs** |

The model explains **~96% of the variance** in used car selling prices.

---

## 🔍 Feature Importance

| Feature | Importance |
|---|---|
| Present Price | 88.45% |
| Car Age | 6.05% |
| Km Driven | 3.50% |
| Transmission | 1.00% |
| Fuel Type | 0.65% |
| Seller Type | 0.35% |
| Owner | 0.01% |

> **Present Price** is by far the strongest predictor of used car selling price.

---

## 🔮 Sample Prediction

```python
new_car = {
    'Present_Price'   : 8.5,    # Lakhs
    'Driven_kms'      : 35000,
    'Fuel_Type'       : 'Petrol',
    'Selling_type'    : 'Dealer',
    'Transmission'    : 'Manual',
    'Owner'           : 0,
    'Car_Age'         : 7       # 2026 - 2019
}
# Predicted Selling Price: ₹5.47 Lakhs
```

---

## 🛠️ Technologies Used

- **Python 3.x**
- **Pandas** — Data manipulation
- **NumPy** — Numerical operations
- **Matplotlib & Seaborn** — Data visualization
- **Scikit-learn** — Machine learning model

---

## 📌 Future Improvements

- Try other models: XGBoost, Gradient Boosting, Linear Regression
- Hyperparameter tuning with GridSearchCV
- Deploy as a web app using Streamlit or Flask
- Add more features like car brand, city, and condition rating

---

## 👤 Author

Your Name  
[GitHub](https://github.com/your-username) · [LinkedIn](https://linkedin.com/in/your-profile)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).