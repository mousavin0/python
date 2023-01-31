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

<p align="center">
 <img src='https://github.com/mousavin0/python/blob/main/British%20Airways/bild.png'>
<\p>


A neural network (RNN based) is used to predict the sentiment from the short headers of the reviews. It works with 100% test accuracy.

Moreover, using a customer booking dataset, we have made a predictive model for whether customers complete their purchase. First we looked at the relative frequency of completed purchases.


<p align="center">
 <img src='https://github.com/mousavin0/python/blob/main/British%20Airways/piechart.jpg'>
<\p>

Based on above, there is little balance among groups. Therefore, a classifier that always predict 'not completed' would have accuracy of 85 percent. We therefore chose to resample from the 'not completed' group by replacement to make a new dataset where both group have the same size and then fitted a random forest classifier. The resulting model fit has 96 percent accuracy on a test data. See the confusion matrix below.

<p align="center">
 <img src='https://github.com/mousavin0/python/blob/main/British%20Airways/confusion_matrix.jpg'>
<\p>

Moreover, a feature importance plot of the model look as below:

<p align="center">
 <img src='https://github.com/mousavin0/python/blob/main/British%20Airways/feature_importance.jpg'>
<\p>
