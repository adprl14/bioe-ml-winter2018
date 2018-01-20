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
