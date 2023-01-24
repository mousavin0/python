# python

## Titanic Dataset
The goal is to fit a classification model that can predict if a passenger survive or not based on some information provided.
The following models are tried: Logistic regression, SVM, SGD, KNN, Decision Tree, Gradient Boosting, Random Forest and Naive Bayes,
Hyper parameter tuning is performed using GridSearchCV and when needed pipline is used to perform feature Scaling. 
Best performance is acheived by Gradient Boositng with the test accuracy of 0.83.

## British Airways
First British Airways reviews (review, header, rank) are collected by scraping the web page: 'https://www.airlinequality.com/airline-reviews/british-airways'.
The ranks are used to construct a 'positive' or 'negative' sentiment label for the reviews.
A word cloud is made for each of the cateogires.

![alt text](https://github.com/mousavin0/python/blob/main/British%20Airways/bild.png)


Finally a neural network (RNN based) is used to predict the sentiment. It works with 100% test accuracy.


