This approach involves studying the data and the requirements of specific algorithms and selecting data transforms that change your data to best meet the requirements.

```ad-warning
Many practitioners see this as the only possible approach to selecting data preparation techniques as it is often the only approach taught or described in textbooks.
```

This approach might involve first selecting an algorithm and preparing data specifically for it, or testing a suite of algorithms and ensuring the data preparation methods are tailored to each algorithm.

**This approach requires having detailed knowledge about your data**. This can be achieved by **reviewing summary statistics for each variable, plots of data distributions, and possibly even statistical tests to see if the data matches a known distribution.**

This approach **also requires detailed knowledge of the algorithms you will be using.** This can be achieved by reviewing textbooks that describe the algorithms.

From a high level, the data requirements of most algorithms are well known.

For example, **the following algorithms will probably be sensitive to the scale and distribution of your numerical input variables, as well as the presence of irrelevant and redundant variables**:

-   Linear Regression (and extensions)
-   Logistic Regression
-   Linear Discriminant Analysis
-   Gaussian Naive Bayes
-   Neural Networks
-   Support Vector Machines
-   k-Nearest Neighbors

**The following algorithms will probably not be sensitive to the scale and distribution of your numerical input variables and are reasonably insensitive to irrelevant and redundant variables**:

-   Decision Tree
-   AdaBoost
-   Bagged Decision Trees
-   Random Forest
-   Gradient Boosting

The benefit of this approach is that **it gives you some confidence that your data has been tailored to the expectations and requirements of specific algorithms. This may result in good or even great performance.**

<mark style="background: #FF5582A6;">The downside is that it can be a slow process requiring a lot of analysis, expertise, and, potentially, research. It also may result in a false sense of confidence that good or best results have already been achieved and that no or little further improvement is possible.</mark> 