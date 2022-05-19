Linear regression, at it’s core, is a way of calculating the relationship between two variables. It assumes that there’s a direct correlation between the two variables, and that this relationship can be represented with a straight line.

These two variables are called the _independent variable_ and the _dependent variable_, and they are given these names for fairly intuitive reasons. The _independent variable_ is so named because the model assumes that it can behave however it likes, and doesn’t depend on the other variable for any reason. The _dependent variable_ is the opposite; the model assumes that it is a direct result of the _independent variable_, it’s value is highly dependent on the _independent variable_.

Linear regression creates a linear mathematical relationships between these two variables. It enables calculation predicting the _dependent variable_ if the _dependent variable_ is known. To bring this back to our somewhat ludicrous garden gnome example, we could create a regression with the East-West location of the garden gnome as the _independent variable_ and the North-South location as the _dependent variable_. We could then calculate the North-South location of any gnome in the city so long as we know its East-West location.

Since it’s such a simple form of regression, the governing equation for linear regression is also quite simple. It takes the form:

y = B* x + A

where y is the _dependent variable_, x is the _independent variable_, and A and B are coefficients determining the slope and intercept of the equation.