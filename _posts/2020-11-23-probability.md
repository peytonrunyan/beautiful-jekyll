---
layout: post
title: Probability Resources
subtitle: Fundamentals of Probability
# gh-repo: daattali/beautiful-jekyll
gh-badge: [star, fork, follow]
tags: [test]
comments: true
---

## Resources

[Discussion on Bayes](https://www.sciencedirect.com/topics/computer-science/prior-probability)

[Quick Rundown of Joint, Marginal, and Conditional Probability](https://sites.nicholas.duke.edu/statsreview/jmc/)

[Machine Learning Mastery Intro to Bayes](https://machinelearningmastery.com/bayes-theorem-for-machine-learning/)

[Understanding Bayes: A Look the Likelihood](https://alexanderetz.com/2015/04/15/understanding-bayes-a-look-at-the-likelihood/)

[Probability concepts explained: Bayesian inference for parameter estimation](https://towardsdatascience.com/probability-concepts-explained-bayesian-inference-for-parameter-estimation-90e8930e5348)

[Maximum Likelihood Estimation](https://towardsdatascience.com/probability-concepts-explained-maximum-likelihood-estimation-c7b4342fdbb1)

## **Concepts:**

Assume that *Y* is our outcome and *X* is our input data. We can think of *X* as our *evidence* for a predicting an outcome. 

### **Prior - P(Y)**

This is the probability of an outcome given the dataset. 
* If we have a mix of 100 dogs and 17 of them are large, our prior probability that the dog is large is 17/100
* If 2% of home loans default, then our prior for P(home loan default) is 0.2

### **Posterior (also called the Conditional Probability) - P(Y|X)**

It can be easier to think of the conditional probability in terms of a machine learning model. 

Imagine a logistic regression model that predicts whether or not a home will sell in the next 3 months based on the price of the house, the square footage, and the average price of a home in the area. That X (input) data is our evidence. The target is our Y. Our model makes a prediction about the probability of the home selling based on the input data.

In other words, our model provides us the conditional probability of outcome *Y* given evidence *X*. Stated another way, this model provides us with *P(Y|X)*.

### **Likelihood- P(X|Y)**

In the case of estimating parameters, P(X|theta) we can think of it as the probability of observing our data if the parameter theta was the actual parameter describing the distribution.

So why is it called likelihood? This is because P(X|theta) is equal to L(theta|X). In other words, the likelihood of a paramter given the observed data is equal to the probability of observing the data given the parameter. 