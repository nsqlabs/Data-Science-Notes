A solution to the problem of ensuring each instance is used for training and testing an equal number of times while reducing the variance of an accuracy score is to use [cross validation](https://en.wikipedia.org/wiki/Cross-validation_(statistics)). Specifically k-fold cross validation, where k is the number of splits to make in the dataset.

<center style="background: white; padding: 20px">
	<img src="https://scikit-learn.org/stable/_images/grid_search_cross_validation.png" />
</center>

```ad-example
title: Choosing k folds
For example, let’s choose a value of k=10 (very common). This will split the dataset into 10 parts (10 folds) and the algorithm will be run 10 times. Each time the algorithm is run, it will be trained on 90% of the data and tested on 10%, and each run of the algorithm will change which 10% of the data the algorithm is tested on.

In this example, each data instance will be used as a training instance exactly 9 times and as a test instance 1 time. The accuracy will not be a mean and a standard deviation, but instead will be an exact accuracy score of how many correct predictions were made.
```

==The k-fold cross validation method is the go-to method for evaluating the performance of an algorithm on a dataset. You want to choose k-values that give you a good sized training and test dataset for your algorithm. Not too disproportionate (too large or small for training or test). If you have a lot of data, you may may have to resort to either sampling the data or reverting to a split test.


> [!caution] Not everything is perfect
> Cross validation does give an unbiased estimation of the algorithms performance on unseen data, but <mark style="background: orange; color: black">what if the algorithm itself uses randomness. The algorithm would produce different results for the same training data each time it was trained with a different random number seed (start of the sequence of pseudo-randomness).?</mark> **Cross validation does not account for variance in the algorithm’s predictions!**

> [!caution] 
>Another point of concern is that cross validation itself uses randomness to decide how to split the dataset into k folds. Cross validation does not estimate how the algorithm perform with different sets of folds.


This only matters if you want to understand how robust the algorithm is on the dataset.

## Multiple Cross Validation

> [!seealso] A partial solution
>**A way to account for the variance in the algorithm itself is to run cross validation multiple times and take the mean and the standard deviation of the algorithm accuracy from each run.**

This will will give you an an estimate of the performance of the algorithm on the dataset and an estimation of how robust (the size of the standard deviation) the performance is.

If you have one mean and standard deviation for algorithm A and another mean and standard deviation for algorithm B and they differ (for example, algorithm A has a higher accuracy), how do you know if the difference is meaningful?

This only matters if you want to compare the results between algorithms.