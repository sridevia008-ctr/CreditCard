# Credit Card Default Prediction & Risk Analysis

This repository contains an end-to-end Machine Learning project that predicts credit card client default behaviors. The project covers data preprocessing, categorical feature encoding, handling severe class imbalance using **SMOTE**, exploratory data analysis, and building predictive models.

---

## 📌 Project Overview

Predicting credit card default is crucial for financial institutions to manage credit risk and optimize lending strategies. This project analyzes demographic factors, credit limit details, repayment history, and bill statement values to accurately identify potential defaulters.

### Key Highlights
* **Data Preprocessing & Cleaning:** Managed missing values and standardized feature formats.
* **Categorical Encoding:** Applied **One-Hot Encoding** on demographic variables such as `MARRIAGE` and `EDUCATION`.
* **Addressing Class Imbalance:** Utilized **SMOTE (Synthetic Minority Over-sampling Technique)** to balance the dataset target distribution (expanding training samples to ~46,728 rows for balanced class training).

---

## 📊 Dataset Features

The dataset includes demographic and historical financial record attributes:

| Feature Category | Features Included |
| :--- | :--- |
| **Demographics** | `AGE`, `SEX`, `EDUCATION` (`HIGH_SCHOOL`, `UG`, `PG`, `OTHERS`), `MARRIAGE` (`MARRIED`, `SINGLE`, `OTHERS`) |
| **Credit Details** | `LIMIT_BAL` (Amount of given credit) |
| **Repayment Status** | Past monthly payment statuses (`SEP_PAY`, `AUG_PAY`, `JUL_PAY`, `JUN_PAY`, `MAY_PAY`, `APR_PAY`) |
| **Bill & Payment History** | Monthly bill statements and previous payment amounts (`MAY_PAYMENT`, `APR_PAYMENT`, etc.) |
| **Target Variable** | `target` (0 = Non-Defaulter, 1 = Defaulter) |

---

## ⚙️ Tech Stack & Libraries

* **Language:** Python 3.x
* **Environment:** Jupyter Notebook / Anaconda
* **Data Manipulation:** `pandas`, `numpy`
* **Data Visualization:** `matplotlib`, `seaborn`
* **Machine Learning & Resampling:** `scikit-learn`, `imbalanced-learn` (`SMOTE`)

---

## 🚀 Getting Started

### Prerequisites

Ensure you have Python installed along with the required dependencies:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn imbalanced-learn
