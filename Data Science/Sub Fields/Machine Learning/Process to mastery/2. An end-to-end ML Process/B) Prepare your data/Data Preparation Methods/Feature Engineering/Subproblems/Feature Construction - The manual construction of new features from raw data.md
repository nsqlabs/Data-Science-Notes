**The best results come down to you, the practitioner, crafting the features.**

**Feature importance and selection can inform you about the objective utility of features, but those features have to come from somewhere.**

You need to manually create them. <mark style="background: #FF5582A6;">This requires spending a lot of time with actual sample data (not aggregates) and **thinking about the underlying form of the problem, structures in the data and how best to expose them to predictive modeling algorithms.**</mark> 

With tabular data, **it often means a mixture of aggregating or combining features to create new features, and decomposing or splitting features to create new features.**

With textual data, **it often means devising document or context specific indicators relevant to the problem.** With image data, it can often mean **enormous amounts of time prescribing automatic filters to pick out relevant structures.**

```ad-hint
It is manual, it is slow, it requires lots of human brain power, and it makes a big difference.
```

This is the part of feature engineering that is often talked the most about as an artform, the part that is attributed the importance and signalled as the differentiator in competitive machine learning.

```ad-quote
*"Feature engineering and feature selection are not mutually exclusive.  They are both useful.  I’d say feature engineering is more important though, especially because you can’t really automate it."* - Robert Neuhaus, answer to “[Which do you think improves accuracy more, feature selection or feature engineering?](https://www.quora.com/How-valuable-do-you-think-feature-selection-is-in-machine-learning-Which-do-you-think-improves-accuracy-more-feature-selection-or-feature-engineering)”