# Subsidy-Yaraneh-
My data is related with some properties of households in States: Hamedan, Qom, Qazvin, Alborz.
The goal is not to subsidize the households which are in 3 decile of richer households. So this means predicting True positive is more important.
After doing some visualization and preprocessing, I splitted data in two set: train and test and I did crossvalidation over all models and I used test set just one time after I selected the best model. 
For this binary classification i tried diffrent machine learning algorithms: KNeighbors , Logistic Regression, SVM , Decision Tree, Random Forest, Gradient Boosting.
Since our data is a little imbalanced and predicting True positive is important acuuracy score was not useful so I selected : "average-precision" to evaluate models. And at last after selecting best model, for selecting best threshold, The best way was to compare "macro-averages" on train-set
And for the last step after picking model and best threshold all without using test-set, The model will be evaluate on the test set.
