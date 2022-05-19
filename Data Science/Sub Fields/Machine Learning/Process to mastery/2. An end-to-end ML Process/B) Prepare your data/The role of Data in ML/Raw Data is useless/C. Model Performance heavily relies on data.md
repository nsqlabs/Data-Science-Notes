```ad-warning
Even if you prepare your data to meet the expectations of each model, you may not get the best performance.
```

Often, the performance of machine learning algorithms that have strong expectations degrades gracefully to the degree that the expectation is violated.

Further, it is common for an algorithm to perform well or better than other methods, even when its expectations have been ignored or completely violated. It is a common enough situation that this must be factored into the preparation and evaluation of machine learning algorithms.

```ad-quote
*"The idea that there are different ways to represent predictors in a model, and that some of these representations are better than others, leads to the idea of feature engineering — the process of creating representations of data that increase the effectiveness of a model."*  Page 3, [Feature Engineering and Selection](https://amzn.to/2Wu7zlL), 2019.
```

<mark style="background: #FF5582A6;">The performance of a machine learning algorithm is only as good as the data used to train it.</mark> This is often summarized as <mark style="background: #FF5582A6;">“**garbage in, garbage out**“</mark> . Garbage is harsh, but it could mean a “_weak representation_” of the problem that insufficiently captures the dynamics required to learn how to map examples of inputs to outputs.

Let’s take for granted that we have “_sufficient_” data to capture the relationship between input and output variables. It’s a slippery and domain-specific principle, and in practice, we have the data that we have, and our job is to do the best we can with that data.

A dataset may be a “_weak representation_” of the problem we are trying to solve for many reasons, although there are two main classes of reason. 
- It may be because complex nonlinear relationships are compressed in the raw data that can be unpacked using data preparation techniques.
- It may also be because the data is not perfect, ranging from mild random fluctuations in the observations, referred to as a statistical noise, to errors that result in out-of-range values and conflicting data.
	- **Complex Data**: Raw data contains compressed complex nonlinear relationships that may need to be exposed
	-   **Messy Data**: Raw data contains statistical noise, errors, missing values, and conflicting examples.

```ad-hint
We can think about getting the most out of our predictive modeling project in two ways: focus on the model and focus on the data.
```

We **could minimally prepare the raw data and begin modeling. This puts full onus on the model to tease out the relationships in the data and learn the mapping function from inputs to outputs as best it can.** This may be a reasonable path through a project and may require a <mark style="background: #FF5582A6;">large dataset and a flexible and powerful machine learning algorithm</mark> with few expectations, such as random forest or gradient boosting.

<mark style="background: #FFB8EBA6; color: black">Alternately, we could push the onus back onto the data and the data preparation process. This requires that each row of data maximumly or best expresses the information content of the data for modeling.</mark> Just like denormalization of data in a relational database to rows and columns, data preparation can denormalize the complex structure inherent in each single observation. This is also a reasonable path. It may require more knowledge of the data than is available but allows good or even best modeling performance to be achieved almost irrespective of the machine learning algorithm used.

```ad-tip
Often a balance between these approaches is pursued on any given project. That is both exploring powerful and flexible machine learning algorithms and using data preparation to best expose the structure of the data to the learning algorithms.
```

This is all to say, data preprocessing is a path to better data, and in turn, better model performance.