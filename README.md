MUSHROOM CLASSIFICATION:-
The given data about the mushrooms was analysed.The aim was to build a model so as to correctly classify any mushrooom as poisonous(1) or edible(0) by learning from the given training data.It conatined 25 columns consisting of one Target variable(Class) and 24 features.
The feature column veil-type was deleted since it had only one value for all the trainig samples.
There were some missing values in the feature column stalk-root.Since it was a categorical variable; so they were assigned a unique and user-defined category as '?'.
VISUALISATIONS and INFERENCES followed next which included Univariate and Bivariate analysis of the features.On visualising the features radius and weight; OUTLIERS were detected.
Since i have used Decision Trees to perform the given Classification task , hence there was no need to specially deal with the outliers because tree based models do well even in the presence of outliers.
FEATURE CREATION and Feature scaling followed next. A new feature named "ratio"(weight/radius) was created by taking the ratio of features "weight" and "radius".
The new feature created("ratio") had much higher correlation with the target variable as compared to the feature "weight".
Finally after DATA PREPROCESSING and FEATURE GENERATION ; Decision Tree model was implemented.
Decision Tree Classifier was impelmented by performing 5-Fold Cross validation for tuning the parameter max_depth of the tree so as to avoid Overfitting.
At the end ; predictions were made on the Test data using the Decision Tree Model learned on the Training data and were stored in the final named predictions.csv 
