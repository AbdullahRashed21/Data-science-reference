# Classification Evaluation Metrics Practice

1. Instead of using any built-in sklearn scoring methods, write your own accuracy, precision, recall, and F1 evaluation functions that take arrays of actual and predicted target labels as arguments. 
    * e.g.  `def accuracy(actuals, preds)`
2. Load the Wisconsin breast cancer data from sklearn (binary classification problem). See [here](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_breast_cancer.html) for documentation about the dataset and a demo of how to use it.  
Hint: Useful attributes are "data", "target", and "feature_names".  
3. Do a train/test split and fit a logistic regression and 10 nearest neighbors model. 
4. Use your functions to score your models on the test set.
5. Write your own function for generating an ROC curve plot from model predictions without using sklearn's assistance. Remember that ROC plots true positive rate (recall) vs. false positive rate for a given probability decision threshold. 
So you should loop over a range of probability cutoffs from 1 to 0, convert a model's predicted probabilities (`model.predict_proba()[:,1]`) to target labels using each cutoff, and plot the results as a curve.  
Hint: First create a function that calculates the false positive rate.