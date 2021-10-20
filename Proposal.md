# Metis Project 4: Classification - PROPOSAL
 
### Question/need:
While not an original problem, credit card fraud has been an issue almost as long as credit cards have existed. According to the [Nilson Report](https://www.prnewswire.com/news-releases/payment-card-fraud-losses-reach-27-85-billion-300963232.html) released in 2019, $27.85 billion was stolen by fraudsters in 2018, and this figure has only grown since then.

Machine learning can help solve this problem by flagging potentially suspicious transactions, allowing credit card companies to contact customers before further fraudulent transactions occur.

### Data Description:
The dataset contains 284,807 transactions, each with 30 features, as well as a flag indicating whether a transaction was fraudulent or not.

Unfortunately, due to privacy concerns, 28 of these features are composite metrics calculated from multiple real features, so interpretation will be more difficult with only the "Time" and "Transaction Amount" features interpretable.

That said, fraud detection models are often black-box programs that don't require much interpretability, so my focus will be on minimizing the costs of false-positives/negatives.

### Tools:
I'll be using Python and its Pandas library for data ingestion/cleaning, and Scikit-Learn for classification modeling. As usual, Matplotlib and Seaborn will be used for data visualization.

