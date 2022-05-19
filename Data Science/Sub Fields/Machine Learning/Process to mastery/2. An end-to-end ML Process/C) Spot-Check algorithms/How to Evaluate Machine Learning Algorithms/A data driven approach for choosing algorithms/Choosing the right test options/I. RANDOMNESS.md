The root of the difficulty in choosing the right test options is randomness. Most (almost all) machine learning algorithms use randomness in some way. The randomness may be explicit in the algorithm or may be in the sample of the data selected to train the algorithm.

![Randomness](https://machinelearningmastery.com/wp-content/uploads/2014/02/randomness-300x200.jpg)


This does not mean that the algorithms produce random results, it means that they produce results with some noise or [variance](https://en.wikipedia.org/wiki/Variance). We call this type of limited variance, stochastic and the algorithms that exploit it, [stochastic algorithms](https://en.wikipedia.org/wiki/Stochastic_process).

## Train and Test on Same Data

If you have a dataset, you may want to train the model on the dataset and then report the results of the model on that dataset. That’s how good the model is, right?

**The problem with this approach of evaluating algorithms is that you indeed will know the performance of the algorithm on the dataset, but do not have any indication of how the algorithm will perform on data that the model was not trained on (so-called unseen data).**

This matters, only if you want to use the model to make predictions on unseen data.

## Split Test

**A simple way to use one dataset to both train and estimate the performance of the algorithm on unseen data is to split the dataset. You take the dataset, and split it into a training dataset and a test dataset.** For example, you randomly select 66% of the instances for training and use the remaining 34% as a test dataset.

The algorithm is run on the training dataset and a model is created and assessed on the test dataset and you get a performance accuracy, lets say 87% classification accuracy.

Spit tests are fast and great when you have a lot of data or when training a model is expensive (it resources or time). A split test on a very very large dataset can produce an accurate estimate of the actual performance of the algorithm.

How good is the algorithm on the data? Can we confidently say it can achieve an accuracy of 87%?

```ad-caution
A problem is that if we spit the training dataset again into a different 66%/34% split, we would get a different result from our algorithm. This is called model variance.
```

## Multiple Split Tests

A solution to our problem with the split test getting different results on different splits of the dataset is to reduce the variance of the random process and do it many times. We can collect the results from a fair number of runs (say 10) and take the average.

```ad-example
For example, let’s say we split our dataset 66%/34%, ran our algorithm and got an accuracy and we did this 10 times with 10 different splits. We might have 10 accuracy scores as follows: 87, 87, 88, 89, 88, 86, 88, 87, 88, 87.

> The average performance of our model is 87.5, with a standard deviation of about 0.85.
```

```ad-danger
A problem with multiple split tests is that it is possible that some data instance are never included for training or testing, where as others may be selected multiple times. The effect is that this may skew results and may not give an meaningful idea of the accuracy of the algorithm.
```