# Intuition

### 1. What is the intuition behind the algorithm

Initially, I used to learn an algorithm and used to forget after some time and whenever I get back to revise it I used to find it hard to understand which I already learned back then. Over time I realized that we humans can’t really remember things if they are too theoretical and we are more likely to remember it for a long time if learn it through visualizations. That is where geometry helps us visualize the core of an algorithm in the easiest way possible. And we are more tend to understand it deeper if we have some cool real-world daily life examples for these algorithms.

> Once you complete learning an algorithm from any course of your choice, open a new tab and start searching for the intuition of that algorithm. Trust me, there are a lot of cool explanations available on the internet. For starters, Quora and Medium are the best places to begin with.

### 2. How does the algorithm work?

Once you got the Intuition about it, play around and try to observe how the algorithm actually works. One more thing you need to check is how the algorithm works with various forms of data like Text/categorical/numbers.

During this phase, experiment with multiple factors and see how algorithms tend to work, you can refer to the readily available algorithms from Scikit-Learn. Check the parameters of the algorithm and try to play with them and see how they impact the model’s performance.

### 3. Where it can be used / Where it cannot be used

This is the most important factor that most people often miss out, while they focus more on what and how it works. Why it works or Why it doesn’t work is very important in understanding the algorithm in depth.

> Try to experiement and understand how It is working with large datasets, high dimensional data. If it is prone to outliers or imbalanced Dataset.

In interviews the toughest questions are not What and How but **Why.** Assume Tomorrow you make a personal project after learning algorithms and you used a particular X algorithm to solve it, the interviewer is most likely to respond with **why X algorithm why not Y?** Let's think you came up with accuracy as the reason, then comes the toughest question **why do you think it works better than the rest.**

> **Oh boy! That is why you should be aware of where it works and where it doesn’t work.**

For example, You need to come up with a reply like Since our data was high dimensional and non-linear in nature, algorithm X tends to do better with non-linear data than Y due to so and so reasons.

### 4. Why the interpretability of an Algorithm is important

This is one of the key steps, the reason this is important is that as a job of data scientist you might need to present the model to your clients who might have absolutely no Technical knowledge. During this, you might need to convince them that your model is predicting the right outcome and you need to provide some good reasons why they should adapt to it. You simply can’t throw the accuracy at them. If your algorithm is interpretable then you can show them why the model predicts something. Interpretability means nothing but the feature importance of an algorithm.

For example: If you are working on a Healthcare project where your model predicts the disease of a person to either positive/negative. It's a very sensitive problem and they can’t afford to make mistakes that is when interpretability comes in. If your model shows you the reason(since X feature(some levels in the body) is greater than x value or something) for predicting the person as positive/negative, it will become much easier and makes sense.

### 5. Why learn the Time/Space Complexity of an Algorithm?

When we work in realtime we might have to deal with huge amounts of data and if there is a requirement for low latency, that is where Time and Space Complexity can help you pick the right algorithms.

If your model occupies more memory, to run it in real-time can get very expensive especially if you are using the cloud infrastructure to run the model. Sometimes a few business problems come with a low latency requirement where are some algorithms that provide good accuracy but fail to satisfy the requirement due to their limitations with time/Space Complexities.

Wikipedia is a great resource to get all this relevant information for each algorithm.

### 6. Why do we need to understand the math behind an algorithm?

Math again? Yes, yes I get it. We can use algorithms even without understanding the math by simply importing from Scikit learn, but let me tell this is not at all recommended for the long run. Well, no matter if we accept it or not we definitely need math for a better understanding of what really happening under the hood. This might disappoint a few but I got good news we can not avoid Math but we can simplify it and avoid rigorous math.

> Simply, most of the Machine Learning algorithms job is to minimize the difference (LOSS) between Actual output and Predicted Output.  
> algorithm=minimize (Loss) + regularization term

For example, we should minimize log loss for logistic regression and Hinge loss for SVM and etc.

> Note: This is not the case for every ML algorithm, this works for few algorithms only.

To minimize this loss, internally these algorithms use Optimization techniques like Gradient Descent and its other flavors which involve a little math. So if you are someone who is not so well with math then just try to understand the loss functions and its Gradient descent for each algorithm, this way you can avoid all other rigorous math and stay intact with the goal. once you are comfortable with that you can dive deep into more math stuff.

### 7. Why Implement it from Scratch (Optional):

If suppose you are learning a guitar, you would start with the basics first and then slowly you try to replicate the music which is already composed by others and during this phase if you understand how they were able to create that music and tune, then the next step is to create your own music right?

