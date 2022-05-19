-   We always need to make sure that the evaluation metric we choose for a regression problem does penalize errors in a way that reflects the consequences of those errors for the business, organizational, or user needs of our application.

-   If there are outliers in the data, they can have an unwanted influence on the overall R2 or MSE scores. MAE is robust to the presence of outliers because it uses the absolute value. Hence, we can use the MAE score if ignoring outliers is important to us.

-   MAE is the best metrics when we want to make a distinction between different models because it doesn’t reflect large residuals.

-   If we want to ensure that our model takes the outliers into account more, we should use the MSE metrics.