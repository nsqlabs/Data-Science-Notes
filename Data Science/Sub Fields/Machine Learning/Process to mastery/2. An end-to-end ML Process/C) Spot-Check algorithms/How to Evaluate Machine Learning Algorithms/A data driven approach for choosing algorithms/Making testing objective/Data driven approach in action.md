We do not need to fall into a heap of despair. We become scientists.

> [!danger] You have biases that can short-cut decisions for algorithm selection and algorithm parameter selection. They can serve you well in many cases, we think.

I want you to challenge this, try to consider abandoning heuristics and best practices and take on a data-driven approach to algorithm selection.

> [!example] How to use it?
> - Rather than picking your favorite algorithm, try 10 or 20 algorithms.
> - Double down on those that show signs of being better in performance, robustness, speed or whatever concerns interest you most.
> - Rather than picking the common parameters, grid search tens, hundreds or thousands of combinations of parameters.

Become the objective scientist, **leave behind anecdotes and study the intersection of complex learning systems and data observations from your problem domain.**

> [!caution] This is a powerful approach that requires less up-front knowledge, but a lot more back-end computation and experimentation.

As such, **you will very likely be required to work with a smaller sample of your dataset so that you can get results quickly.** You will want a test harness that you can have complete faith in.

> How can you have complete trust in your test harness?

You develop trust by selecting the [test options](https://machinelearningmastery.com/how-to-choose-the-right-test-options-when-evaluating-machine-learning-algorithms/ "How To Choose The Right Test Options When Evaluating Machine Learning Algorithms") in a data-driven manner that gives you objective confidence that your chosen configuration is reliable.
- The type of estimation method (split, boosting, k-fold cross validation, etc.)
- It’s configuration (size of k, etc.).