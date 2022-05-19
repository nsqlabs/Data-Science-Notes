Even if your raw data contains only numbers, some data preparation is likely required.

<mark style="background: #FF5582A6;">There are many different machine learning algorithms to choose from for a given predictive modeling project. We cannot know which algorithm will be appropriate, let alone the most appropriate for our task. Therefore, it is a good practice to evaluate a suite of different candidate algorithms systematically and discover what works well or best on our data.</mark> 

The problem is, **each algorithm has specific requirements or expectations with regard to the data.**

```ad-quote
*"… data preparation **can make or break a model’s predictive ability. Different models have different sensitivities to the type of predictors in the model**; how the predictors enter the model is also important."* — Page 27, [Applied Predictive Modeling](https://amzn.to/3b2LHTL), 2013.
```

For example, **some algorithms assume each input variable, and perhaps the target variable, to have a specific probability distribution.** This is often the case for linear machine learning models that expect each numeric input variable to have a Gaussian probability distribution. This means that **if you have input variables that are not Gaussian or nearly Gaussian, you might need to change them so that they are Gaussian or more Gaussian.** Alternatively, it **may encourage you to reconfigure the algorithm to have a different expectation on the data.**

Some algorithms are known to **perform worse if there are input variables that are irrelevant or redundant to the target variable.** There are also algorithms that are negatively impacted if two or more input variables are highly correlated. In these cases, irrelevant or highly correlated variables may need to be identified and removed, or alternate algorithms may need to be used.

**There are also algorithms that have very few requirements about the probability distribution of input variables or the presence of redundancies, but in turn, may require many more examples (rows) in order to learn how to make good predictions.**

```ad-quote
*"The need for data pre-processing is determined by the type of model being used. Some procedures, such as tree-based models, are notably insensitive to the characteristics of the predictor data. Others, like linear regression, are not."* — Page 27, [Applied Predictive Modeling](https://amzn.to/3b2LHTL), 2013.
```

As such, **there is an interplay between the data and the choice of algorithms. Primarily, the algorithms impose expectations on the data, and adherence to these expectations requires the data to be appropriately prepared.** Conversely, the form of the data may help choose algorithms to evaluate that are more likely to be effective.