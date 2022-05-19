A solution to comparing algorithm performance measures when using multiple runs of k-fold cross validation is to use statistical significance tests (like the [Student’s t-test](https://en.wikipedia.org/wiki/Student's_t-test)).

The results from multiple runs of k-fold cross validation is a list of numbers. We like to summarize these numbers using the mean and standard deviation. You can think of these numbers as a sample from an underlying population. A statistical significance test answers the question: are two samples drawn from the same population? (no difference). If the answer is “yes”, then, even if the mean and standard deviations differ, the difference can be said to be not statistically significant.

We can use statistical significance tests to give meaning to the differences (or lack there of) between algorithm results when using multiple runs (like multiple runs of k-fold cross validation with different random number seeds). This can when we want to make accurate claims about results (algorithm A was better than algorithm B and the difference was statistically significant)

This is not the end of the story, because there are different statistical significance tests (parametric and nonparametric) and parameters to those tests (p-value).