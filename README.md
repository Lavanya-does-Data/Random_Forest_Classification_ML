**Random Forest: Financial Risk Prediction**
**Overview**

This project applies Random Forest to a financial customer dataset to investigate predictive performance across both regression and classification tasks.

Objective

Build and evaluate Random Forest models using customer financial and behavioral attributes, while comparing model performance across different prediction tasks.

Dataset

The dataset contains customer-level financial information including income, credit score, BNPL activity and debt, payment history, employment status, shopping behavior, and transaction values.

Customer_ID was excluded from the modeling process.

Approach
Data quality checks and preprocessing
Missing-value treatment
Categorical feature encoding
Train/test split
Random Forest model development
Model evaluation
Performance analysis
Models
Random Forest Regression

Predicts a continuous financial outcome.

Metrics: R², MAE, MSE

Random Forest Classification

Predicts customer default-risk categories.

Metrics: Accuracy, Precision, Recall, F1-Score, Confusion Matrix

Key Findings:
The main finding was that the customer financial variables contained enough signal for Random Forest to make fairly strong predictions, but the classification performance wasn't uniform across risk categories. The model was very good at identifying Low-risk customers and reasonably good at identifying High-risk customers, but it struggled with Medium-risk customers. So although the overall accuracy was about 96%, looking at the class-level recall showed us that accuracy was somewhat misleading because the dataset was dominated by Low-risk customers. From a business perspective, that tells me that improving detection of the less represented and more ambiguous risk categories would be more valuable than simply optimizing overall accuracy.

Tech Stack
Python · Pandas · NumPy · Scikit-learn · Jupyter Notebook
