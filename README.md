# ICU Patient Data Analysis & Machine Learning 🏥📊🤖

Welcome to the **ICU Patient Data Analysis & Machine Learning** project! This repo shows how we transform, analyze, and build predictive models using ICU clinical data to better understand patient outcomes — especially focusing on ICU mortality risk.

---

## 🚀 Project Goal

The goal of this project is to build a proof-of-concept machine learning pipeline that predicts ICU patient mortality within 24 hours using rich clinical features. We do this by carefully cleaning and transforming ICU datasets, engineering meaningful features, and training interpretable models.

---

## 📝 Summary

In this project, you will find a complete workflow that covers:

* Data ingestion and anonymization to protect patient privacy 🔒
* Data transformation and standardization to a common ICU schema 📋
* Exploratory Data Analysis (EDA) for feature understanding and insight discovery 🔍
* Feature engineering for richer clinical signals 💡
* Handling class imbalance and careful train/test splits 🧩
* Model training, evaluation, and interpretation with XGBoost and Logistic Regression 🎯
* Visualization of feature importance and correlation heatmaps 📈

---

## 🛠️ Step-by-Step Breakdown

### 1. Data Collection & Preparation 📥

We start by loading the raw ICU data and associated clinical tables, ensuring data quality and handling missing values. Anonymization techniques protect sensitive patient identifiers.

### 2. Standardizing Data to ICU Schema 🗂️

All features are converted to a standardized format with clear data types and descriptions — making downstream processing and modeling easier and more reliable.

### 3. Encoding Categorical Features 🔠

Categorical columns are one-hot encoded, and gender is split into binary columns, to prepare for machine learning algorithms that require numeric input.

### 4. Indexing & Sorting ⏳

Synthetic timestamps are added and data sorted to facilitate efficient queries and maintain data integrity.

### 5. Feature Engineering & Aggregation 🔧

Vital signs, lab results, fluid outputs, and diagnosis codes are aggregated over the first 24 hours in the ICU to capture the early patient state. Composite clinical scores like the shock index and lab abnormality counts are created to summarize risk.

### 6. Exploratory Data Analysis (EDA) 🔍

We dive deep into understanding data distributions, correlations, and differences between survivors and non-survivors — providing clinical insights and confirming feature relevance.

### 7. Handling Class Imbalance & Train/Test Splits ⚖️

Given the imbalance (few mortality events), we carefully split data ensuring positive cases in the test set and calculate appropriate weighting to balance the model training.

### 8. Model Training & Evaluation 🎯

We train an XGBoost classifier, evaluate its accuracy, ROC-AUC, and generate classification reports — interpreting results with an emphasis on the proof-of-concept nature due to limited data.

### 9. Feature Importance & Visualization 📊

Important clinical predictors are visualized to highlight which features contribute most to mortality risk prediction — aiding interpretability.

### 10. Database Integration & ETL 🛢️

DataFrames are inserted into a MySQL database with descriptive table names for organized storage and further analysis.

---

## ⚠️ Important Notes

* The dataset is limited with a small number of positive mortality cases, so the model is intended as a **proof of concept** and **not** for clinical deployment.
* Data anonymization and privacy are maintained throughout.
* This repo demonstrates an end-to-end data science workflow with a focus on clarity, reproducibility, and interpretability.

---

## 👩‍💻 How to Use This Repo

1. Clone the repo
2. Set up your environment and install dependencies
3. Follow the notebooks/scripts to run ETL, feature engineering, and model training
4. Explore results and visualizations to gain insights
5. Customize with your own data or extend the analysis
---

Thanks for checking out this project! 🚑💻✨


Would you like me to format this into markdown `.md` file style for direct upload?
