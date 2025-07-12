# MB Bank Customer Churn Prediction

This project was developed as the final capstone for a Data Science in Business course (Datapot x FTU). The goal is to predict customer churn using anonymized transaction and savings data provided by MB Bank (dummy dataset).

## Objective

To identify which customers are likely to churn (i.e., stop using the bank’s services) based on their behavior and transaction history, in order to support customer retention strategies.

## Dataset Description

The dataset contains customer transaction and savings behavior from 2020 and partial activity data from 2021 (March and June).

Key features include:

- Demographic attributes (age, gender, occupation, etc.)
- 2020 transactional data (spending volume, frequency, savings usage)
- 2021 activity markers (to define churn label)
- Target variable: churn (1 = customer churned, 0 = retained)

## Methodology

1. Churn Definition  
   - Customers were labeled as “churned” if they had no transactions and did not use the “Heo số” savings app in both March and June 2021.

2. Data Preprocessing  
   - Removed redundant or irrelevant columns (e.g., IDs, location codes)  
   - Filtered out inactive accounts in late 2020  
   - Handled missing values  
   - Engineered features from transaction and savings behavior

3. Model Building  
   - Split data into training and testing sets  
   - Trained multiple classifiers:  
     - Logistic Regression  
     - Random Forest  
     - Gradient Boosting  
     - Support Vector Machine (SVM)  
     - K-Nearest Neighbors (KNN)  
   - Evaluated models using:  
     - Cross-validation  
     - F1-score  
     - Confusion Matrix  

## Tools Used

- Python (pandas, numpy, matplotlib, seaborn, scikit-learn)
- Jupyter Notebook

## Results

- The best-performing model achieved an F1-score of approximately XX (replace with actual score).
- Important features included: savings behavior, transaction volume, and frequency of activity.

## Learning Outcomes

- Learned how to define a real-world business problem from raw data
- Applied classification models to predict churn
- Gained experience with end-to-end ML pipeline from data cleaning to model evaluation
