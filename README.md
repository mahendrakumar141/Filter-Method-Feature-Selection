# Filter-Method-Feature-Selection

Type of Feature Selection

Filter Method

Wrapper Method

Embedded Method

1.> Filter Method

Filter methods are generally used as a preprocessing step. The selection of features is independent of any machine learning algorithms. Instead, features are selected on the basis of their scores in various statistical tests for their correlation with the outcome variable.

1- BASIC METHOD_

A- Constant Features

Constant features are those that show the same value, just one value, for all the observations of the dataset. This is, the same value for all the rows of the dataset. These features provide no information that allows a machine learning model to discriminate or predict a target. Identifying and removing constant features. To identify constant features, we can use the VarianceThreshold function from sklearn.

B-Quasi-Constant Features

Quasi-constant features are those that show the same value for the great majority of the observations of the dataset. Mostly we do not consider these features in prediting the result. To identify Quasi constant features, we can use the VarianceThreshold function from sklearn. We will be using the same training set and test set.

C-Duplicated Features

Often datasets contain one or more features that show the same values across all the observations. This means that both features are in essence identical. In addition, it is not unusual to introduce duplicated features after performing one hot encoding of categorical variables, particularly when using several highly cardinal variables.
Note: Finding duplicated features is a computationally costly operation in Python, therefore depending on the size of your dataset, you might not always be able to perform it.

2- Fisher Score(chi2 test)


Measures the dependence of 2 variables

Suited for categorical variables.

Target should be binary.

Variable values should be non negative, typically Boolean or counts.



3-ANOVA (Analysis Of Variance)

Measures the dependency of two variables.

Suited for continuous variables.

Requires a binary target.

Assumes linear relationship between variable and target.

Assumes variables are normally distributed.

Sensitive to sample size


4-ROC-AUC / RMSE

Measures the dependency of two variables.

Suited for all type of variables.

Makes no assumption on the distribution of the variables.


