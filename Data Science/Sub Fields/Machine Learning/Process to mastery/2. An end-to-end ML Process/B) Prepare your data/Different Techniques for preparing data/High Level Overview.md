# Data Preparation for Rows

```ad-abstract
title: Definition
This group is for data preparation techniques that add or remove rows of data. In machine learning, rows are often referred to as samples, examples, or instances.
```

These techniques are often used to augment a limited training dataset or to remove errors or ambiguity from the dataset. The main class of techniques that come to mind are data preparation techniques that are often used for imbalanced classification

- This includes techniques such as [SMOTE](https://machinelearningmastery.com/smote-oversampling-for-imbalanced-classification/) that create synthetic rows of training data for under-represented classes and random undersampling that remove examples for over-represented classes.
- It also includes more advanced combined [over- and undersampling techniques](https://machinelearningmastery.com/combine-oversampling-and-undersampling-for-imbalanced-classification/) that attempt to identify and remove ambiguous examples along the decision boundary of a classification problem and remove them or change their class label.
- This class of data preparation techniques also includes [algorithms for identifying and removing outliers from the data](https://machinelearningmastery.com/how-to-use-statistics-to-identify-outliers-in-data/). These are rows of data that may be far from the center of probability mass in the dataset and, in turn, may be unrepresentative of the data from the domain.

# Data Preparation for Columns

```ad-abstract
title: Definition
This group is for data preparation techniques that add or remove columns of data. 
In machine learning, columns are often referred to as variables or features. 
These techniques are often required to either reduce the complexity (dimensionality) of a prediction problem or to unpack compound input variables or complex interactions between features.
```

The main class of techniques that come to mind are **feature selection techniques.**

- This includes techniques that **use statistics to [score the relevance of input variables](https://machinelearningmastery.com/feature-selection-with-real-and-categorical-data/) to the target variable based on the data type of each.**
- This also includes feature selection techniques that [systematically test the impact of different combinations of input variables on the predictive skill of a machine learning model.](https://machinelearningmastery.com/rfe-feature-selection-in-python/)
- Related are techniques that [use a model to score the importance of input features based on their use by a predictive model, referred to as feature importance methods. ](https://machinelearningmastery.com/calculate-feature-importance-with-python/) These methods are often used for data interpretation, although they can also be used for feature selection.
- This group of methods also brings to mind [techniques for creating or deriving new columns of data, new features.](https://machinelearningmastery.com/polynomial-features-transforms-for-machine-learning/) These are often referred to as feature engineering, although sometimes the whole field of data preparation is referred to as feature engineering. 
	- For example, new features that represent values raised to exponents or multiplicative combinations of features can be created and added to the dataset as new columns.
- This might also include data transforms that change a variable type, such as creating dummy variables for a categorical variable, often referred to as a [one-hot encoding.](https://machinelearningmastery.com/one-hot-encoding-for-categorical-data/)
# Data preparation for values

```ad-abstract
title: Definition

This group is for data preparation techniques that change the raw values in the data. These techniques are often required to meet the expectations or requirements of specific machine learning algorithms.
```

The main class of techniques that come to mind is data transforms that change the scale or distribution of input variables.

- For example, data transforms such as [standardization and normalization](https://machinelearningmastery.com/standardscaler-and-minmaxscaler-transforms-in-python/) change the scale of numeric input variables. Data transforms like ordinal encoding change the type of categorical input variables.
- There are also many data transforms for changing the distribution of input variables. For example, [discretization](https://machinelearningmastery.com/discretization-transforms-for-machine-learning/) or binning change the distribution of numerical input variables into categorical variables with an ordinal ranking.
- The [power transform](https://machinelearningmastery.com/power-transforms-with-scikit-learn/) can be used to change the distribution of data to remove a skew and make the distribution more normal (Gaussian).
- The [quantile transform](https://machinelearningmastery.com/quantile-transforms-for-machine-learning/) is a flexible type of data preparation technique that can map a numerical input variable or to different types of distributions such as normal or Gaussian.
- Another type of data preparation technique that belongs to this group are methods that systematically change values in the dataset. This includes techniques that identify and replace missing values, often referred to as [missing value imputation](https://machinelearningmastery.com/statistical-imputation-for-missing-values-in-machine-learning/). This can be achieved using statistical methods or more advanced model-based methods.

```ad-tip
All of the methods discussed could also be considered feature engineering methods (e.g. fitting into the previously discussed group of data preparation methods) if the results of the transforms are appended to the raw data as new columns.
```

# Data Preparation for Columns + Values

This group is for data **preparation techniques that change both the number of columns and the values in the data.**

- The main class of techniques that this brings to mind are [dimensionality reduction techniques](https://machinelearningmastery.com/dimensionality-reduction-for-machine-learning/) that specifically reduce the number of columns and the scale and distribution of numerical input variables.
- This includes matrix factorization methods used in linear algebra as well as manifold learning algorithms used in high-dimensional statistics.

```ad-tip
Although these techniques are designed to create projections of rows in a lower-dimensional space, perhaps this also leaves the door open to techniques that do the inverse. That is, use all or a subset of the input variables to create a projection into a higher-dimensional space, perhaps decompiling complex non-linear relationships. 

Perhaps polynomial transforms where the results replace the raw dataset would fit into this class of data preparation methods.
```

# Data Preparation for Rows + Values

This group is for data preparation techniques that change both the number of rows and the values in the data.

I have not explicitly considered data transforms of this type before, but it falls out of the framework as defined.

A group of methods that come to mind are clustering algorithms where all or subsets of rows of data in the dataset are replaced with data samples at the cluster centers, referred to as cluster centroids.

Related might be replacing rows with exemplars (aggregates of rows) taken from specific machine learning algorithms, such as support vectors from a support vector machine, or the codebook vectors taken from a learning vector quantization.

Naturally, these aggregate rows are simply added to the dataset rather than replacing rows, then they would naturally fit into the “_Data Preparation for Rows_” group described above.