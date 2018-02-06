---
title: Review Questions
layout: page
---

### Lecture 1

1. What are 4 reasons to build a model?
2. p(x) = a/x for 1 < x < 10 describes a distribution pdf. What is a? What is the average of this distribution?
3. What are the three kinds of variables? Give an example of each.
4. You are interested in the sample distribution of the mean for an exponential distribution (N=8). What can you say about it relative to the original one?
5. What can you say about the sample distribution for the N=1 case?
6. Studying an anti-tumor compound, you breate two tumors in either flank (i.e. one mouse gets two tumors) of five mice, then treat the animals with compound measuring tumor growth. What is N? Justify your answer.
7. You want to model a process where each successive outcome is 1/3 as likely (i.e. getting 3 is 1/3 as likely as getting 2). Setup what this distribution would look like.

### Lecture 2

1. Are ordinary least squares or non-linear least squares guaranteed to find the solution?
2. How are new points predicted to be distributed in ordinary least squares?
3. How are new points predicted to be distributed in non-linear least squares?
4. How might you determine whether the assumptions you made when running OLS are valid? (Hint: think about the tests from lec 1)
5. What is a situation in which the assumptions of OLS can be valid but calculating a solution fails?
6. You're not sure a function you wrote to calculate the OLS estimator is working correctly. What could you check to ensure you have the right answer? (Hint: Lecture 2, slide 14)
7. You've made a monitor that you know provides a voltage proportional to blood glucose. Design a scheme for a model to convert from voltage to blood glucose, using some set of calibration points. What is the absolute minimum number of calibration points you'd need? How would you expect new calibration points to be distributed?

### Lecture 3

1. What is the bias-variance tradeoff? Why might we want to introduce bias into a model?
2. What is regularization? What are some reasons to use it?
3. What is the difference between ridge regression and LASSO? How should you choose between them?
4. Are you guaranteed to find the optimal answer for ridge regression? What about LASSO?
5. What is variable selection? Which method(s) perform it? What can you say about the answers?
6. What does it mean when one says ridge regression and LASSO give a family of answers?
7. What can we say about the relationship between *fitting* error and *prediction* error?
8. What does regularization do to the degrees of freedom (p) of a model? How about the number of measurements (n)?
9. A colleague tells you about a new form of regularization they've come up with (e.g. maximize the weighting for the variables most correlated with the output). How would this influence the variance of the model? Might this improve the prediction error?

### Lecture 4

1. Why does cross-validation need to be performed across multiple folds?
2. How will cross-validation influence the model fit error? How does it affect the model prediction error?
3. We want to demonstrate that we can predict the time until failure for an artificial heart from a set of clinical measurements. We plan to utilize LASSO regression to develop this prediction model, and are interested in the variables selected by LASSO. Walk through the steps to implement cross-validation here. How can you ensure you select only one set of variables?
4. List three ways in which cross-validation and bootstrap are similar.
5. List three ways in which cross-validation and bootstrap are different.
6. You are part of a team developing a model to predict incidence of hospital-aquired infection from clinical variables. You build a model on data collected from your hospital and are able to show great predictive capacity upon cross-validation. However, when applying the model from data within another hospital, you fail to predict any of the cases. What might lead to the discrepency here?
7. You want to determine whether the first parameter in your ordinary least squares model, beta_1, is significantly non-zero. How can you apply bootstrap to accomplish this?

### Lecture 5

1. What is a prior? How does one go about specifying one?
2. Can a prior be based on data? If so, how is this data related to the experiment being modeled?
3. What are three differences between a Bayesian and maximum likelihood (frequentist) approach?
4. When will a Bayesian and maximum likelihood approach agree?
5. You are asked to provide up-to-date estimates of the 6 month failure rate for a stent going to market. A previous device had 3 devices out of 100 fail within 6 months, and you strongly suspect this device is similar. Provide the Bayesian estimate of the failure rate (i.e. P(FR | N,m)) given N devices have made it to 6 months, and m have failed. (Hint: Devices EITHER pass or fail here.)
6. What would be a reasonable estimate if you had no previous device's data?
7. What do you expect to happen to a posterior distribution as you add more and more data?

### Lecture 6

1. Who/what sort of people need to test their code?
2. What is the difference between unit tests and integration tests?
3. What does testing guarantee?
4. What is the difference between testing and fuzzing?
5. What is linting?
6. You and a colleague are putting together a model. What are some factors that could influence the results besides the code that you write?

### Lecture 7

1. What do dimensionality reduction methods reduce? What is the tradeoff?
2. What are three benefits of dimensionality reduction?
3. Does matrix factorization have one answer? If not, what are two choices you could make?
4. What does principal components analysis aim to preserve?
5. What are the minimum and maximum number of principal components one can have for a dataset of 300 observations and 10 variables?
6. How can you determine the "right" number of PCs to use?
7. What is a loading matrix? What would be the dimensions of this matrix for the dataset in Q5 when using three PCs?
8. What is a scores matrix? What would be the dimensions of this matrix for the dataset in Q5 when using three PCs?
9. By definition, what is the direction of PC1?
10. See board. How does movement of the indicated point represent changes in the original data?

### Lecture 8

1. What are three differences between PCA and PLSR in implementation and application?
2. What is the difference between PCR and PLSR? When does this different matter more/less?
3. What does one need to do to one's data before applying PLSR?
4. How can you determine the right number of components for a model?
5. What feature of biological data make PLSR/PCR superior to direct regularization approaches (LASSO/ridge)?
6. What benefit does a two component model have over those with 3+ components?
7. Can you apply K-fold cross-validation to a PLSR model? If so, when do you scale your data?
8. Can you apply bootstrapping to a PLSR model? Describe what this would look like.
9. You use the same X data but want to predict a different Y variable. Do your X loadings change in your new model?
