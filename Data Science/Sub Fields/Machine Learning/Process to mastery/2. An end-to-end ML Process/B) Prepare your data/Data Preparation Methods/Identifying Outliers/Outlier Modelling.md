Outliers are extreme values that fall a long way outside of the other observations. For example, in a normal distribution, outliers may be values on the tails of the distribution.

The process of identifying outliers has many names in data mining and machine learning such as outlier mining, outlier modeling and novelty detection and anomaly detection.

Some methods to detect them:

-   **Extreme Value Analysis**: Determine the statistical tails of the underlying distribution of the data. For example, statistical methods like the z-scores on univariate data.
-   **Probabilistic and Statistical Models**: Determine unlikely instances from a probabilistic model of the data. For example, gaussian mixture models optimized using expectation-maximization.
-   **Linear Models**: Projection methods that model the data into lower dimensions using linear correlations. For example, principle component analysis and data with large residual errors may be outliers.
-   **Proximity-based Models**: Data instances that are isolated from the mass of the data as determined by cluster, density or nearest neighbor analysis.
-   **Information Theoretic Models**: Outliers are detected as data instances that increase the complexity (minimum code length) of the dataset.
-   **High-Dimensional Outlier Detection**: Methods that search subspaces for outliers give the breakdown of distance based measures in higher dimensions (curse of dimensionality).


## Get Started

There are many methods and much research put into outlier detection. **Start by making some assumptions and design experiments where you can clearly observe the effects of the those assumptions against some performance or accuracy measure.**

I recommend **working through a stepped process from extreme value analysis, proximity methods and projection methods.**

### Extreme Value Analysis

You do not need to know advanced statistical methods to look for, analyze and filter out outliers from your data. Start out simple with extreme value analysis.

-   Focus on univariate methods
-   Visualize the data using scatterplots, histograms and box and whisker plots and look for extreme values
-   Assume a distribution (Gaussian) and look for values more than 2 or 3 standard deviations from the mean or 1.5 times from the first or third quartile
-   Filter out outliers candidate from training dataset and assess your models performance

### Proximity Methods

Once you have explore simpler extreme value methods, consider moving onto proximity-based methods.

-   Use clustering methods to identify the natural clusters in the data (such as the k-means algorithm)
-   Identify and mark the cluster centroids
-   Identify data instances that are a fixed distance or percentage distance from cluster centroids
-   Filter out outliers candidate from training dataset and assess your models performance

### Projection Methods

Projection methods are relatively simple to apply and quickly highlight extraneous values.

-   Use projection methods to summarize your data to two dimensions (such as [PCA](https://machinelearningmastery.com/calculate-principal-component-analysis-scratch-python/), SOM or Sammon’s mapping)
-   Visualize the mapping and identify outliers by hand
-   Use proximity measures from projected values or codebook vectors to identify outliers
-   Filter out outliers candidate from training dataset and assess your models performance

### Methods Robust to Outliers

An alternative strategy is to move to models that are robust to outliers. There are robust forms of regression that minimize the median least square errors rather than mean (so-called robust regression), but are more computationally intensive. There are also methods like decision trees that are robust to outliers.

You could spot check some methods that are robust to outliers. If there are significant model accuracy benefits then there may be an opportunity to model and filter out outliers from your training data.