# Credit Card Default Prediction & Data EDA

## Project Overview

This project focuses on **Exploratory Data Analysis (EDA)** and **Machine Learning modeling** to predict whether a credit card user will default on their payment. The goal is to analyze customer demographic, credit, and payment history data to identify patterns that lead to default and build predictive models to classify default risk.

This project is useful for financial institutions to minimize risk and make better lending decisions.

---

## Dataset Information

The dataset contains customer information such as:

* Credit limit
* Gender
* Education
* Marital status
* Age
* Repayment status (past months)
* Bill amount (past months)
* Previous payment amount (past months)
* Default payment status (Target variable)

**Target Variable:**

* `default.payment.next.month`

  * 1 = Default
  * 0 = No Default

---

## Project Workflow

### 1. Data Cleaning

* Checked for missing values
* Renamed columns for better readability
* Removed duplicate records
* Corrected data types
* Handled outliers where necessary

### 2. Exploratory Data Analysis (EDA)

EDA was performed to understand patterns and relationships between variables.

**EDA includes:**

* Default vs Non-default distribution
* Gender vs Default
* Education vs Default
* Marital Status vs Default
* Age distribution
* Credit limit vs Default
* Repayment status vs Default
* Bill amount trends
* Payment amount trends
* Correlation heatmap

### 3. Feature Engineering

* Created new features from repayment history
* Normalized/Standardized numerical features
* Encoded categorical variables

### 4. Model Building

Machine learning models used:

* Logistic Regression
* Decision Tree
* Random Forest
* XGBoost
* Support Vector Machine (SVM)

### 5. Model Evaluation

Models were evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix
* ROC-AUC Score

---

## Tools & Libraries Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost
* Jupyter Notebook

---

## Key Insights

* Customers with **low credit limit** have higher default probability.
* **Repayment history** is the strongest predictor of default.
* Customers who delayed payments for multiple months are more likely to default.
* **Younger age group** has slightly higher default rate.
* **Lower payment amounts** relative to bill amount indicate higher default risk.

---

## Project Structure

```
Credit-Card-Default-Prediction/
│
├── data/
│   └── credit_card_default.csv
│
├── notebooks/
│   └── EDA_and_Model.ipynb
│
├── models/
│   └── trained_model.pkl
│
├── images/
│   └── plots.png
│
├── README.md
└── requirements.txt
```

---

## How to Run This Project

1. Clone the repository:

```
git clone https://github.com/your-username/credit-card-default-prediction.git
```

2. Navigate to the project folder:

```
cd credit-card-default-prediction
```

3. Install dependencies:

```
pip install -r requirements.txt
```

4. Run Jupyter Notebook:

```
jupyter notebook
```

---

## Future Improvements

* Hyperparameter tuning
* Deploy model using Flask/Streamlit
* Use Deep Learning models
* Handle class imbalance using SMOTE
* Feature importance analysis

---

## Author

Your Name
Data Science / Machine Learning Project

---

## License

This project is for educational purposes.
