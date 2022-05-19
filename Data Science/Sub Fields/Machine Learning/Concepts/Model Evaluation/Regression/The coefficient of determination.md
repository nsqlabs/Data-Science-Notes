> Also known as $R^2$ score

$R^2$ score determines how well the regression predictions approximate the real data points.

The value of $R^2$ is calculated with the following formula:

$$
R^2 = 1 - \frac {\sum_{i=1}^N (y_i - \hat{y})^2} {{\sum_{i=1}^N (y_i - \bar{y})^2}}
$$

where $ŷ_i$ represents the predicted value of $y_i$ and $ȳ$ is the mean of observed data which is calculated as

$$
\bar{y} = \sum_{i=1}^N y_i
$$