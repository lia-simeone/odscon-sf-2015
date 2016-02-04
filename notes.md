Pickle, by default, always uses the oldest version which will generate new files

Fit, predict, and score methods can be used for all of the models in sklearn

You can visualize trees using sklearn, but can't "examine" the model by looking at specific splits (per a question)

Linear SVM - look at the coefficients to evaluate, for GBM use feature importance

They're working on the ability to search across model types. He says 1 year.

He removed the mean and scaled the variance before using an unsupervised method (PCA). He said it's also good for SVM. 
He does **not** recommend scaling the data before splitting on test and train. It can contaminate the data.

If you have a very imbalanced dataset (he suggests less than 10%), you should use stratified cross validation. 
This will make sure the ratio of each class is the same in each sample as the overall ratio.
If you data is sorted, you should use shuffle. Otherwise it splits the data in order!!!!

The default score showed depends on the model. Regression shows R^2 and GBM shows Accuracy.

Accuracy is a poor evaluator when the classes are very imbalanced.

Kernels for grid search?

Ideally, you shouldn't do parameter search and then add or change the features
Feature selection should be part of the cross validation

"You should set up your infrastructure so building models is free"

You can use pipelines to do cross validation on each step in a pipeline. You can also do gridsearch.
The example he shows is standarizing data before using SVM. 

He has a video series on machine learning. And is writing a book.
Andrea Mueller.
