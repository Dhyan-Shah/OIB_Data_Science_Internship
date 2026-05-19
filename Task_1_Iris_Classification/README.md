# 🌸 Iris Flower Classification

A machine learning project to classify Iris flower species — **Setosa**, **Versicolor**, and **Virginica** — based on sepal and petal measurements using Python and Scikit-Learn.

---

## 📁 Project Structure

```
iris-flower-classification/
│
├── Iris.csv                          # Dataset
├── Iris_Flower_Classification.ipynb  # Main Jupyter Notebook
└── README.md                         # Project documentation
```

---

## 📊 Dataset

- **Source:** [Kaggle — Iris Flower Dataset](https://www.kaggle.com/datasets/arshid/iris-flower-dataset)
- **Samples:** 150 (50 per species)
- **Features:** 4 numeric + 1 target

| Feature | Description |
|---|---|
| `SepalLengthCm` | Sepal length in centimetres |
| `SepalWidthCm` | Sepal width in centimetres |
| `PetalLengthCm` | Petal length in centimetres |
| `PetalWidthCm` | Petal width in centimetres |
| `Species` | Target — Iris-setosa / Iris-versicolor / Iris-virginica |

---

## ⚙️ Installation

### Prerequisites
- Python 3.8+
- pip

### Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

---

## 🚀 Usage

### Run the Jupyter Notebook
```bash
jupyter notebook Iris_Flower_Classification.ipynb
```

### Run the Python Script
```bash
python iris_classification.py
```

---

## 🤖 Models Used

| Model | CV Accuracy |
|---|---|
| ⭐ Logistic Regression | **97.33%** |
| K-Nearest Neighbors (KNN) | 97.33% |
| Support Vector Machine (SVM) | 96.67% |
| Random Forest | 96.67% |
| Decision Tree | 95.33% |

> All models evaluated using **5-Fold Cross-Validation**.

---

## 📈 Results

- 🏆 **Best Model:** Logistic Regression (97.33% CV accuracy)
- 🌸 **Iris Setosa** is perfectly separable — 100% precision & recall
- 🔑 **Petal Length** is the most important feature for classification
- ⚠️ **Versicolor vs Virginica** is the most challenging distinction

---

## 📉 Visualizations

The notebook includes:
- Sepal & Petal scatter plots by species
- Box plots for feature distributions
- Correlation heatmap
- Model comparison bar chart
- Confusion matrix
- Feature importance chart (Random Forest)

---

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.x-orange?logo=scikit-learn)
![Pandas](https://img.shields.io/badge/Pandas-2.x-150458?logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.x-11557c)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)

---

## 📄 License

This project is open-source and available under the [MIT License](https://opensource.org/licenses/MIT).