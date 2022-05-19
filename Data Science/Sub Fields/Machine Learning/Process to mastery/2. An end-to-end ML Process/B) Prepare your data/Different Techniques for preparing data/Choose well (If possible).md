The performance of a machine learning model is only as good as the data used to train it.

This puts a heavy burden on the data and the techniques used to prepare it for modeling.

Data preparation refers to the techniques used to transform raw data into a form that best meets the expectations or requirements of a machine learning algorithm.

<mark style="background: #FF5582A6;">It is a challenge because we cannot know a representation of the raw data that will result in good or best performance of a predictive model.</mark> 

```ad-quote
*"However, we often do not know the best re-representation of the predictors to improve model performance. **Instead, the re-working of predictors is more of an art, requiring the right tools and experience to find better predictor representations.** Moreover, we may need to search many alternative predictor representations to improve model performance."* — Page xii, [Feature Engineering and Selection](https://amzn.to/3gMVxNE), 2019.
```

Instead, <mark style="background: #FF5582A6;">we must use controlled experiments to systematically evaluate data transforms on a model in order to discover what works well or best.</mark> 

As such, on a predictive modeling project, there are three main strategies we may decide to use in order to select a data preparation technique or sequences of techniques for a dataset; they are:

1.  Manually specify the data preparation to use for a given algorithm based on the deep knowledge of the data and the chosen algorithm.
2.  Test a suite of different data transforms and sequences of transforms and discover what works well or best on the dataset for one or range of models.
3.  Apply a suite of data transforms on the data in parallel to create a large number of engineered features that can be reduced using feature selection and used to train models.