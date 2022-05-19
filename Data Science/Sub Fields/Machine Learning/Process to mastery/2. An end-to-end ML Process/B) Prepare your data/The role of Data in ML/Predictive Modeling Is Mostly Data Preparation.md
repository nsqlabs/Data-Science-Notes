Modeling data with machine learning algorithms has become routine.

The vast majority of the common, popular, and widely used machine learning algorithms are decades old. Linear regression is more than 100 years old.

That is to say, **most algorithms are well understood and well parameterized and there are standard definitions and implementations available in open source software, like the scikit-learn machine learning library in Python.**

Although the algorithms are well understood operationally,<mark style="background: #FF5582A6;"> most don’t have satisfiable theories about why they work or how to map algorithms to problems. This is why each predictive modeling project is empirical rather than theoretical, requiring a process of systematic experimentation of algorithms on data.</mark> 

**Given that machine learning algorithms are routine for the most part, the one thing that changes from project to project is the specific data used in the modeling.**

```ad-quote
*"Data quality is one of the most important problems in data management, since dirty data often leads to inaccurate data analytics results and incorrect business decisions."* — Page xiii, [Data Cleaning](https://amzn.to/2SARxFG), 2019.
```

**If you have collected data for a classification or regression predictive modeling problem, it may be the first time ever, in all of history, that the problem has been modeled.** You are breaking new ground. That is not to say that the class of problems has not been tackled before; it probably has and you can learn from what was found if results were published. But it is today that **your specific collection of observations makes your predictive modeling problem unique.**

As such, <mark style="background: orange; color: black; font-weight: 800">the majority of your project will be spent on the data. Gathering data, verifying data, cleaning data, visualizing data, transforming data, and so on.</mark> 

```ad-quote
*"… it has been stated that up to 80% of data analysis is spent on the process of cleaning and preparing data. However, being a prerequisite to the rest of the data analysis workflow (visualization, modeling, reporting), it’s essential that you become fluent and efficient in data wrangling techniques."* - Page v, [Data Wrangling with R](https://amzn.to/2z8NB8k), 2016.
```

<mark style="background: orange; color: black; font-weight: 800">Your job is to discover how to best expose the learning algorithms to the unknown underlying structure of your prediction problem. The path to get there is through data preparation</mark>

In order for you to be an effective machine learning practitioner, you must know:

-   The **different types of data preparation to consider on a project.**
-   The **top few algorithms for each class of data preparation technique**.
-   **When to use and how to configure top data preparation techniques.**

This is often hard-earned knowledge, as there are few resources dedicated to the topic. Instead, you often must scour literature on statistics and application papers to get an idea of what’s available and how to use it.

```ad-quote
*"Practitioners agree that **the vast majority of time in building a machine learning pipeline is spent on feature engineering and data cleaning.** Yet, despite its importance, the topic is rarely discussed on its own.*" — Page vii, [Feature Engineering for Machine Learning](https://amzn.to/3b9tp3s), 2018.