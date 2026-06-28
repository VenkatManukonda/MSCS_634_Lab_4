# MSCS_634_Lab_4

## Purpose

The goal of this lab was to compare several regression techniques using the Diabetes dataset and understand how increasing model complexity and regularization influence prediction performance. Instead of focusing only on which model produced the highest score, I wanted to see how each approach behaved, how well it generalized to unseen data, and how regularization could reduce the risk of overfitting.

## What I Observed

The first thing that stood out was the difference between the simple and multiple regression models. Using a single feature provided a reasonable baseline, but the predictions were noticeably less accurate than those from the model that used all available features. This reinforced the idea that disease progression depends on multiple health measures rather than a single factor.

Polynomial regression produced another interesting result. Increasing the polynomial degree improved the model's ability to fit the training data, but after a certain point, the improvement on the test data became much smaller and could even decline. Comparing training and test results made it much easier to recognize signs of overfitting, rather than assuming that a more complex model is automatically better.

Ridge and Lasso regression demonstrated how regularization changes model behavior. Smaller alpha values behaved similarly to ordinary linear regression, while larger alpha values placed stronger constraints on the model. Ridge generally maintained stable performance by shrinking the coefficients, whereas Lasso simplified the model by reducing the influence of less important features. Testing several alpha values made these differences much easier to understand.

## What I Learned

One of the biggest lessons from this lab is that evaluating regression models requires more than looking at a single metric. MAE, MSE, RMSE, and R² each describe performance from a different perspective, and considering them together provides a more complete picture of prediction quality.

I also gained a better appreciation for the balance between model complexity and generalization. More flexible models can fit the training data very well, but that does not always translate into better performance on unseen data. Regularization offers a practical way to control that complexity without discarding useful information.

## Challenges and Decisions

The main challenge was comparing several regression models fairly while maintaining consistent evaluation. Using the same train-test split and the same evaluation metrics for every model made the comparison more meaningful.

Another decision was to evaluate several polynomial degrees and multiple alpha values, rather than relying on a single configuration. This provided a clearer picture of how model complexity and regularization affect performance and made it easier to identify where overfitting began to appear.

Overall, this lab showed that selecting the best regression model involves balancing prediction accuracy, model complexity, and generalization to new data. While some models performed better than others, the comparison showed that the most reliable model is the one that performs consistently rather than simply fitting the training data as closely as possible.
