markdown# 🍎 Food Nutrition EDA & Correlation Analysis

![Python](https://img.shields.io/badge/Python-3.8+-blue?style=for-the-badge&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-4C72B0?style=for-the-badge)
![NumPy](https://img.shields.io/badge/NumPy-Numerical-013243?style=for-the-badge&logo=numpy)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter)

> Uncovering nutritional patterns, correlations, and food quality rankings through data-driven exploration.

---

## 📌 Overview

This project performs **Exploratory Data Analysis (EDA)** and **Correlation Analysis** on a real-world food nutrition dataset. By analyzing macronutrients and micronutrients — including calories, protein, fats, and carbohydrates — we surface meaningful insights about how nutritional components relate to each other and identify which foods offer the highest nutritional value.

---

## 🎯 Objectives

- ✅ Clean and preprocess the raw nutrition dataset
- ✅ Analyze distributions of key nutritional features
- ✅ Identify and visualize correlations between nutrients
- ✅ Detect outliers using statistical plots
- ✅ Engineer a **Nutrition Density** score to rank foods
- ✅ Extract actionable insights from data

---

## 🛠️ Tech Stack

| Library | Purpose |
|---|---|
| `Python` | Core programming language |
| `Pandas` | Data manipulation & preprocessing |
| `NumPy` | Numerical operations & masking |
| `Matplotlib` | Base plotting library |
| `Seaborn` | Statistical visualization |
| `WordCloud` | Text-based visual for food categories |

---

## 📂 Project Structure
```
Food-Nutrition-EDA-Correlation-Analysis/
│
├── 📓 Food_Nutrition_EDA_and_Correlation_Analysis.ipynb
├── 📊 dataset.csv
└── 📄 README.md
```

---

## 📊 Analysis Breakdown

### 🔹 Data Cleaning
- Identified and handled missing values
- Filtered and retained only relevant numeric columns
- Prepared dataset for downstream analysis

### 🔹 Exploratory Data Analysis
- **Distribution plots** — understand how each nutrient is spread
- **Boxplots** — detect outliers across nutritional features
- **Pairplots** — visualize multi-feature relationships simultaneously
- **WordCloud** — text visualization of food names/categories

### 🔹 Correlation Analysis
- Generated a full **correlation matrix** across all nutritional features
- Applied **upper triangle masking** for cleaner heatmap rendering:
```python
mask = np.triu(np.ones_like(correlation_matrix, dtype=bool))
correlation_matrix.mask(mask)
```

- Visualized with a **Seaborn heatmap** using diverging color scale

### 🔹 Feature Engineering
- Computed a custom **Nutrition Density Score** per food item
- Ranked foods based on overall nutrient quality

---

## 📈 Visualizations

| Chart Type | Insight Provided |
|---|---|
| 🔥 Heatmap | Correlation strength between all nutrients |
| 📊 Pairplot | Multi-dimensional feature relationships |
| 📈 Bar Chart | Food rankings by nutrition density |
| 📦 Boxplot | Outliers and spread per nutrient |
| ☁️ WordCloud | Text-based food category overview |

---

## 🔍 Key Insights

- 📌 **Strong positive correlation** found between total fat, saturated fat, and calorie content
- 📌 **Carbohydrates and sugars** show a predictable co-occurrence across food groups
- 📌 **Significant outliers** detected in sodium and sugar distributions
- 📌 **Nutrition Density ranking** highlights foods that maximize nutrients relative to calories

---

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/Food-Nutrition-EDA-Correlation-Analysis.git
cd Food-Nutrition-EDA-Correlation-Analysis
```

### 2. Install Dependencies
```bash
pip install pandas numpy matplotlib seaborn wordcloud
```

### 3. Launch the Notebook
```bash
jupyter notebook
```

Open `Food_Nutrition_EDA_and_Correlation_Analysis.ipynb` and run all cells.

---

## 🔮 Future Improvements

- [ ] Advanced statistical testing (t-tests, ANOVA)
- [ ] PCA for dimensionality reduction and visualization
- [ ] Predictive model for nutrition scoring
- [ ] Interactive dashboard deployment with **Streamlit**

---

## 👨‍💻 Author

**Nithyanantham A**
BCA Graduate | Python & Data Analytics Enthusiast
