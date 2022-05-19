It is a big problem for data scientists when a model works well on training data but it doesn’t fit unseen/new data. This might be a problem of [overfitting](https://elitedatascience.com/overfitting-in-machine-learning) or underfitting, poor predictions, and poor performance.

These problems happen due to a lack of model validation. Model validation means validating your model on some part of training data which is not being used for training. With the model validation approach, a data scientist can validate model accuracy and optimize the model accordingly to reach its peak potential.

Validation helps reach a balanced training model as shown in the image above.

There are two ways to approach model validation: cross-validation and hyperparameter tuning. Model validation consistency has a crucial impact on the results and helps maintain a [bias-variance tradeoff](https://en.wikipedia.org/wiki/Bias%E2%80%93variance_tradeoff), which is an important property of the model.