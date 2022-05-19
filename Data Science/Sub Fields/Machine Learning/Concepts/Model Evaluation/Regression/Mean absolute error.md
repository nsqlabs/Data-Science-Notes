Mean absolute error (MAE) is one of the most common metrics that is used to calculate the prediction error of the model. Prediction error of a single row of data is:

$$
\text{Prediction Error} = \text{Actual Value} - \text{Predicted Value}
$$

We need to calculate prediction errors for each row of data, get their absolute value and then find the mean of all absolute prediction errors.

MAE is given by the following formula:

$$
\text {MAE (Mean Absolute Error)} = \frac{1}{N} \sum_{i=1} ^ N |y_i - \hat{y}|
$$

where $y_i$ represents the predicted value of $ŷ_i$.

<center>
	<img src="https://i.ibb.co/6m8j6Bz/MAEgraphical.png" width=300 />
</center>

The plot above represents the **residuals differences between the predicted values (regression line) and the output values. MAE uses the absolute value of the residuals, so it cannot indicate whether the model is underperforming or overperforming.**

Each residual contributes linearly to the total error because we are summing individual residuals. For that reason, small MAE suggests the model is great at prediction. Similarly, a large MAE suggests that your model may have trouble at generalizing well. An MAE of 0 means that our model outputs perfect predictions, but this is unlikely to happen in real scenarios.