# Metis Project 4: Credit Card Fraud

The goal of this project is to construct a model that can predict credit card fraud.


To achieve this goal, I constructed a Logistic Regression model that uses transaction data to flag transactions as potentially fraudulent.

First, I placed the data into train/test sets with an 80/20 ratio.

Next, I created a default Logistic Regression model, and fit it to the training data as a baseline.
I used the test data to score the model - the results are shown below.
(it's also best viewed with GitHub's light theme)
![Alt text](https://raw.githubusercontent.com/MK38993/Metis-Project-4---Classification/main/ROC%20LogReg.png "HEY      EVERY      !! IT'S ME!!! EV3RY  BUDDY  'S FAVORITE [[Number 1 Rated Salesman1997]] SPAMT   SPAMTON G. SPAMTON!!")

| 	 Test Dataset     | Predicted Negative     | Predicted Positive |
|--------------|-----------|------------|
| True Negative | 56863      |    14     |
| True Positive      | 30  | 55       |

|Scoring Metric | Value|
|--|--|
|Accuracy|0.9992275552122467|
|Precision |0.7971014492753623|
|Recall|0.6470588235294118|
|F1|0.7142857142857144|

While the model didn't score terribly, there's a lot of room for improvement, both for objective F1 score, and for business cost reductino.

I looped through multiple undersampling and threshold variables to construct a table of models models, but I can't find any way to objectively find the best recall/precision balance until I can find/calculate the costs of false negatives/positives in concrete numbers. This will be my top priority for the project.

## F1 Score of models with varying thresholds and undersampling
![Alt text](https://raw.githubusercontent.com/MK38993/Metis-Project-4---Classification/main/model_table.png "WHY BE THE [[Little Sponge]] WHO HATES ITS [[$4.99]] LIFE WHEN YOU CAN BE A [[BIG SHOT!!!!!]]")