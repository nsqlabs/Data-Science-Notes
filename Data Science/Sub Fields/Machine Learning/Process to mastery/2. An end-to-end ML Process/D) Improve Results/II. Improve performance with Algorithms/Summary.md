Machine learning is all about algorithms.

**Strategy**: Identify the algorithms and data representations that perform above a baseline of performance and better than average. Remain skeptical of results and design experiments that make it hard to fool yourself.

### Algorithm Tactics

-   **Resampling Method**. _What resampling method is used to estimate skill on new data?_ Use a method and configuration that makes the best use of available data. The k-fold cross-validation method with a hold out validation dataset might be a best practice.
-   **Evaluation Metric**. _What metric is used to evaluate the skill of predictions?_ Use a metric that best captures the requirements of the problem and the domain. It probably isn’t classification accuracy.
-   **Baseline Performance**. _What is the baseline performance for comparing algorithms?_ Use a random algorithm or a zero rule algorithm (predict mean or mode) to establish a baseline by which to rank all evaluated algorithms.
-   **Spot Check Linear Algorithms**. _What linear algorithms work well?_ Linear methods are often more biased, are easy to understand and are fast to train. They are preferred if you can achieve good results. Evaluate a diverse suite of linear methods.
-   **Spot Check Nonlinear Algorithms**. _What nonlinear algorithms work well?_ Nonlinear algorithms often require more data, have greater complexity but can achieve better performance. Evaluate a diverse suite of nonlinear methods.
-   **Steal from Literature**. _What algorithms are reported in the literature to work well on your problem?_ Perhaps you can get ideas of algorithm types or extensions of classical methods to explore on your problem.
-   **Standard Configurations**. _What are the standard configurations for the algorithms being evaluated?_ Each algorithm needs an opportunity to do well on your problem. This does not mean tune the parameters (yet) but it does mean to investigate how to configure each algorithm well and give it a fighting chance in the algorithm bake-off.

**Outcome**: You should now have a short list of well-performing algorithms and data representations.