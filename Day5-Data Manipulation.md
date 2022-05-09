# Data Manipulation - Capital One
### Question: How to clean the data?
##### My Answers:
* Outlier: Remove. Sometimes, an outlier was caused by the measurement or recording errors. For example, the age was recorded as 200, which is impossible for a human being. Therefore, we'll remove this outlier.
* Missing Value: Replace or remove. Depends on the different data sets, I usually use the median, average or mode to replace the missing value. For example, if there's a missing value within the age column, then I'll calculate the average age and replace it with the missing value.
* Data Type: Sometimes, the categorical value will be regarded as a numerical value. For example, 1 means pass and 0 means failed. However, sometimes, 0 and 1 may be regarded as a numerical value, which may generate the different analysis and lead to bias. Therefore, we need to check the data type before we apply the algorithms.
* Data scaling: If we're gonna to use the algorithms like SVM or K-nearest neighbors, it is important that a change of "1" in any numeric feature is given the same importance. For example, we all know that the height and weight are in different unit. Therefore, we need to scale the the variables in order to compare different variables on equal footing.
* Data Normalization: Sometimes, our data needs to be normalized in order to apply a specific algorithm like t-tests, ANOVAs, linear regression, linear discriminant analysis and Gaussian naive Bayes. (Pro tip: any method with "Gaussian" in the name probably assumes normality.)

##### Credit to:
1. Kaggle Data Cleaning Challenge: https://www.kaggle.com/rtatman/data-cleaning-challenge-scale-and-normalize-data
2. http://www.1point3acres.com/bbs/forum.php?mod=viewthread&tid=423953&extra=page%3D1%26filter%3Dsortid%26sortid%3D311%26sortid%3D311
