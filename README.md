🍎 Food Nutrition EDA & Correlation Analysis
📌 Project Overview

This project performs Exploratory Data Analysis (EDA) and Correlation Analysis on a food nutrition dataset to uncover patterns, relationships, and nutritional insights.

The goal is to analyze nutritional components such as calories, protein, fats, carbohydrates, and other macro/micro nutrients to understand how they relate to each other.

🎯 Objectives

Perform data cleaning and preprocessing

Analyze distribution of nutritional features

Identify correlations between nutrients

Visualize insights using multiple plots

Compute and rank foods by Nutrition Density

Build meaningful analytical insights from raw data

🛠️ Tech Stack

Python

Pandas

NumPy

Matplotlib

Seaborn

WordCloud

📂 Project Structure
Food-Nutrition-EDA-Correlation-Analysis/
│
├── Food_Nutrition_EDA_and_Correlation_Analysis.ipynb
├── dataset.csv
└── README.md

📊 Key Analysis Performed
🔹 Data Cleaning

Checked missing values

Filtered numeric columns

Prepared dataset for correlation analysis

🔹 Exploratory Data Analysis

Distribution plots

Boxplots for outlier detection

Pairplots for feature relationships

WordCloud visualization for text features

🔹 Correlation Analysis

Generated correlation matrix

Applied upper triangle masking using:

mask = np.triu(np.ones_like(correlation_matrix, dtype=bool))
correlation_matrix.mask(mask)


Visualized correlations using Seaborn heatmap

🔹 Feature Engineering

Calculated Nutrition Density

Ranked foods based on nutrient quality

📈 Visualizations Included

Heatmaps

Pairplots

Bar charts

Boxplots

WordCloud

🔍 Insights

Identified strong correlations between macronutrients.

Observed relationships between calorie content and fat/carbohydrate levels.

Detected outliers in nutritional distribution.

Ranked foods based on nutrient density.

🚀 How to Run

Clone the repository:

git clone https://github.com/your-username/Food-Nutrition-EDA-Correlation-Analysis.git


Install required libraries:

pip install pandas numpy matplotlib seaborn wordcloud


Open the Jupyter Notebook:

jupyter notebook

📌 Future Improvements

Add advanced statistical analysis

Implement PCA for dimensionality reduction

Build predictive model for nutrition scoring

Deploy as interactive dashboard (Streamlit)

👨‍💻 Author

Nithyanantham A
BCA Graduate | Python & Data Analytics Enthusiast
