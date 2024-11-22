# Using Machine Learning To Classify Credit Risk

## Overview of the Analysis
* In this project, I trained and evaluated a machine learning model that can identify the creditworthiness of borrowers. 
* The model was trained on a data set that included the lending activity from a peer-to-peer lending services company. This data included loan size, the interest rate, income of the borrower, debt to income ratio, number of accounts, derogatory marks, total debt, and loan status. Using this information, it was my goal to predict the loan status of borrowers.
* In order to do this, I first took divided the data into labels and features. The label, the loan status, is what I aimed to predict. The rest of the data was combined into the features and used to train the model. After dividing the data up, I used the `train_test_split` function to split the data into training and testing data. Then, using the training data, I used `LogisticRegression` to fit a logistic regression model, and then used that model to make predictions on the testing data. Finally, using `confusion_matrix` and `classification_report`, I evaluated the performance of the model.

## Results
* This model has a high rate of accuracy: 0.99%. The precision, recall, and f1-score for the healthly loan labels (0) were extremely high: 1.00, 0.99, and 1.00 respectively. The same scores for the high-risk loan labels (1) were lower: 0.84, 0.94, 0.89 respectively, but overall this model still did a very good job of predicting the correct labels.


## Summary
* Based on the results of this model, I would recommend it to a company for use in classifying the creditworthiness of borrowers. The accuracy of the model (99%) demonstrates that it is highly reliable. Furthermore, the model was able to correctly classify the healthy loan labels almost perfectly, which is more important to be able to predict for the company than the high-risk loan labels, because the cost of mistakenly classifying a high-risk borrower as healthy would be higher than the opposite. 