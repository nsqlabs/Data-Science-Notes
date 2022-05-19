Feature engineering is an informal topic, but one that is absolutely known and agreed to be key to success in applied machine learning.

In creating this guide I went wide and deep and synthesized all of the material I could.

You will discover what feature engineering is, what problem it solves, why it matters, how to engineer features, who is doing it well and where you can go to learn more and get good at it.

If you read one article on feature engineering, I want it to be this one.

```ad-quote
"*Feature engineering is another topic which doesn’t seem to merit any review papers or books, or even chapters in books, but it is absolutely vital to ML success. […] Much of the success of machine learning is actually success in engineering features that a learner can understand.*" — Scott Locklin, in “[Neglected machine learning ideas](https://scottlocklin.wordpress.com/2014/07/22/neglected-machine-learning-ideas/)”
```

Here is how I define feature engineering:


```ad-quote
"*Feature engineering is **the process of transforming raw data into features that better represent the underlying problem to the predictive models**, resulting in improved model accuracy on unseen data.*"
```
You can see the dependencies in this definition:

-   The performance measures you’ve chosen (RMSE? AUC?)
-   The framing of the problem (classification? regression?)
-   The predictive models you’re using (SVM?)
-   The raw data you have selected and prepared (samples? formatting? cleaning?)

```ad-tip
"*Feature engineering is manually designing what the input x’s should be*" — Tomasz Malisiewicz, answer to “[What is feature engineering?](https://www.quora.com/What-is-feature-engineering)”
```


### Feature Engineering is a Representation Problem

<mark style="background: #FF5582A6;">Machine learning algorithms learn a solution to a problem from sample data.
</mark> 
In this context, <mark style="background: #FF5582A6;">feature engineering asks: what is the best representation of the sample data to learn a solution to your problem?</mark> 

It’s deep. <mark style="background: #FF5582A6;">Doing well in machine learning, even in artificial intelligence in general comes back to representation problems.</mark> It’s hard stuff, perhaps unknowable (or at best intractable) to know the best representation to use, _a priori_.

```ad-tip
"*You have to turn your inputs into things the algorithm can understand*" — Shayne Miel, answer to “[What is the intuitive explanation of feature engineering in machine learning?](https://www.quora.com/What-is-the-intuitive-explanation-of-feature-engineering-in-machine-learning)”
```

>


### Feature Engineering is an Art

It is an art like engineering is an art, like programming is an art, like medicine is an art.

<mark style="background: #FF5582A6;">There are well defined procedures that are methodical, provable and understood.
</mark> 
The <mark style="background: #FF5582A6;">data is a variable and is different every time. You get good at deciding which procedures to use and when, by practice. By empirical apprenticeship.</mark> Like engineering, like programming, like medicine, like machine learning in general.

Mastery of feature engineering comes with hands on practice, and study of what others that are doing well are practicing.

```ad-quote
*"…some machine learning projects succeed and some fail. What makes the difference? Easily the most important factor is the features used."* — Pedro Domingos, in “[A Few Useful Things to Know about Machine Learning](https://homes.cs.washington.edu/~pedrod/papers/cacm12.pdf)”
```