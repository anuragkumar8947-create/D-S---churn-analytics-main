# Data Science & Customer Churn Analytics Pipeline

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/gargdhruv020/Data-Science-Churn-Analytics/blob/main/notebooks/Data_Analysis_Pipeline.ipynb)

An end-to-end multi-level data science project featuring data cleaning, exploratory data analysis, time-series decomposition, predictive machine learning (churn classification), NLP sentiment analysis, and an interactive Power BI dashboard.

---

## 📌 Project Overview

- **Level 1 (Basic):** 
  - Data cleaning, deduplication, and categorical encoding on Telecom Churn datasets (`churn-bigml-80.csv`, `churn-bigml-20.csv`).
  - Summary statistics, histograms, boxplots, scatter plots, and correlation heatmaps on the Iris dataset (`1) iris.csv`).
- **Level 2 (Intermediate):** 
  - Simple Linear Regression on the Boston Housing dataset (`4) house Prediction Data Set.csv`).
  - Time-Series 30-Day Moving Average & Seasonal Decomposition on Apple stock data (`2) Stock Prices Data Set.csv`).
  - K-Means Clustering ($K=3$) with Elbow Method analysis on the Iris dataset.
- **Level 3 (Advanced):**
  - **Predictive Modeling:** Logistic Regression, Decision Tree, and Random Forest classification with Hyperparameter Tuning (`GridSearchCV`) for customer churn prediction.
  - **NLP Sentiment Analysis:** Text preprocessing, `TextBlob` polarity scoring, and Word Cloud generation on customer review data (`3) Sentiment dataset.csv`).
  - **Business Intelligence Dashboard:** Interactive Power BI dashboard (`.pbix`) built using model prediction outputs.

---

## 🛠️ Tools & Libraries Used

- **Language:** Python 3.x
- **Data Analysis & Visualization:** `pandas`, `numpy`, `matplotlib`, `seaborn`
- **Machine Learning & Stats:** `scikit-learn`, `statsmodels`
- **NLP:** `nltk`, `textblob`, `wordcloud`
- **BI Dashboard:** Power BI Desktop

---

## 📁 Repository Structure

```text
Data-Science-Churn-Analytics/
│
├── data/                       # Raw input CSV datasets
│   ├── 1) iris.csv
│   ├── 2) Stock Prices Data Set.csv
│   ├── 3) Sentiment dataset.csv
│   ├── 4) house Prediction Data Set.csv
│   ├── churn-bigml-80.csv
│   └── churn-bigml-20.csv
│
├── outputs/                    # Generated charts & exported predictions
│   ├── churn_dashboard_data.csv
│   ├── iris_eda_summary.png
│   ├── linear_regression_house.png
│   ├── time_series_stock.png
│   ├── kmeans_clusters_iris.png
│   ├── sentiment_distribution.png
│   └── wordcloud.png
│
├── models/                     # Saved model & scaler .pkl files
│   ├── random_forest_churn_model.pkl
│   ├── linear_regression_house_model.pkl
│   └── churn_scaler.pkl
│
├── dashboard/                  # Power BI report files & static PDF exports
│   └── Churn_Analytics_Dashboard.pdf
│
├── notebooks/                  # Google Colab / Jupyter Notebook
│   └── Data_Analysis_Pipeline.ipynb
│
├── .gitignore                  # Git ignore rules
├── requirements.txt            # Python dependencies
└── README.md                   # Project documentation