Data collected from your domain is referred to as raw data and is collected in the context of a problem you want to solve.

This means you must first define what you want to predict, then gather the data that you think will help you best make the predictions. This data collection exercise often requires a domain expert and may require many iterations of collecting more data, both in terms of new rows of data once they become available and new columns once identified as likely relevant to making a prediction.

-   **Raw data**: Data in the form provided from the domain.

In almost all cases, raw data will need to be changed before you can use it as the basis for modeling with machine learning.

> A feature is a numeric representation of an aspect of raw data. Features sit between data and models in the machine learning pipeline. Feature engineering is the act of extracting features from raw data and transforming them into formats that are suitable for the machine learning model.

— Page vii, [Feature Engineering for Machine Learning](https://amzn.to/3b9tp3s), 2018.

The cases with no data preparation are so rare or so trivial that it is practically a rule to prepare raw data in every machine learning project.

### 2. Machine Learning Algorithms Have Requirements



### 3. Model Performance Depends on Data

Even if you prepare your data to meet the expectations of each model, you may not get the best performance.

Often, the performance of machine learning algorithms that have strong expectations degrades gracefully to the degree that the expectation is violated.

Further, it is common for an algorithm to perform well or better than other methods, even when its expectations have been ignored or completely violated. It is a common enough situation that this must be factored into the preparation and evaluation of machine learning algorithms.

> The idea that there are different ways to represent predictors in a model, and that some of these representations are better than others, leads to the idea of feature engineering — the process of creating representations of data that increase the effectiveness of a model.

— Page 3, [Feature Engineering and Selection](https://amzn.to/2Wu7zlL), 2019.

The performance of a machine learning algorithm is only as good as the data used to train it. This is often summarized as “**garbage in, garbage out**“. Garbage is harsh, but it could mean a “_weak representation_” of the problem that insufficiently captures the dynamics required to learn how to map examples of inputs to outputs.

Let’s take for granted that we have “_sufficient_” data to capture the relationship between input and output variables. It’s a slippery and domain-specific principle, and in practice, we have the data that we have, and our job is to do the best we can with that data.

A dataset may be a “_weak representation_” of the problem we are trying to solve for many reasons, although there are two main classes of reason. It may be because complex nonlinear relationships are compressed in the raw data that can be unpacked using data preparation techniques. It may also be because the data is not perfect, ranging from mild random fluctuations in the observations, referred to as a statistical noise, to errors that result in out-of-range values and conflicting data.

-   **Complex Data**: Raw data contains compressed complex nonlinear relationships that may need to be exposed
-   **Messy Data**: Raw data contains statistical noise, errors, missing values, and conflicting examples.

We can think about getting the most out of our predictive modeling project in two ways: focus on the model and focus on the data.

We could minimally prepare the raw data and begin modeling. This puts full onus on the model to tease out the relationships in the data and learn the mapping function from inputs to outputs as best it can. This may be a reasonable path through a project and may require a large dataset and a flexible and powerful machine learning algorithm with few expectations, such as [random forest](https://machinelearningmastery.com/random-forest-ensemble-in-python/) or [gradient boosting](https://machinelearningmastery.com/gradient-boosting-machine-ensemble-in-python/).

Alternately, we could push the onus back onto the data and the data preparation process. This requires that each row of data maximumly or best expresses the information content of the data for modeling. Just like denormalization of data in a relational database to rows and columns, data preparation can denormalize the complex structure inherent in each single observation. This is also a reasonable path. It may require more knowledge of the data than is available but allows good or even best modeling performance to be achieved almost irrespective of the machine learning algorithm used.

Often a balance between these approaches is pursued on any given project. That is both exploring powerful and flexible machine learning algorithms and using data preparation to best expose the structure of the data to the learning algorithms.

This is all to say, data preprocessing is a path to better data, and in turn, better model performance.

1. [[A. Machine Learning Algorithms Expect Numbers]]
2. [[B. Machine Learning Algorithms Have Requirements]]
3. [[C. Model Performance heavily relies on data]]