Data preparation may be one of the most difficult steps in any machine learning project.

The reason is that each dataset is different and highly specific to the project. Nevertheless, there are enough commonalities across predictive modeling projects that we can define a loose sequence of steps and subtasks that you are likely to perform.

This process provides a context in which we can consider the data preparation required for the project, informed both by the [[I. What is the problem| definition of the project performed before data preparation]] and the evaluation of machine learning algorithms performed after.

---

# What Is Data Preparation

```ad-quote
Data wrangling, which is also commonly referred to as data munging, transformation, manipulation, janitor work, etc., can be a painstakingly laborious process.
```

On a predictive modeling project, such as classification or regression, <mark style="background: #FF5582A6;">raw data typically cannot be used directly.</mark> 

This is because of reasons such as:

-   Machine learning algorithms require **data to be numbers.**
-   Some machine learning algorithms impose **requirements on the data.**
-   **Statistical noise and errors in the data may need to be corrected.**
-   **Complex nonlinear relationships may be teased out of the data.**

As such, **the raw data must be pre-processed prior to being used to fit and evaluate a machine learning model.** This step in a predictive modeling project is referred to as “**data preparation**“, although it goes by many other names, such as “_data wrangling_“, “_data cleaning_“, “_data pre-processing_” and “_feature engineering_“. Some of these names may better fit as sub-tasks for the broader data preparation process.


```ad-abstract
title: Definition of data preparation
We can define data preparation as the transformation of raw data into a form that is more suitable for modeling.
```

This is highly specific to your data, to the goals of your project, and to the algorithms that will be used to model your data.

Nevertheless, there are common or standard tasks that you may use or explore during the data preparation step in a machine learning project.

These tasks include:

1.  **Data Cleaning**: Identifying and correcting mistakes or errors in the data.
2.   **Feature Selection**: Identifying those input variables that are most relevant to the task.
3.   **Data Transforms**: Changing the scale or distribution of variables.
4.   **Feature Engineering**: Deriving new variables from available data.
5.   **Dimensionality Reduction**: Creating compact projections of the data.

Each of these tasks is a whole field of study with specialized algorithms.