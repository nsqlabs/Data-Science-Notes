For any Machine learning algo the ultimate goal is to reduce the error’s in the dataset so that it can predict the target variable’s more accurately.

To start, we need to find an equation of a line that **minimizes** the distance between all data points (see example below).

![](https://miro.medium.com/max/1400/1*F4JzgiTIUfFePLBj4A_JPw.jpeg)

One way to measure distance between the scattered points and the line is to find the distances between their Y values (in our case, sale price).
Let’s say we use our line [[Example|from earlier]], $F(x) = 100x + 50000$, and want to see how accurate our previous function is for a **1,500 square foot** house that actually sold for **$300,000**. Well, if we input a 1,500 square foot house into our earlier projection, it says we should have sold the house for $200,000 but in reality it sold for $300,000. A difference of $100,000! Point one for the real estate agent.

This difference, or **error**, in price is exactly what we need to do for the rest of the 99 data points. Once we do this for each point, we then add the errors together to measure our accuracy. More formally stated…

$$
\sum_{i=1}^n (y_i - \bar{y})^2
$$

Being:
- $y_i$ each point in the target dataset.
- $\bar{y}$ The predicted value for i

```ad-hint
These individual differences betweeen the real value and the predicted value are also called _residuals_. Let’s call the resulting sum the _sum of residuals_ (or SOR for short).
```