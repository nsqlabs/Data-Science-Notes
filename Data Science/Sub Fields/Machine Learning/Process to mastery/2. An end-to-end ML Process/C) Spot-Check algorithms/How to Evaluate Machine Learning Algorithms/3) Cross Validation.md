A more sophisticated approach than using a test and train dataset is to use the entire transformed dataset to train and test a given algorithm. A method you could use in your test harness that does this is called cross validation.

It first involves separating the dataset into a number of equally sized groups of instances (called folds). The model is then trained on all folds exception one that was left out and the prepared model is tested on that left out fold. The process is repeated so that each fold get’s an opportunity at being left out and acting as the test dataset. Finally, the performance measures are averaged across all folds to estimate the capability of the algorithm on the problem.

<center style="background: white; padding: 20px">
	<img src="https://scikit-learn.org/stable/_images/grid_search_cross_validation.png" />
</center>

For example, a 3-fold cross validation would involve training and testing a model 3 times:

-   #1: Train on folds 1+2, test on fold 3
-   #2: Train on folds 1+3, test on fold 2
-   #3: Train on folds 2+3, test on fold 1

The number of folds can vary based on the size of your dataset, but common numbers are 3, 5, 7 and 10 folds. The goal is to have a good balance between the size and representation of data in your train and test sets.

When you’re just getting started, stick with a simple split of train and test data (such as 66%/34%) and move onto cross validation once you have more confidence.