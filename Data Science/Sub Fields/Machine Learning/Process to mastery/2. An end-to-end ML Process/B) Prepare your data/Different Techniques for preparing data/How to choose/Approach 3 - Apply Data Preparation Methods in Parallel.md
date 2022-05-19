Like the [[Approach 2 - Grid Search Data Preparation Methods|previous approach]], with this approach, **assumes that algorithms have expectations and requirements, and it also allows for good solutions to be found that violate those expectations, although it goes one step further.**

This approach **also acknowledges that a model fit on multiple perspectives on the same data may be beneficial over a model that is fit on a single perspective of the data.**

```ad-abstract
This is achieved by **performing multiple data transforms on the raw dataset in parallel, then gathering the results from all transforms together into one large dataset with hundreds or even thousands of input features** (i.e. the [FeatureUnion class](https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.FeatureUnion.html) in scikit-learn can be used to achieve this). 
```

**It allows for good input features found from different transforms to be used in parallel.**

```ad-warning
The number of input features may explode dramatically for each transform that is used. Therefore, it is good to combine this approach with a feature selection method to select a subset of the features that is most relevant to the target variable. Again, this may involve the application of one, two, or more different feature selection techniques to provide a larger than normal subset of useful features.
```

Alternatively, a dimensionality reduction technique (e.g. [PCA](https://machinelearningmastery.com/principal-components-analysis-for-dimensionality-reduction-in-python/)) can be used on the generated features, or an algorithm that performs automatic feature selection (e.g. [random forest](https://machinelearningmastery.com/random-forest-ensemble-in-python/)) can be trained on the generated features directly.

<mark style="background: #FF5582A6;">I like to think of it as an explicit feature engineering approach where we generate all the features we can possibly think of from the raw data, unpacking distributions and relationships in the data. Then select a subset of the most relevant features and fit model. Because we are explicitly using data transforms to unpack the complexity of the problem into parallel features, it may allow the use of a much simpler predictive model, such as a linear model with a strong penalty to help it ignore less useful features.</mark> 

**A variation on this approach would be to fit a different model on each transform of the raw dataset and use an ensemble model to combine the predictions from each of the models.**

```ad-success
A benefit of this general approach is that it allows a model to harness multiple different perspectives or views on the same raw data, a feature that the other two approaches discussed above lack. This may allow extra predictive skill to be squeezed from the dataset. 
```
```ad-failure
A downside of this approach is the increased computational cost, and the careful choice of the feature selection technique, and/or model used to interpret such a large number of input features.
```