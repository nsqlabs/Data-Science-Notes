Not all features are created equal.

Those attributes that are irrelevant to the problem need to be removed. There will be some features that will be more important than others to the model accuracy. There will also be features that will be redundant in the context of other features.

[Feature selection](https://en.wikipedia.org/wiki/Feature_selection) addresses these problems by **automatically selecting a subset that are most useful to the problem.**

Feature selection algorithms may use **a scoring method to rank and choose features, such as correlation or other feature importance methods.**

More advanced methods **may search subsets of features by trial and error, creating and evaluating models automatically in pursuit of the objectively most predictive sub-group of features.**

There are also methods that bake in feature selection or get it as a side effect of the model. **Stepwise regression is an example of an algorithm that automatically performs feature selection as part of the model construction process.**

Regularization methods like LASSO and ridge regression may also be considered algorithms with feature selection baked in, as they actively seek to remove or discount the contribution of features as part of the model building process.