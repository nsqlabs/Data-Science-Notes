![](https://www.datarobot.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-22-at-11.22.15-AM-e1527613915658.png)

Overfitting happens when a [machine learning](https://www.datarobot.com/wiki/machine-learning/) [model](https://www.datarobot.com/wiki/model/) has become too attuned to the data on which it was trained and therefore loses its applicability to any other dataset. A model is overfitted when it is so specific to the original data that trying to apply it to data collected in the future would result in problematic or erroneous outcomes and therefore less-than-optimal decisions.

```ad-warning

The overfitted model is not going to be useful unless we apply it to the exact same dataset because no other data will fall exactly along the overfitted line.

```

## Why is Overfitting Important?

Overfitting causes the model to misrepresent the data from which it learned. An overfitted model will be less accurate on new, similar data than a model which is more generally fitted, but the overfitted one will appear to have a higher accuracy when you apply it to the training data.

```ad-danger
With no protection against overfitting, model developers might train and deploy a model they think is highly accurate, when in fact it will underperform in production when given new data.
```

Deploying an overfitted model can cause all kinds of problems. For example, if you think your model is 95% accurate in predicting the likelihood of loan default when in reality it is overfitted and has an accuracy somewhere closer to 60%, applying it to future loan decisions will result in the loss of business that would otherwise have been profitable and will result in more dissatisfied customers.