```ad-hint
You can objectively estimate the usefulness of features.
```

This can be helpful as a pre-cursor to selecting features. <mark style="background: #FF5582A6;">Features are allocated scores and can then be ranked by their scores. Those features with the highest scores can be selected for inclusion in the training dataset, whereas those remaining can be ignored.</mark> 

<mark style="background: #FF5582A6;">Feature importance scores can also provide you with information that you can use to extract or construct new features, similar but different to those that have been estimated to be useful.</mark> 

**A feature may be important if it is highly correlated with the dependent variable** (the thing being predicted). Correlation coefficients and other univariate (each attribute is considered independently) methods are common methods.


```ad-abstract
More complex predictive modeling algorithms perform feature importance and selection internally while constructing their model. Some examples include MARS, [Random Forest](https://en.wikipedia.org/wiki/Random_forest#Variable_importance) and Gradient Boosted Machines. These models can also report on the variable importance determined during the model preparation process.
```