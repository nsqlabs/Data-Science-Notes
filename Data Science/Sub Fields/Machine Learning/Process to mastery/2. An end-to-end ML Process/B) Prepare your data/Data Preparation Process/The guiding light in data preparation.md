Data preparation is not performed blindly.

<mark style="background: #FF5582A6;">In some cases, variables must be encoded or transformed before we can apply a machine learning algorithm, such as converting strings to numbers. In other cases, it is less clear, such as scaling a variable may or may not be useful to an algorithm.</mark> 

The broader philosophy of data preparation is to <mark style="background: #FF5582A6;">discover how to best expose the underlying structure of the problem to the learning algorithms. **This is the guiding light**.</mark> 


```ad-hint
We don’t know the underlying structure of the problem; if we did, we wouldn’t need a learning algorithm to discover it and learn how to make skillful predictions. Therefore, exposing the unknown underlying structure of the problem is a process of discovery, along with discovering the well- or best-performing learning algorithms for the project.
```

```ad-quote
*"[...] However, <mark style="background: #FF5582A6;">we often do not know the best re-representation of the predictors to improve model performance. Instead, the re-working of predictors is more of an art, requiring the right tools and experience to find better predictor representations</mark> . Moreover, we may need to search many alternative predictor representations to improve model performance."* — Page xii, [Feature Engineering and Selection](https://amzn.to/2Wu7zlL), 2019.
```

It can be more complicated than it appears at first glance. For example, **different input variables may require different data preparation methods. Further, different variables or subsets of input variables may require different sequences of data preparation methods.**

It can feel overwhelming, given the large number of methods, each of which may have their own configuration and requirements. Nevertheless, the machine learning process steps before and after data preparation can help to inform what techniques to consider.