# 🚨 Fraud Detection using Machine Learning

A Machine Learning project that detects fraudulent credit card transactions using supervised learning techniques. This project focuses on handling highly imbalanced data with **SMOTE** and compares the performance of **Logistic Regression** and **Random Forest Classifier** using appropriate evaluation metrics.

---

## 📌 Project Overview

Credit card fraud is a significant financial challenge. Since fraudulent transactions are extremely rare compared to legitimate ones, traditional accuracy is not a reliable evaluation metric.

This project builds a fraud detection pipeline that:

* Performs data exploration and preprocessing.
* Handles class imbalance using **SMOTE (Synthetic Minority Over-sampling Technique)**.
* Trains multiple classification models.
* Evaluates models using **Precision, Recall, F1-Score, and ROC-AUC**.
* Compares model performance to identify the best fraud detection model.

---

## 🎯 Objectives

* Analyze the credit card transaction dataset.
* Handle imbalanced classes using SMOTE.
* Train and evaluate classification models.
* Compare model performance using appropriate metrics.
* Build a reproducible machine learning workflow.

---

## 📂 Dataset

The dataset used in this project is **not included** in this repository because it exceeds GitHub's 100 MB file size limit.

You can download the dataset from Kaggle:

**Credit Card Fraud Detection Dataset**
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

After downloading, place the `creditcard.csv` file inside the project folder before running the notebook.

---

## 🛠️ Technologies Used

* Python
* Jupyter Notebook
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Imbalanced-learn (SMOTE)

---

## 📊 Project Workflow

1. Import required libraries
2. Load the dataset
3. Explore and understand the data
4. Perform basic data preprocessing
5. Scale transaction amount
6. Split data into training and testing sets
7. Apply SMOTE to balance the training data
8. Train Logistic Regression model
9. Train Random Forest Classifier
10. Evaluate both models
11. Compare model performance
12. Draw conclusions

---

## 🤖 Machine Learning Models

* Logistic Regression
* Random Forest Classifier

---

## 📈 Evaluation Metrics

Instead of relying on Accuracy, the models are evaluated using:

* Precision
* Recall
* F1-Score
* ROC-AUC Score
* Confusion Matrix
* ROC Curve

---

## 📁 Project Structure

```text
Fraud_Detection_Project/
│
├── creditcard.csv
├── Fraud_Detection_Project.ipynb
├── README.md
└── requirements.txt
```

---

## ▶️ How to Run

1. Clone the repository.

```bash
git clone <repository-url>
```

2. Install dependencies.

```bash
pip install -r requirements.txt
```

3. Place `creditcard.csv` in the project folder.

4. Open the notebook.

```bash
jupyter notebook Fraud_Detection_Project.ipynb
```

5. Run all cells.

---

## 📌 Results

The project compares Logistic Regression and Random Forest after applying SMOTE.

The final model is selected based on:

* Higher Precision
* Better Recall
* Higher F1-Score
* Better ROC-AUC Score

---

## 🚀 Future Improvements

* Hyperparameter Tuning using GridSearchCV
* Cross Validation
* XGBoost Classifier
* LightGBM
* Feature Selection
* Model Deployment using Streamlit or Flask

---

## 👨‍💻 Author

**Zubair ulhassan**

BS Data Science

--=