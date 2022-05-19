A machine learning model is typically specified with some functional form that includes parameters.

An example is a line intended to model data that has an outcome variable `y` that can be described in terms of a feature `x`. In that case, the functional form would be:

$$
y = mx + b
$$

_fitting_ the model means finding values for `m` and `b` that are in accordance with training data, which is a set of points `(x1, y1)`, `(x2, y2)`, ..., `(xN, yN)`. It may not be possible to set `m` and `b` such that the line passes through all training data points, but some _loss function_ could be defined for describing a well-fit line. The _fitting_ algorithm's purpose would be to minimize that loss function. In the case of line fitting, the loss could be the total distance of training data points to the line, but it may be more mathematically convenient to set the loss to the total _squared distance_ of training data points to the line.

In general, a model can be more complex than a line and include many parameters. For some models, the number of parameters is not fixed and can change as part of the _fitting_ process. The features and the outcome variable can be discrete, continuous, and/or multidimensional. For _unsupervised_ problems, there is no outcome variable.

In all these cases, _fitting_ is still analogous to the line example above, where an algorithm is run to find model parameters that in some sense explain the training data. This often involves running some optimization procedure.

A model that is well-fit to the training data may not be well-fit to other non-training data, even if the other data is sampled from the same distribution as the training data. A technique called regularization can be used to address this issue.

![](https://www.researchgate.net/profile/Prasanna-Date/publication/343498508/figure/fig1/AS:921736623190020@1596770544633/Fitting-a-linear-regression-model-green-line-to-data-blue-dots.ppm)