In the same way, We can understand the existing algorithms more clearly by implementing them from scratch replicating the existing one. You’ll get to learn some important points that can help you build better models in the future. Just remember we might not be able to use Scikit learn’s version of an algorithm always in our project due to some issues. In such cases, you’ll have to be ready to optimize or modify the algorithm in a way that satisfies your requirement.

This is easier said than done, it will take a lot of your time to reach this point that is why I marked this as optional. At least try to implement one algorithm to understand how it actually works. If you find it hard to code, break down the algorithm into parts and write the pseudo code first later try to convert that into actual code.

**Python Machine Learning** by **Sebastian Raschka** is a really good book that can guide you in developing algorithms from scratch.


---

# Technical

What do you need to know about a machine learning algorithm to be able to use it well on a classification or prediction problem?

I won’t argue that the more that you know about how and why a particular algorithm works, the better you can wield it. But I do believe that there is a point of diminishing returns where you can stop, use what you know to be effective and dive deeper into the theory and research on an algorithm if and only if you need to know more in order to get better results.

## 1.  How do you refer to the technique (_e.g. what name_)?

This is obvious but important. You need to know the canonical name of the technique.

You need to be able to recognize the classical name or the name of the method from other fields as well and know that it is the same thing. This also includes the acronym for the algorithm, because sometimes they are less than intuitive.

This will help you sort out the base algorithm from extensions and the family tree of where the algorithm fits and relates to similar algorithms.

## 2. How Do You Represent a Learned Model?

I really like this nuts and bolts question.

This is question often overlooked in textbooks and papers and is perhaps the first question an engineer has when thinking about how a model will actually be used and deployed.

```ad-attention
The representation is the numbers and data structure that captures the distinct details learned from data by the learning algorithm to be used by the prediction algorithm. It’s the stuff you save to disk or the database when you finalize your model. It’s the stuff you update when new training data becomes available.
```

Let’s make this concrete with an example. In the case of linear regression, the representation is the vector of regression coefficients. That’s it. In the case of a decision tree is is the tree itself including the nodes, how they are connected and the variables and cut-off thresholds chosen.

## 3. How Do You Learn a Model?

Given some training data, the algorithm needs to create the model or fill in the model representation. This question is about exactly how that occurs.

Often learning involves estimating parameters from the training data directly in simpler algorithms.

In most other algorithms it involves using the training data as part of a cost or loss function and an optimization algorithm to minimize the function. Simpler linear techniques may use linear algebra to achieve this result, whereas others may use a numerical optimization.

Often the way a machine learning algorithm learns a model is synonymous with the algorithm itself. This is the challenging and often time consuming part of running a machine learning algorithm.

The learning algorithm may be parameterized and it is often a good idea to list common ranges for parameter values or configuration heuristics that may be used as a starting point.

## 4. How Do You Make Predictions With A Model?

Once a model is learned, it is intended to be used to make predictions on new data. Note, we re exclusively talking about predictive modeling machine learning algorithms for classification and regression problems.

This is often the fast and even trivial part of using a machine learning algorithm. Often it is so trivial that it is not even mentioned or discussed in the literature.

It may be trivial because prediction may be as simple as filling in the inputs in an equation and calculating a prediction, or traversing a decision tree to see what leaf-node lights up. In other algorithms, like k-nearest neighbors the prediction algorithm may be the main show (k-NN has no training algorithm other than “store the whole training set”).

## 5. How Do You Best Prepare Data For The Algorithm?

Machine learning algorithms make assumptions.

Even the most relaxed non-parametric methods make assumptions about your training data. It is good or even critical to review these assumptions. Even better is to translate these assumptions into specific data preparation operations that you can perform.

This question flushes out transforms that you could use on your data before modeling, or at the very least gives you pause to think about data transforms to try. What I mean by this is that it is best to treat algorithm requirements and assumptions as suggestions of things to try to get the most out your model rather than hard and fast rules that your data must adhere to.

Just like you cannot know which algorithm will be best for your data before hand, you cannot know the best transforms to apply to your data to get the most from an algorithm. Real data is messy and it is a good idea to try a number of presentations of your data with a number of different algorithms to see what warrants deeper investigation. The requirements and assumptions of machine learning algorithms help to point out presentations of your data to try.

## 6. How Do You Get More Information About the Algorithm?

Some algorithms will bubble up as generally better than others on your data problem.

When they do, you need to know where to look to get a deeper understanding of the technique. This can help with further customizing the algorithm for your data and with tuning the parameters of the learning and prediction algorithms.

It is a good idea to collect and list resources that you can reference if and when you need to dive deeper. This may include:

-   Journal Articles
-   Conference Papers
-   Books including textbooks and monographs
-   Webpages

I also think it is a good idea to know of more practical references like example tutorials and open source implementations that you can look inside to get a more concrete idea of what is going on.