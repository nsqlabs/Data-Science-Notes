
Parameters (known as hyperparameters) are **values that control the learning process and determine the values of model parameters that a learning algorithm ends up learning during the [[What is fitting|fitting process]].** The prefix ‘hyper_’ suggests that they are ‘top-level’ parameters that control the learning process and the model parameters that result from it.

```ad-caution
As a machine learning engineer designing a model, you choose and set hyperparameter values that your learning algorithm will use before the training of the model even begins. In this light, hyperparameters are said to be external to the model because the model cannot change its values during learning/training.
```

Hyperparameters are used by the learning algorithm when it is [[What is fitting|learning]] but they are not part of the resulting model. At the end of the learning process, we have the trained model parameters which effectively is what we refer to as the model.

```ad-warning
The hyperparameters that were used during training are not part of this model. We cannot for instance know what hyperparameter values were used to train a model from the model itself, we only know the model parameters that were learned.
```

Each model has totally different parameters.