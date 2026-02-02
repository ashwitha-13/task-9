# task-9
random forest
Credit Card Fraud Detection using Random Forest
Overview:
This project focuses on detecting fraudulent credit card transactions using machine learning techniques. Fraud detection datasets are typically highly imbalanced, where fraudulent transactions form a very small percentage of the data. To address this challenge, the project uses appropriate evaluation metrics and ensemble learning methods to build an effective fraud detection model.

The project compares a baseline Logistic Regression model with a Random Forest classifier and identifies important features contributing to fraud detection.

Dataset:
Dataset Name: Credit Card Transactions Dataset
File Used: creditcardcsv.csv
Target Variable: Automatically detected (e.g., Class, fraud, is_fraud, target, or label)
Nature of Data: Combination of numerical and categorical features
Key Challenge: Severe class imbalance between fraud and non-fraud transactions

Tools and Libraries:
Python
Pandas
NumPy
Matplotlib
Scikit-learn
Joblib

Steps Performed:
Loaded the dataset and analyzed fraud vs non-fraud transaction distribution.
Automatically detected the target (fraud) column to avoid hard-coded dependencies.
Separated features and target variable and removed non-useful identifiers such as Time or Id when present.
Handled categorical features using one-hot encoding to make the data suitable for machine learning models.
Split the dataset into training and testing sets using stratified sampling to preserve class imbalance.
Trained a baseline Logistic Regression model for performance comparison.
Trained a Random Forest classifier with 100 estimators and class balancing.
Evaluated models using Precision, Recall, and F1-score instead of accuracy.
Visualized feature importances from the Random Forest model to identify key fraud indicators.
Compared the performance of Logistic Regression and Random Forest models.
Saved the best-performing model using Joblib for future reuse.

Evaluation Metrics:
Due to class imbalance, accuracy is misleading for fraud detection. Therefore, the following metrics were used:
Precision
Recall
F1-score
These metrics provide a better understanding of how well the model identifies fraudulent transactions.

Results:
The Random Forest model outperformed the baseline Logistic Regression model, especially in terms of recall and F1-score. Feature importance analysis revealed the most influential factors contributing to fraud detection.

Output Files:
fraud_detection_random_forest.pkl – Saved Random Forest model
Feature importance plot
Console-based performance comparison table

Conclusion:
This project demonstrates the effectiveness of ensemble learning methods such as Random Forest in handling imbalanced fraud detection problems. Proper preprocessing, metric selection, and model comparison are critical for building reliable fraud detection systems.
