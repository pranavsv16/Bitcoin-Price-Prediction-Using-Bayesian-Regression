# Bitcoin-Price-Prediction-Using-Bayesian-Regression
Predicting Bitcoin Price Variations using Bayesian Regression

In this project, the task is predicting the price variations of bitcoin, a virtual cryptographic currency. These predictions could be used as the foundation of a bitcoin trading strategy. To make these predictions, we will use Bayesian Regression, and implement this technique in Python.

### Dataset

The datasets have three attributes: (1) time in epoch, (2) price in USD per bitcoin, and (3) bitcoin amount in a transaction (buy/sell). However, only the first two attributes are relevant to this project.

To make the data to have evenly space records, all the records within a 20 second window are taken and replaced it by a single record as the average of all the transaction prices in that window. Not every 20 second window had a record; therefore those missing entries were filled using the prices of the previous 20 observations and assuming a Gaussian distribution. The raw data that has been cleaned is given in the file dataset.csv.
