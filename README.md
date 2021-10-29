# Predicting Credit Card Fraud

#### Matthew Kwee, 29 Oct. 2021

## Abstract

For this project, I compared multiple classification models in order to minimize the fraud-related costs incurred by banks.

Using a dataset from [Kaggle](https://www.kaggle.com/mlg-ulb/creditcardfraud"......"), I trained Logistic Regression, Random Forest, and Gradient Boosted Tree models, and scored them using a custom cost function.


## Design
The dataset presents a binary classification problem for machine learning models. Fraud reimbursement is a significant cost for banks; classifying transactions accurately would reduce a bank's expenditures, allowing them to provide services at more competitive prices.


## Data
I downloaded a fraud detection dataset from [Kaggle](https://www.kaggle.com/mlg-ulb/creditcardfraud"......"), which documents  284,807 transactions in Europe, over a span of two days.
Each datapoints has 30 features, all continuous. 28 of these are composite features in order to protect consumers' privacy, while Time and Purchase Amount are labeled.
The data are extremely unbalanced; only 492 transactions are fraudulent - 0.172%.

## Algorithms
1. Splitting data into 60-20-20 Train-Validation-Test buckets
2. Undersampling/weighting data in order to compensate for unbalanced dataset.
3. Designing a custom cost function to score models
4. Fitting and fine-tuning Logistic Regression, Random Forest, and Gradient Boosted Tree models. I considered the K-Nearest-Neighbors algorithm, but quickly discarded it; long prediction times and poor accuracy made it greatly inferior to the other models in this particular situation.

## Models
I considered Logistic Regression, Random Forest, and Gradient Boosted Tree classifiers before settling on random forest, which had the strongest scoring metrics across the board, and minimized fraud costs most effectively.

### Models
|Metric|Logistic Regression|Random Forest|XGBoost|
|-|-|-|-|
|Accuracy |0.998683|0.999719|0.999034
|Precision |0.630769|0.918919|0.704545
|Recall |0.752294|0.935780|0.853211
|F1 |0.686192|0.927273|0.771784
|Cost/Transaction|€0.0409889|€0.0339465|€0.0377385

## Tools
- Pandas and NumPy for data manipulation.
- Scikit-Learn and XGBoost for creating and training classification models.
- Google Sheets for methodology visualization (well, the little visualization that there was)


## Communication
My slide presentation can be found [here](https://docs.google.com/presentation/d/1VhAYXAPedJVgi2wCJ9LIrZnQWw0wwXehXpaiUgsjeo0/edit?usp=sharing"......").