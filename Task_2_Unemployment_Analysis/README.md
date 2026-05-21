# 📊 Unemployment Analysis in India — Task 2

> Analyzing India's unemployment trends using Python, with a focus on the sharp spike caused by the **Covid-19 pandemic and national lockdown (2020)**.

---

## 📁 Project Structure

```
Unemployment-Analysis/
│
├── Unemployment_Analysis_India.ipynb   # Main Jupyter Notebook
├── Unemployment_in_India.csv           # Dataset 1 – Historical state-wise data
├── Unemployment_Rate_upto_11_2020.csv  # Dataset 2 – Jan–Nov 2020 with geo-coordinates
└── README.md                           # Project documentation
```

---

## 📌 Problem Statement

Unemployment is measured by the **unemployment rate** — the number of people who are unemployed as a percentage of the total labour force. India witnessed a dramatic rise in unemployment during the Covid-19 lockdown. This project explores:

- How unemployment changed over time across Indian states
- The difference between rural and urban unemployment
- The direct impact of the Covid-19 lockdown on employment
- Geographic distribution of unemployment across India

---

## 📂 Datasets

| File | Records | Period | Source |
|------|---------|--------|--------|
| `Unemployment_in_India.csv` | ~768 rows | May 2019 – Nov 2020 | CMIE via Kaggle |
| `Unemployment_Rate_upto_11_2020.csv` | ~267 rows | Jan 2020 – Nov 2020 | CMIE via Kaggle |

### Columns (Dataset 1)
| Column | Description |
|--------|-------------|
| `Region` | Indian state name |
| `Date` | Month-end date |
| `Frequency` | Monthly |
| `Estimated Unemployment Rate (%)` | % of unemployed in labour force |
| `Estimated Employed` | Number of employed persons |
| `Estimated Labour Participation Rate (%)` | % of working-age population active |
| `Area` | Rural / Urban |

### Additional Columns (Dataset 2)
| Column | Description |
|--------|-------------|
| `Region` | Geographic zone (North/South/East/West/Central) |
| `Longitude` | State centroid longitude |
| `Latitude` | State centroid latitude |

---

## 🛠️ Tech Stack

| Library | Purpose |
|---------|---------|
| `pandas` | Data loading, cleaning, manipulation |
| `numpy` | Numerical operations |
| `matplotlib` | Static charts |
| `seaborn` | Statistical visualizations & heatmaps |
| `plotly` | Interactive charts & geo maps |

---

## ⚙️ Installation & Setup

### 1. Clone / Download the project
```bash
git clone https://github.com/your-username/unemployment-analysis-india.git
cd unemployment-analysis-india
```

### 2. Create a virtual environment (optional but recommended)
```bash
python -m venv venv
source venv/bin/activate        # macOS/Linux
venv\Scripts\activate           # Windows
```

### 3. Install dependencies
```bash
pip install pandas numpy matplotlib seaborn plotly jupyter
```

### 4. Launch the notebook
```bash
jupyter notebook Unemployment_Analysis_India.ipynb
```

---

## 📓 Notebook Sections

| # | Section | Description |
|---|---------|-------------|
| 1 | Import Libraries | All required packages |
| 2 | Load & Inspect Data | Load both CSVs, preview rows |
| 3 | Data Cleaning | Parse dates, strip whitespace, drop nulls, rename columns |
| 4 | Descriptive Statistics | Mean, std, min, max for key metrics |
| 5 | Overall Trend | Monthly avg unemployment line chart with COVID annotation |
| 6 | Rural vs Urban | Side-by-side trend comparison |
| 7 | State-wise Avg | Horizontal bar chart ranked by unemployment |
| 8 | Top 5 / Bottom 5 | Most & least affected states |
| 9 | Covid-19 Impact | Pre vs Post lockdown comparison per state |
| 10 | Box Plot | Monthly distribution of unemployment |
| 11 | Heatmap | State × Month unemployment grid |
| 12 | Scatter Plot | Labour participation rate vs unemployment |
| 13 | Correlation Matrix | Relationships between numeric features |
| 14 | Region Analysis | Pie chart + 2020 monthly bar chart |
| 15 | Geo Map | Scatter geo map of India (bubble size = unemployment) |
| 16 | Sunburst Chart | Region → State hierarchical breakdown |
| 17 | Insights & Summary | Key findings + final summary table |

---

## 📊 Key Findings

- 🔴 **Covid-19 Shock:** India's unemployment rate surged from ~7–8% pre-lockdown to over **24% in April 2020** — the sharpest single-month spike on record.
- 🏙️ **Urban > Rural:** Urban unemployment was consistently higher than rural; both spiked sharply during the lockdown.
- 📍 **Most Affected States:** Jharkhand, Bihar, and Haryana recorded the highest average unemployment rates.
- 📍 **Least Affected States:** Meghalaya, Odisha, and Gujarat maintained relatively lower rates throughout.
- 📈 **Recovery:** Unemployment began declining from July 2020, suggesting partial economic recovery as restrictions eased.
- 🔗 **Labour Participation:** Mild negative correlation between labour participation rate and unemployment — people leaving the workforce can mask true unemployment levels.

---

## 📸 Sample Visualizations

- 📈 Line chart — National unemployment trend with lockdown band
- 🗺️ Geo scatter map — Bubble map across Indian states
- 🌡️ Heatmap — State × Month unemployment intensity
- ☀️ Sunburst — Region → State hierarchical view
- 📦 Box plots — Monthly distribution spread

---

## 🙌 Acknowledgements

- Dataset: [CMIE (Centre for Monitoring Indian Economy)](https://www.cmie.com/) via [Kaggle](https://www.kaggle.com/)
- Project inspired by **Oasis Infobyte Data Science Internship – Task 2**

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).