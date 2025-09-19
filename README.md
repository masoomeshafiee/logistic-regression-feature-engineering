
# Logistic Regression with Feature Engineering for Healthcare & Toxicology

## Overview
This project implements **logistic regression from scratch** and applies it to two binary classification problems:  
- **Hepatitis dataset** → predicting liver disease diagnosis from patient blood test records  
- **Mushroom dataset** → predicting whether mushrooms are edible or poisonous based on physical traits  

The focus is on **feature engineering, recursive feature elimination, and hyperparameter tuning** to improve both interpretability and accuracy of logistic regression.

---

## Motivation
Logistic regression, despite being simple, is interpretable and well-suited for medical contexts.  Here, I show how thoughtful feature engineering and validation can significantly improve model performance.

---

## Key Features
- Logistic regression **implemented from scratch**  
- **Polynomial and interaction features** to capture nonlinear relationships  
- **Recursive Feature Elimination (RFE)** for feature selection  
- **Cross-validation** to reduce overfitting  
- **Hyperparameter tuning** (learning rate, convergence stability)  
- Detailed **data exploration and visualization and statistical analysis**

---

## Key Results
  - Baseline accuracy: ~71%  
  - After feature engineering & tuning: **~80%**  

**Takeaway**: Careful feature engineering and validation improve interpretability and predictive performance in healthcare-related datasets.

---

## Repository Structure
├── notebooks/
│ ├── project_part_A.ipynb # Hepatitis dataset analysis
│ ├── project_part_B.ipynb # Mushroom dataset analysis
├── report.pdf # Full project report
├── requirements.txt # Python dependencies
├── .gitignore # Ignore unnecessary files
└── README.md


---

## Getting Started

### Installation
Clone the repository:
```bash
git clone https://github.com/masoomeshafiee/logistic-regression-feature-engineering.git
cd logistic-regression-feature-engineering
```
Install dependencies:
```bash
pip install -r requirements.txt
```

### Usage
Open the Jupyter notebooks:
```bash
jupyter notebook notebooks/
```
Run the cells in:

**project_part_A.ipynb** → Hepatitis dataset
**project_part_B.ipynb** → Mushroom dataset


#### Future Work

- Extending analysis with Random Forests or LASSO regularization
- Applying pipeline to larger real-world medical datasets



