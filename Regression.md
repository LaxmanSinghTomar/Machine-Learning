# Regression

## What is Regression Analysis?
Regression analysis is a set of statistical processes that estimate the relationship between the independent and dependent variables. The most common approach is
to estimate the conditional expectation of the dependent variable given the independent variables (based on the assumption that the independent variables are
linearly independent).

## Relationship between Regression Analysis & Supervised Learning
Regression comes under the Supervised Learning category because it learns the model from the labeled dataset to predict the value of the continuous variables.

## Popular Regression Techniques
1. **Linear Regression:** Fits a straight line to explain the relationship between independent & dependent variables. Used when the dependent variable is continuous.

2. **Logistic Regression:** Finds the probability of success. Used when the dependent variable is binary.

3. **Polynomial Regression:** Fits the curve between independent & dependent variables, where the dependent variable is a polynomial function of the independent variable.

## Bias-Variance Trade-off
Predictive models suffers from the bias(how well does the model fit the data) and variance(how much does the model change when the input changes).
Simpler Models are stable(low variance) but don't get close to the truth(high bias).
Complex Models are prone to overfitting(high variance) but expressive enough to get close to the truth(low bias).

We look to find the sweet-spot somewhere in the middle.

## Low-bias and High-variance; what to do?
As we read above, low bias implies that model's predicted values are closer to the true/actual values i.e. model is flexible enough to mimic the training distribution. But the real problem starts here, as the better a model is mimicking a training distribution more poor;y it generalizes i.e. poor performance on unseen data.

In such situations, you can make use of Bagging Algorithms(like Random Forests) to tackle high variance problems. What it does is, it divides a dataset into subsets made with repeated sampling. Then, using these samples, we generate a set of models using a single-learning algorithm. Later, using voting(in case of classification) or averaging(in case of regression) we can combine the model predictions.

If you're looking to overcome the issue of high-variance, you can:
  - Use Regularization Techniques, where the higher model coefficients get penalized and henceforth it reduces the model complexity.
  - Use only top "n" features from the variable importance chart.(Variable Importance is the statistical significance of each variable/feature in the data w.r.t. to it's effect on the generated model.
  
 When we have all the variables in the dataset, filtering the meaningful signal from the data is difficult for the algorithm.
 
 ## Low-bias and High-variance, useful when?
 Low-bias and High-variance can be used in K-Nearest Neighbors. It doesn't assume anything special about the distribution of the data at hand hence has low bias, and can easily change the prediction when training set changes resulting into high-variance.
 
 ## Interpretation from Coefficient Estimates
 Regression has the following equation:

