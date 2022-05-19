```ad-quote
*"As with many questions of statistics, the answer to **“which feature engineering methods are the best?” is that it depends.** Specifically, it depends on the model being used and the true relationship with the outcome."*
```

On the surface, this is a challenging question, but if we look at the data preparation step in the context of the whole project, it becomes more straightforward. The steps in a predictive modeling project before and after the data preparation step inform the data preparation that may be required.

The step before data preparation involves [[The subtasks of defining a problem|defining the problem]]. There may also be interplay between the data preparation step and the evaluation of models.

Model evaluation may involve sub-tasks such as:

-   Select a performance metric for evaluating model predictive skill.
-   Select a model evaluation procedure.
-   Select algorithms to evaluate.
-   Tune algorithm hyperparameters.
-   Combine predictive models into ensembles.

Information known about the choice of algorithms and the discovery of well-performing algorithms can also inform the selection and configuration of data preparation methods.

For example, the choice of algorithms may impose requirements and expectations on the type and form of input variables in the data. This might require variables to have a specific probability distribution, the removal of correlated input variables, and/or the removal of variables that are not strongly related to the target variable.

The choice of performance metric may also require careful preparation of the target variable in order to meet the expectations, such as scoring regression models based on prediction error using a specific unit of measure, requiring the inversion of any scaling transforms applied to that variable for modeling.

These examples, and more, highlight that although data preparation is an important step in a predictive modeling project, it does not stand alone. Instead, it is strongly influenced by the tasks performed both before and after data preparation. This highlights the highly iterative nature of any predictive modeling project.