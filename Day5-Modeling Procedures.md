# The procedures of applying algorithms to do the prediction
### Step1: Clean data
* Fix: outliers, missing values
* Data type: consistent data entry (categorical v.s. numerical)
* Manipulation: data scaling, normalization, transformation
* Be aware if the data has multicollinearity --> do factor analysis (Study this part), VIF, Tolerance, Correlation matrix

### Step2: Decide which algorithms to use
* For example, we may apply the linear regression to the numerical output variables. For the categorical output variables, we often use the logistic regression or random forest. For count data, we can use the Poisson model.
* Be aware of the assumption of each algorithm. For example, the data should be in the normal distribution if you decide to use t-test, ANOVA, linear regression, etc.

### Step3: Split data
* train (80%) v.s. test (20%)
* Be aware of the unbalanced data while splitting -> oversampling the smaller class or undersampling the larger class
* Sometimes, we'll use the validation set as well (Study this part & cross validation)

### Step4: Apply the model to train set
* See the model performance using something like the confusion matrix, AUC, ROC curve, precision, recall, F1, etc. (Study this part)
* Identify the importance of features -> Do feature selection, clustering, PCA for dimensionality reduction, etc. (Study this part)
* Identify if the model is solid or not e.g. residual analysis, QQ plot (Study this part)
* If we have an assumption/hypothesis, use the test statistics like t-test/f-test to see if the result rejects the null hypothesis.

### Step5: Apply the model to the test set after we build up the model
* See the performance (usually is lower than the performance in Step4. Otherwise, it may be overfitting if the AUC in test set is greater than the AUC in the train set)
* Interpretation of the final results e.g. confidence interval, coefficient, R-squared and adjusted R-squared, p-value
