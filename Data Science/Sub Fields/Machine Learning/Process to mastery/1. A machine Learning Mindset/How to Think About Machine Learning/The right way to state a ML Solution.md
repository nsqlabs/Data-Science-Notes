The solution you require is best described as the following:

> A model or procedure that automatically creates the most likely approximation of the unknown underlying relationship between inputs and associated outputs in historical data.

Again, this is super specific.

**You need an automatic method that produces a program or model that you can use to make predictions.**

**You cannot sit down and write code to solve your problem. It is entirely data-specific and you have a lot of data.**

In fact, problems of this type resist top-down hand-coded solutions. **If you could sit down and write some if-statements to solve your problem, you would not need a machine learning solution. It would be a programming problem.**

<mark style="background: #FF5582A6;">The type of machine learning methods that you need will learn the relationship between the inputs and outputs in your historical data.</mark> 

```ad-tip
This framing allows you to think about what that real underlying yet unknown mapping function might look like and how noise, corruption, and sampling of your historical data may impact approximations of this mapping made by different modeling methods.
```

Without this framing, you will wonder things like:

-   Why there isn’t just one super algorithm or set of parameters.
-   Why the experts can’t just tell you what algorithm to use.
-   Why you can’t achieve a zero error rate with predictions from your model.

It helps you see the ill-defined nature of the predictive modeling problem you’re trying to solve and sets reasonable expectations.