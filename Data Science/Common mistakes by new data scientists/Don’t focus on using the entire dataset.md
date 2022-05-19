Sometimes as a data science aspirant, when you have to work on a data science project, you may be tempted to use the entire dataset provided. However, as already mentioned above, a dataset could have several imperfections, such as the presence of outliers, missing values, and redundant features. If the fraction of your dataset containing imperfections is really small, then you may simply eliminate the subset of imperfect data from your dataset. However, if the proportion of improper data is significant, then methods such as data imputation techniques could be used to approximate missing data.

Before implementing a machine learning algorithm, it is necessary to select only relevant features in the training dataset. The process of transforming a dataset in order to select only relevant features necessary for training is called dimensionality reduction. Feature selection and dimensionality reduction are important because of three main reasons:

**a) Prevents Overfitting**: A high-dimensional dataset having too many features can sometimes lead to overfitting (model captures both real and random effects).

**b) Simplicity**: An over-complex model having too many features can be hard to interpret, especially when features are correlated with each other.

**c) Computational Efficiency**: A model trained on a lower-dimensional dataset is computationally efficient (execution of algorithm requires less computational time).

For more information about dimensionality reduction techniques, please see the following articles:

-   [Feature Selection and Dimensionality Reduction Using Covariance Matrix Plot](https://medium.com/towards-artificial-intelligence/feature-selection-and-dimensionality-reduction-using-covariance-matrix-plot-b4c7498abd07)
-   [Machine Learning: Dimensionality Reduction via Principal Component Analysis](https://medium.com/towards-artificial-intelligence/machine-learning-dimensionality-reduction-via-principal-component-analysis-1bdc77462831)

Using dimensionality reduction techniques to remove unnecessary correlations between features could help improve the quality and predictive power of your machine learning model.