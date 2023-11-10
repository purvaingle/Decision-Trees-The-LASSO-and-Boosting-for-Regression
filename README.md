# I. Decision Trees as Interpretable Models
Dataset used:  the Accute Inflamations data from https://archive.ics.uci.edu/ml/datasets/Acute+Inflammations 

## Tasks performed: 

1. Built a decision tree on the whole data set and plotted it.
2. Converted the decision rules into a set of IF-THEN rules.
3. Used cost-complexity pruning to find a minimal decision tree and a set of decision
rules with high interpretability.

## II. The LASSO and Boosting for Regression
Dataset used: Communities and Crime data from https://archive.ics.uci.edu/ml/datasets/Communities+and+Crime. Used the first 1495 rows of data as the training set and the rest as the test set.

## Tasks performed:

1. I plotted a correlation matrix for the features in the dataset.

2. I calculated the Coefficient of Variation (CV) for each feature, using the formula CV = s/m, where s is the sample standard deviation and m is the sample mean.

3. I selected sqrt{128} features with the highest CV and created scatter plots and box plots for them. From the visualizations, I drew conclusions about the significance of those features.

4. I fitted a linear model using least squares to the training set and reported the test error.

5.  I fitted a ridge regression model on the training set, with lambda chosen by cross-validation, and reported the test error obtained.

6.  I fitted a LASSO model on the training set, selecting lambda through cross-validation. I then reported the test error and provided a list of the variables selected by the model.

7. Next, I repeated the process with standardized features. I reported the test error for both cases and compared the results.

8. Additionally, I fitted a PCR (Principal Component Regression) model on the training set, determining the number of principal components M through cross-validation. I then reported the test error obtained for this model.

9. In this section, I utilized an L1-penalized gradient boosting tree, also known as an L1 penalized gradient boosting tree, for regression tasks. This approach involves using L1-penalized regression at each node in the tree. I employed the XGBoost library to fit this model. To determine the appropriate value for \( \alpha \), the regularization term, I performed cross-validation.
