# 📧 Task 4: Email Spam Detection with Machine Learning

A Python-based machine learning project that classifies emails as **Spam** or **Ham (Not Spam)** using Natural Language Processing (NLP) and multiple ML classifiers.

---

## 📁 Project Structure

```
Task_4_Spam_Detection/
│
├── spam.csv                   # Dataset (5,572 labeled SMS/email messages)
├── spam_detection.ipynb       # Main Jupyter Notebook
└── README.md                  # Project documentation
```

---

## 📌 Problem Statement

Spam mail (junk mail) is sent to massive numbers of users and often contains scams, cryptic messages, or dangerous phishing content. The goal of this project is to build a machine learning model that can automatically detect and classify a message as spam or ham.

---

## 📊 Dataset

- **File:** `spam.csv`
- **Source:** [UCI SMS Spam Collection Dataset](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset)
- **Size:** 5,572 messages
- **Columns:**
  - `v1` → Label (`ham` or `spam`)
  - `v2` → Raw message text

| Class | Count | Percentage |
|-------|-------|------------|
| Ham   | 4,825 | ~86.6%     |
| Spam  | 747   | ~13.4%     |

---

## 🛠️ Technologies Used

| Library | Purpose |
|--------|---------|
| `pandas` | Data loading and manipulation |
| `numpy` | Numerical operations |
| `matplotlib` | Data visualization |
| `seaborn` | Statistical plots |
| `scikit-learn` | ML models, TF-IDF, evaluation |
| `re`, `string` | Text preprocessing |

---

## ⚙️ Installation & Setup

### 1. Clone / Download the project
```bash
git clone https://github.com/your-username/spam-detection.git
cd spam-detection
```

### 2. Install dependencies
```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

### 3. Launch Jupyter Notebook
```bash
jupyter notebook spam_detection.ipynb
```

> ✅ Make sure `spam.csv` is in the **same directory** as the notebook before running.

---

## 🔄 Workflow

```
Raw Data (spam.csv)
       ↓
  Data Exploration (EDA)
       ↓
  Text Preprocessing
  (lowercase, remove punctuation/numbers)
       ↓
  TF-IDF Vectorization
  (5000 features, bigrams, stop-words removed)
       ↓
  Train-Test Split (80% / 20%)
       ↓
  Train 3 ML Models
  ┌────────────────────┐
  │  Naive Bayes       │
  │  Logistic Reg.     │
  │  Linear SVM        │
  └────────────────────┘
       ↓
  Evaluate & Compare
       ↓
  Predict on Custom Messages
```

---

## 🤖 Models & Results

| Model | Accuracy |
|-------|----------|
| Naive Bayes | ~97.3% |
| Logistic Regression | ~98.1% |
| Linear SVM | ~98.4% |

> **Best Model:** Linear SVM / Logistic Regression

### Evaluation Metrics used:
- Accuracy
- Precision, Recall, F1-Score
- Confusion Matrix

---

## 📈 Visualizations Included

- Class distribution (bar chart & pie chart)
- Message length distribution by label
- Confusion matrices for all 3 models
- Model accuracy comparison chart
- Top 20 spam & ham indicator words (from LR coefficients)

---

## 🔍 Custom Prediction

You can test the model on your own messages using the built-in function:

```python
predict_spam([
    "Congratulations! You've won a FREE iPhone. Click here to claim!",
    "Hey, are we still on for lunch tomorrow?",
    "URGENT: Your account is compromised. Call now!"
])
```

**Output:**
```
[SPAM 🚫] Congratulations! You've won a FREE iPhone. Click here to claim!
[HAM  ✅] Hey, are we still on for lunch tomorrow?
[SPAM 🚫] URGENT: Your account is compromised. Call now!
```

---

## 💡 Key Findings

- Spam messages are significantly **longer** on average than ham messages
- Top spam indicator words: `free`, `win`, `call`, `prize`, `claim`, `text`, `mobile`
- Top ham indicator words: `ok`, `just`, `will`, `come`, `good`, `know`
- TF-IDF with **bigrams** improves model performance over unigrams alone

---

## 📝 Notes

- The dataset is **imbalanced** (~87% ham), so precision and recall for the spam class are more meaningful metrics than raw accuracy
- `stratify=y` is used during train-test split to preserve class proportions
- All models are trained on cleaned, lowercased, punctuation-free text

---

## 👤 Author

Dyan Shah
Task 4 — Email Spam Detection with Machine Learning