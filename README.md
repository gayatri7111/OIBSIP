# Oasis Infobyte Internship Program (OIBSIP) — Data Analytics

Welcome to the **Oasis Infobyte Internship Program (OIBSIP)** project submission repository by **Gayatri Gurav**. This repository contains completed, end-to-end analytical solutions, machine learning models, exploratory data analyses, and data preprocessing pipelines for both **Level 1** and **Level 2** of the **Data Analytics Track**.

---

## 📂 Repository Structure & Submission Format

Every project in this repository strictly adheres to the official OIBSIP submission naming convention:
```
OIBSIP/[TrackName]-[Level/Task]-[ProjectName]/
```

```
OIBSIP/
├── .gitignore
├── README.md
└── OIBSIP/
    ├── DataAnalytics-L1-EDARetailSales/
    │   ├── Retail_Sales_EDA(task 1).ipynb
    │   ├── retail_sales_dataset.csv
    │   ├── requirements.txt
    │   ├── README.md
    │   └── visualizations/
    ├── DataAnalytics-L1-CustomerSegmentationRFM/
    │   ├── Customer_Segmentation_RFM(task 2).ipynb
    │   ├── retail_sales_dataset.csv
    │   ├── requirements.txt
    │   ├── README.md
    │   └── visualizations/
    ├── DataAnalytics-L1-DataCleaningRetailSales/
    │   ├── Data_Cleaning_Retail_Sales(task 3).ipynb
    │   ├── retail_sales_dataset.csv
    │   ├── requirements.txt
    │   └── README.md
    ├── DataAnalytics-L1-SentimentAnalysisNLP/
    │   ├── Sentiment_Analysis_NLP(task 4).ipynb
    │   ├── Amazon Product Reviews dataset.csv
    │   ├── requirements.txt
    │   ├── README.md
    │   └── visualizations/
    ├── DataAnalytics-L2-HousePricePrediction/
    │   ├── Predicting_House_Prices(task 1).ipynb
    │   ├── train.csv
    │   ├── requirements.txt
    │   ├── README.md
    │   └── visualizations/
    ├── DataAnalytics-L2-WineQualityPrediction/
    │   ├── Wine_Quality_Prediction(task 2).ipynb
    │   ├── winequality-red.csv
    │   ├── requirements.txt
    │   ├── README.md
    │   └── visualizations/
    └── DataAnalytics-L2-FraudDetection/
        ├── Fraud_Detection(task 3).ipynb
        ├── requirements.txt
        ├── README.md
        └── visualizations/
```

---

## 📊 Projects Overview

### Level 1 Tasks

| # | Task | Project Name | Description & Key Results | Folder Link |
| :-: | :--- | :--- | :--- | :--- |
| **01** | Level 1 — Task 1 | **Exploratory Data Analysis (EDA) on Retail Sales** | Comprehensive exploratory analysis uncovering demographic trends, AOV ($456), and sales seasonality across 1,000 retail records. | [View Project](./OIBSIP/DataAnalytics-L1-EDARetailSales) |
| **02** | Level 1 — Task 2 | **Customer Segmentation using RFM & K-Means** | Behavioral segmentation grouping customers into actionable cohorts based on Recency, Frequency, and Monetary metrics with K-Means clustering. | [View Project](./OIBSIP/DataAnalytics-L1-CustomerSegmentationRFM) |
| **03** | Level 1 — Task 3 | **Retail Sales Data Cleaning & Preprocessing** | Systematic data quality pipeline resolving missing values, duplicates, formatting inconsistencies, and verifying mathematical integrity. | [View Project](./OIBSIP/DataAnalytics-L1-DataCleaningRetailSales) |
| **04** | Level 1 — Task 4 | **Sentiment Analysis using NLP & ML** | Text classification pipeline using TF-IDF and Naive Bayes / Linear SVM, achieving **80.0% accuracy** on e-commerce product reviews. | [View Project](./OIBSIP/DataAnalytics-L1-SentimentAnalysisNLP) |

### Level 2 Tasks

| # | Task | Project Name | Description & Key Results | Folder Link |
| :-: | :--- | :--- | :--- | :--- |
| **01** | Level 2 — Task 1 | **House Price Prediction via Advanced Regression** | Predictive regression modeling capturing **83.01% of variance ($R^2 = 0.8301$)** with an RMSE of $36,095.94 using Linear Regression. | [View Project](./OIBSIP/DataAnalytics-L2-HousePricePrediction) |
| **02** | Level 2 — Task 2 | **Red Wine Quality Multi-Class Classification** | Multi-class modeling on 11 physicochemical metrics, achieving **74.38% accuracy** and 0.7100 Macro F1 with Random Forest Classifier. | [View Project](./OIBSIP/DataAnalytics-L2-WineQualityPrediction) |
| **03** | Level 2 — Task 3 | **Credit Card Fraud Detection using SMOTE** | Resampling and cost-sensitive classification catching **91.43% of fraudulent transactions** with **86.49% precision** via Random Forest. | [View Project](./OIBSIP/DataAnalytics-L2-FraudDetection) |

---

## 🛠️ Technologies & Ecosystem

- **Languages:** Python 3.8+
- **Data Manipulation:** `pandas`, `numpy`
- **Visualization:** `matplotlib`, `seaborn`
- **Machine Learning & Pipelines:** `scikit-learn`, `imbalanced-learn`
- **Natural Language Processing:** `nltk`, `wordcloud`
- **Interactive Development:** Jupyter Notebooks (`.ipynb`)

---

## 🚀 Quick Start Guide

### 1. Clone the Repository
```bash
git clone https://github.com/gayatri7111/OIBSIP.git
cd OIBSIP
```

### 2. Choose a Project & Install Dependencies
Navigate into any project directory and install the dedicated dependencies:
```bash
cd OIBSIP/DataAnalytics-L1-EDARetailSales
pip install -r requirements.txt
```

### 3. Launch Jupyter Notebook
```bash
jupyter notebook
```

---

## 👤 Author & Intern Details

- **Intern Name:** Gayatri Gurav
- **Track:** Data Analytics
- **Internship Program:** Oasis Infobyte Virtual Internship Program (OIBSIP)
- **GitHub Profile:** [@gayatri7111](https://github.com/gayatri7111)
- **Repository:** [OIBSIP](https://github.com/gayatri7111/OIBSIP)
