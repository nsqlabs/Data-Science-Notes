# Informal description

```ad-info
Describe the problem as though you were describing it to a friend or colleague. This can provide a great starting point for highlighting areas that you might need to fill. It also provides the basis for a one sentence description you can use to share your understanding of the problem.
```

For example: _I need a program that will tell me which tweets will get retweets._

# Formalism

Tom Mitchell’s machine learning formalism looks like this:

```ad-info
A computer program is said to learn from experience _E_ with respect to some class of tasks _T_ and performance measure _P_, if its performance at tasks in _T_, as measured by _P_, improves with experience _E_.```
```

Use this formalism to define the _T_, _P_, and _E_ for your problem.

For example:

-   **Task** (_T_): Classify a tweet that has not been published as going to get retweets or not.
-   **Experience** (_E_): A corpus of tweets for an account where some have retweets and some do not.
-   **Performance** (_P_): Classification accuracy, the number of tweets predicted correctly out of all tweets considered as a percentage.

### Assumptions

<mark style="background: #FF5582A6;">Create a list of assumptions about the problem and it’s phrasing. These may be rules of thumb and domain specific information that you think will get you to a viable solution faster.</mark> 

It can be useful to <mark style="background: #FF5582A6;">highlight questions that can be tested against real data because breakthroughs and innovation occur when assumptions and best practice are demonstrated to be wrong in the face of real data. It can also be useful to highlight areas of the problem specification that may need to be challenged, relaxed or tightened.</mark> 

For example:

-   The specific words used in the tweet matter to the model.
-   The specific user that retweets does not matter to the model.
-   The number of retweets may matter to the model.
-   Older tweets are less predictive than more recent tweets.

<center>
	<img src="https://machinelearningmastery.com/wp-content/uploads/2013/12/question-everything-300x225.jpg" width=400 />
</center>

# Similar problems

<mark style="background: #FF5582A6;">What other problems have you seen or can you think of that are like the problem you are trying to solve? Other problems can inform the problem you are trying to solve by highlighting limitations</mark> in your phrasing of the problem such as time dimensions and conceptual drift (where the concept being modeled changes over time). <mark style="background: #FF5582A6;">Other problems can also point to algorithms and data transformations that could be adopted to spot check performance.</mark> 

```ad-example
title:For example:

A related problem would be email spam discrimination that uses text messages as input data and needs binary classification decision.
```