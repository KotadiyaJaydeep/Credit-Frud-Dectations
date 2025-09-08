# Credit Card Default Prediction

## 📖 Project Overview
The primary goal of this project is to predict credit card default risk in order to help financial institutions, banks, and credit card issuers manage their exposure to potential losses. By identifying customers who are likely to default, lenders can make informed decisions regarding credit issuance, limit assignments, and targeted financial products, ultimately ensuring the stability and profitability of their services.

---

## 📑 Table of Contents
1. [Problem Statement](#problem-statement)
2. [Dataset](#dataset)
3. [Data Pipeline](#data-pipeline)
4. [Project Structure](#project-structure)
5. [Conclusion](#conclusion)
6. [References](#references)

---

## 📌 Problem Statement
A credit card company in Taiwan is aiming to better understand the default behavior of its customers. By determining the probability that a customer will default and identifying the key contributing factors, the issuer can make smarter credit decisions. This data-driven approach helps in refining credit issuance strategies, offering tailored products, and mitigating financial risk by focusing on both current and prospective clients.

---

## 📂 Dataset
The dataset includes information on default payments, demographic characteristics, credit histories, and bill statements for credit card users in Taiwan between April 2005 and September 2005. It contains 30,000 records and 25 features, covering factors like payment history, credit usage, and personal attributes.

For further details, visit the [Kaggle dataset link](https://www.kaggle.com/code/selener/prediction-of-credit-card-default/input).

---

## 🔄 Data Pipeline

### 1. Data Exploration
- Loaded and inspected the dataset to understand the shape, feature types, and summary statistics.
- Identified trends, patterns, and anomalies within the dataset.

### 2. Exploratory Data Analysis (EDA)
- Performed univariate, bivariate, and multivariate analysis.
- Investigated distributions, correlations, and potential outliers.
- Visualized relationships using plots and charts to uncover hidden patterns.

### 3. Data Cleaning
- Handled missing values by applying mean, median, and mode imputations where necessary.
- Detected and treated outliers using clipping methods to preserve data integrity.
- Removed duplicate records to ensure clean and accurate datasets.

### 4. Feature Engineering
- Transformed categorical variables using encoding techniques.
- Applied correlation analysis to select significant features.
- Used SMOTE (Synthetic Minority Over-sampling Technique) to handle class imbalance in the target variable.

### 5. Model Training & Evaluation
- Scaled features using standardization to ensure uniformity across different magnitudes.
- Implemented eight machine learning classifiers, including Logistic Regression, KNN, Decision Tree, Random Forest, AdaBoost, XGBoost, and LightGBM.
- Tuned hyperparameters using GridSearchCV for optimized model performance.
- Evaluated models using performance metrics, with particular emphasis on Recall and F1-score due to the importance of minimizing false negatives in financial predictions.

---

## 📂 Project Structure

├── README.md
├── dataset/
│ └── credit_card_default.csv
├── problem-statement/
├── data-analysis/
│ ├── exploratory-data-analysis.ipynb
│ ├── univariate-analysis.png
│ └── bivariate-analysis.png
├── data-cleaning/
│ ├── missing-values-treatment.ipynb
│ ├── outlier-detection.ipynb
│ └── duplicated-values.ipynb
├── feature-engineering/
│ ├── encoding.ipynb
│ ├── feature-selection.ipynb
│ └── smote.ipynb
├── model-building/
│ ├── train-test-split.ipynb
│ ├── scaling.ipynb
│ └── model-training.ipynb
├── model-implementation/
│ ├── logistic-regression.ipynb
│ ├── knn.ipynb
│ ├── random-forest.ipynb
│ └── lightgbm.ipynb
├── model-results/
│ ├── performance-metrics.ipynb
│ └── model-explainability.ipynb
└── references/

---

## 📈 Conclusion

In this project, we tackled a binary classification problem aimed at predicting whether credit card customers are likely to default on payments.

**Key outcomes:**
- We processed and analyzed a dataset with 30,000 entries and 25 attributes, covering customer demographics and financial behavior.
- EDA provided a deep understanding of the data through statistical summaries and visualizations.
- Missing values and outliers were addressed using standard techniques to ensure data quality.
- Feature engineering helped enhance model performance by selecting the most relevant predictors and addressing class imbalance with SMOTE.
- Several machine learning algorithms were trained, tested, and evaluated using metrics such as F1-score and Recall. Given the cost of misclassifying a defaulter as a non-defaulter, recall was prioritized.
- KNN emerged as the best-performing model with a recall of **0.908**, while LightGBM, XGBoost, and Random Forest also delivered strong results with F1-scores around **0.866 to 0.868**.
- Ultimately, KNN was chosen as the final model due to its superior recall, ensuring that the model identifies as many true defaulters as possible — a critical factor in financial risk management.

This project demonstrates the power of data analytics and machine learning in reducing financial risk, improving credit issuance processes, and safeguarding both lenders and consumers.

---

## 📚 References
- Kaggle Dataset: [Prediction of Credit Card Default](https://www.kaggle.com/code/selener/prediction-of-credit-card-default/input)
- SMOTE Algorithm Documentation
- Scikit-learn API Reference

---

Feel free to explore, contribute, or ask questions!


