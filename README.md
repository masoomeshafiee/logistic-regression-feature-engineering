
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
logistic-regression-feature-engineering/

│── README.md

│── report.pdf

│── notebooks/
│    ├── hepatitis_logistic_regression.ipynb   # Hepatitis dataset
│
│    ├── mushroom_logistic_regression.ipynb   # Mushroom dataset

│── environment.yml                        

│── requirements.txt

│── .gitignore


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

**hepatitis_logistic_regression.ipynb** → Hepatitis dataset

**mushroom_logistic_regression.ipynb** → Mushroom dataset

How to run:

- In each code, there is a section called "Data Loading". In the first cell of this section, you can determine the path of the dataset. 

- By simply setting the file path to the CSV file on your drive, you can run the whole code and no further changes are required. 

- Also, if a local environment is used to run the code, the second cell of the "Data Loading" section which is commented out by default, 
can be set to point to the CSV file on the local hard drive, and the whole code will run with no further changes. It is important to remember if a local environment is used, the Google Drive mount should be commented out.


- Beware that since the RFE is computationally heavy, it may take a while for our code to run on notebook . 

##### Code structure:

Each section has a title in the code. But the overall structure for both files is as below:
1. Loading the required libraries and defining necessary functions:
In this section, you can find all the developed functions that we used in our code, namely:
- Logistic Regression class
- Train-test-split function
- K-fold-cross-validation function
- RFE function

2. Data Loading:
This section is responsible for loading the dataset into a pandas dataset

3. Data visualization:
This section is responsible for familiarizing and visualizing the data at hand.

4. Model development:
This section is responsible for model development and testing different features. Each section for a different set of features is marked from 1 to the number of categories of features that we engineered. 
To evaluate each section, we ran k-fold-cross-validation, and RFE to determine feature importance, and printed the result of training the model on our test dataset.
Lastly, the best features were selected in selected_features and we did the above procedure for this final set of features, which is indicated by "Accuracy on test dataset".

5. Testing different learning rates:
This section is responsible for evaluating the effect of different learning rates and epsilons on training the model and finally plotting the result.


#### Future Work

- Extending analysis with Random Forests or LASSO regularization
- Applying pipeline to larger real-world medical datasets



