# Sample Lesson Plan

- [Classification metrics PDF](classification_metrics_lecture.pdf)
- [Classification metrics notebook](classification_error_metrics_student.ipynb)

# Learning Objectives

Students will:
* Understand that accuracy is one (flawed) classification model metric
* Become comfortable with the confusion matrix
* Understand when to apply precision and recall, and in which types of cases we might care about one more than the other
* Understand the F1 score and how to apply it

# Additional Resources

* [Precision, recall, sensitivity, specificity](http://uberpython.wordpress.com/2012/01/01/precision-recall-sensitivity-and-specificity/)
 * [Wikipedia page on precision and recall](http://en.wikipedia.org/wiki/Precision_and_recall)
 * [Scikit learn on classification metrics](http://scikit-learn.org/stable/modules/model_evaluation.html#classification-metrics)
 * [Receiver Operating Characteristic](http://gim.unmc.edu/dxtests/roc2.htm)
 * [Area under curve (ROC)](http://gim.unmc.edu/dxtests/roc3.htm)


##### What is the relationship between F1 and Fß?

If you have found the [metrics function](http://scikit-learn.org/stable/modules/generated/sklearn.metrics.precision_recall_fscore_support.html) in `sklearn` that spits out your precision, recall, and F score, you might have found yourself asking: "What is Fß? Is it the same as F1?"

The answer is ... yes. F1 combines precision and recall. Fß does
the same thing, but uses a weight so that you can weigh one of these
two (precision or recall) more than the other when combining them. It
is a way to tune your score if you care more about precision than
recall, for example. F1 is the Fß for which ß = 1. In
`sklearn`, the default value for ß is 1.

The [wikipedia page](http://en.wikipedia.org/wiki/F1_score) has more on this relationship.
