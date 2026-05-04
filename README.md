# Credit Card Fraud Detection 🔍
### Machine Learning Project | Spring 2026 | MSc in Data Science

## Overview
A comprehensive machine learning study on detecting fraudulent credit card transactions.
Covers the full ML pipeline from exploratory data analysis to clustering and association rule mining.

---

## ⚠️ Dataset Setup (Required Before Running)
The dataset is NOT included in this repository due to its large size (144MB).

**Follow these steps:**
1. Go to: https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud
2. Click **Download**
3. Extract the zip file
4. Place **`creditcard.csv`** in the same folder as the notebook
5. Now run the notebook from top to bottom

> The dataset contains 284,807 credit card transactions (September 2013)
> with 492 fraud cases (0.172%) provided by ULB Machine Learning Group.

---

## Project Structure
| File | Description |
|---|---|
| `Group_MLProject.ipynb` | Full notebook with code and outputs |
| `README.md` | This file |

---

## Tasks Covered
| Task | Topic | Marks |
|---|---|---|
| 1 | Exploratory Data Analysis | 5 |
| 2 | Feature Selection (ANOVA, Mutual Info, Random Forest) | 10 |
| 3 | Class Imbalance (ROS, SMOTE, RUS) | 10 |
| 4 | Classification (Naive Bayes, Decision Tree, Random Forest, KNN, Logistic Regression) | 40 |
| 5 | Model Comparison and Evaluation | 10 |
| 6 | Association Rule Mining (Apriori) | 10 |
| 7 | Cluster Analysis (K-Means, Agglomerative, Divisive) | 15 |

---

## Results Summary
| Model | F1-Score | AUC-ROC |
|---|---|---|
| Random Forest ⭐ | 0.92 | 0.993 |
| Logistic Regression | 0.87 | 0.982 |
| Decision Tree | 0.86 | 0.974 |
| KNN (k=15) | 0.08* | 0.964 |
| Naive Bayes | 0.21 | 0.962 |

*KNN F1 is low due to class imbalance at prediction threshold — AUC-ROC is the reliable metric here.

**Best Model: Random Forest** with AUC-ROC = 0.993

---

## Requirements
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn mlxtend scipy

## How to Run
1. Download dataset from Kaggle (see Dataset Setup above)
2. Install requirements
3. Open `Group_MLProject.ipynb` in Jupyter
4. Run all cells top to bottom
