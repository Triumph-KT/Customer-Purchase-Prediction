# Tourism Package Purchase Prediction

Developed a machine learning model to predict whether customers are likely to purchase a new wellness tourism package, enabling targeted marketing strategies and customer outreach for a travel company.

## Project Overview

This project aims to identify potential customers for a newly launched tourism package by analyzing customer demographics and behavior. By accurately predicting customer interest, the business can focus marketing efforts and improve conversion rates.

## Dataset

The dataset includes customer records with features such as:
- Age
- Monthly Income
- Number of trips
- Passport ownership
- Occupation
- Preferred city tier
- Number of follow-ups
- Marital status

The target variable is:
- **Purchase Decision** (Yes/No)

## Objectives

- Analyze customer profiles to determine factors influencing purchase decisions.
- Build classification models to predict customers likely to purchase the tourism package.
- Optimize model thresholds to prioritize recall, ensuring high identification of potential buyers.
- Provide strategic business insights to enhance marketing efforts.

## Methods

- Data cleaning and preprocessing
- Exploratory Data Analysis (EDA) to identify trends and influential features
- Model training and comparison, including:
  - Logistic Regression
  - Support Vector Machines (SVM) with linear and RBF kernels
  - Decision Tree Classifier (with GridSearchCV tuning)
  - Random Forest Classifier
- Precision-Recall Curve analysis for threshold optimization
- Model evaluation with accuracy, recall, precision, and F1-score

## Results

- Identified key purchase predictors: **monthly income**, **age**, and **number of trips**.
- Achieved the best model performance with **SVM (RBF kernel)**, reaching a **recall of 69%**.
- Improved recall significantly through threshold tuning, increasing from 26% to 69%.
- Decision Trees and Random Forests provided interpretability but showed overfitting tendencies without tuning.
- Logistic Regression and linear models underperformed on the imbalanced dataset.

## Business Impact

- Enabled targeted marketing towards:
  - Customers with higher incomes and travel experience.
  - Younger, single customers more likely to buy travel packages.
  - Passport holders who prefer international travel.
- Informed strategies to expand customer reach in **tier 2 cities**.
- Suggested customized package offerings for high-income and executive-level customers.
- Recommended optimizing follow-up strategies to convert interested leads.

## Technologies Used

- Python
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
- GridSearchCV

## How to Run

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/tourism-package-purchase-prediction.git
    ```

2. Install required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Launch Jupyter Notebook:
    ```bash
    jupyter notebook
    ```

4. Open and run the notebook to reproduce the results.
