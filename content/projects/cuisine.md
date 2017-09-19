+++
showonlyimage = false
draft = false
image = "img/projects/cooking.png"
date = "2017-09-10"
title = "Cuisine Classification"
description = "Different cuisines use different staple ingredients. This classification model labels recipes according to ingredients. The underlying techniques are bag of ingredients, logistic regression, and random forest."
type = "post"
weight = 1
+++

<!--more-->


The dataset is from a 2015 Kaggle competition [What's
Cooking](https://www.kaggle.com/c/whats-cooking). 
I participated in the competition 2 years ago without knowing much about machine
learning. It's nice to revisit the problem and improve my own models 2 years
later.

The winner in the contest has an accuracy of 0.83. My best submission has an
accuracy of 0.79, based on bag of ingredients, logistic regression, and random
forest.

### [Jupyter Notebook](/html/cuisine_classification.html)
### Table of Contents
* Preprocessing
* Idea 1: Bag of Words + Logistic Regression
* Feature Selection
  + Variance Threshold (unhelpful)
  + Mutual Information (unhelpful)
  + Chi2 (unhelpful)
  + Lasso Logistic Regression (helpful)
* Analyze the Weakness of Bag of Words + Logistic Regression
* Idea 2: Random Forest with Bag of Words and Logistic Regression Results as Features
* Idea 3: Random Forest for Confused Cuisine Pairs
  + French vs Italian
  + Modify Logistic Regression Predictions with French vs Italian Classifier
  + Random Forest for each Confused Cuisine Pair
  
#### Test Scores (Accuracy)
* Bag of Words + Random Forest: 0.679
* Idea 1 Bag of Words + Logistic Regression: 0.777
* Idea 2: 0.789
* Idea 3: 0.782
