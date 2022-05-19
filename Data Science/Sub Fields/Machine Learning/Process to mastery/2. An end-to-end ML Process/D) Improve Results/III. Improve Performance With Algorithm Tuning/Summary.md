Algorithm tuning might be where you spend the most of your time. It can be very time-consuming. You can often unearth one or two well-performing algorithms quickly from spot-checking. Getting the most from those algorithms can take, days, weeks or months.

**Strategy**: Get the most out of well-performing machine learning algorithms.

### Tuning Tactics

-   **Diagnostics**. _What diagnostics and you review about your algorithm?_ Perhaps you can [review learning curves](https://machinelearningmastery.com/how-to-control-neural-network-model-capacity-with-nodes-and-layers/) to understand whether the method is over or underfitting the problem, and then correct. Different algorithms may offer different visualizations and diagnostics. Review what the algorithm is predicting right and wrong.
-   **Try Intuition**. _What does your gut tell you?_ If you fiddle with parameters for long enough and the feedback cycle is short, you can develop an intuition for how to configure an algorithm on a problem. Try this out and see if you can come up with new parameter configurations to try on your larger test harness.
-   **Steal from Literature**. _What parameters or parameter ranges are used in the literature?_ Evaluating the performance of standard parameters is a great place to start any tuning activity.
-   **Random Search**. _What parameters can use random search?_ Perhaps you can use random search of algorithm hyperparameters to expose configurations that you would never think to try.
-   **Grid Search**. _What parameters can use grid search?_ Perhaps there are grids of standard hyperparameter values that you can enumerate to find good configurations, then repeat the process with finer and finer grids.
-   **Optimize**. _What parameters can you optimize?_ Perhaps there are parameters like structure or learning rate than can be tuned using a direct search procedure (like pattern search) or stochastic optimization (like a genetic algorithm).
-   **Alternate Implementations**. _What other implementations of the algorithm are available?_ Perhaps an alternate implementation of the method can achieve better results on the same data. Each algorithm has a myriad of micro-decisions that must be made by the algorithm implementor. Some of these decisions may affect skill on your problem.
-   **Algorithm Extensions**. _What are common extensions to the algorithm?_ Perhaps you can lift performance by evaluating common or standard extensions to the method. This may require implementation work.
-   **Algorithm Customizations**. _What customizations can be made to the algorithm for your specific case?_ Perhaps there are modifications that you can make to the algorithm for your data, from loss function, internal optimization methods to algorithm specific decisions.
-   **Contact Experts**. _What do algorithm experts recommend in your case?_ Write a short email summarizing your prediction problem and what you have tried to one or more expert academics on the algorithm. This may reveal leading edge work or academic work previously unknown to you with new or fresh ideas.

**Outcome**: You should now have a short list of highly tuned algorithms on your machine learning problem, maybe even just one.

**Next**:One or more models could be finalized at this point and used to make predictions or put into production. Further lifts in performance can be gained by combining the predictions from multiple models.