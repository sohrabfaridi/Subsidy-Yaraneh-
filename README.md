# Subsidy-Yaraneh-
<p>
My data is related with some properties of households in States: Hamedan, Qom, Qazvin, Alborz.
The goal is not to subsidize the households which are in 3 decile of richer households. So this means predicting True positive is more important.
</p>
<p>
After doing some visualization and preprocessing, I splitted data in two set: train and test and I did crossvalidation over all models and used test set just one time after selecting the best model.<br> 
For this binary classification I tried diffrent machine learning algorithms: KNeighbors , Logistic Regression, SVM , Decision Tree, Random Forest, Gradient Boosting.<br>
Since our data is a little imbalanced and predicting True positive is important acuuracy score was not useful so I selected : "average-precision" to evaluate models. And at last after selecting best model, for selecting best threshold, The best way was to compare "macro-averages" on train-set.<br>
And for the last step after picking model and best threshold all without using test-set, The model will be evaluate on the test set.
</p>
