Module 12 Report

Overview of the Analysis

This analysis applies machine learning models to classify credit risk. The dataset contains financial information from loan applications, with the goal of predicting whether a loan is high or low risk.

Steps in the Analysis:

Data Exploration: The dataset was loaded and key features were reviewed.

Data Preprocessing: The dataset was split into features (X) and labels (y).

Model Training: A machine learning model was trained to classify loan risk.

Model Evaluation: Accuracy, precision, and recall metrics were used to assess model performance.

Results

Machine Learning Model:

Description: Logistic Regression

Accuracy Score: 99%

Precision Score:

Class 0: 1.00

Class 1: 0.87

Recall Score:

Class 0: 1.00

Class 1: 0.95

Summary

The Logistic Regression model performed exceptionally well, achieving an accuracy of 99%.

It perfectly predicted healthy loans (0), with a precision and recall of 1.00, meaning no false positives or false negatives for this class.

While not perfect in predicting high-risk loans (1), it still performed well, with a precision of 0.87, indicating that most high-risk loans were correctly identified, though some healthy loans were misclassified as high-risk (false positives).

The recall score of 0.95 for high-risk loans demonstrates the model's strong ability to catch most high-risk loans, missing only a few (false negatives), which is an excellent hit rate.

These strong results are further supported by high F-scores and weighted average values. However, given the class imbalance (only 625 high-risk loans vs. 18,759 healthy loans), the model might be favoring the majority class, so its performance should be interpreted with caution.

Recommendation: Since high recall for high-risk loans is crucial in credit risk assessment, this model is suitable for minimizing false negatives and ensuring risky loans are correctly classified. If further improvements are needed, techniques to handle class imbalance (e.g., resampling, adjusting class weights, or exploring models like Random Forest or Gradient Boosting) could be considered.
