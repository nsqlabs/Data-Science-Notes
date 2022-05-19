Knowing where feature engineering fits into the context of the process of applied machine learning highlights that it does not standalone.

<mark style="background: #FF5582A6;">It is an iterative process that interplays with data selection and model evaluation, again and again, until we run out of time on our problem.
</mark> 
The process might look as follows:

1.  **Brainstorm features**: Really get into the problem, look at a lot of data, study feature engineering on other problems and see what you can steal.
2.  **Devise features**: Depends on your problem, but you may use automatic feature extraction, manual feature construction and mixtures of the two.
3.  **Select features**: Use different feature importance scorings and feature selection methods to prepare one or more “views” for your models to operate upon.
4.  **Evaluate models**: Estimate model accuracy on unseen data using the chosen features.

<mark style="background: #FF5582A6;">You need a well defined problem so that you know when to stop this process and move on to trying other models, other model configurations, ensembles of models, and so on. There are gains to be had later in the pipeline once you plateau on ideas or the accuracy delta.</mark> 

```ad-caution
<mark>You need a well considered and designed test harness for objectively estimating model skill on unseen data</mark> . It **will be the only measure you have of your feature engineering process, and you must trust it not to waste your time.**
```