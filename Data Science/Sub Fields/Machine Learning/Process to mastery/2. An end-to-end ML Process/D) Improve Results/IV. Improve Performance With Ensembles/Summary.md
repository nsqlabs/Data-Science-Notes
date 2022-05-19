You can combine the predictions from multiple models. After algorithm tuning, this is the next big area for improvement. In fact, you can often get good performance from combining the predictions from multiple “good enough” models rather than from multiple highly tuned (and fragile) models.

**Strategy**: Combine the predictions of multiple well-performing models.

### Ensemble Tactics

-   **Blend Model Predictions**. _Can you combine the predictions from multiple models directly?_ Perhaps you could use the same or different algorithms to make multiple models. Take the mean or mode from the predictions of multiple well-performing models.
-   **Blend Data Representations**. _Can you combine predictions from models trained on different data representations?_ You may have many different projections of your problem which can be used to train well-performing algorithms, whose predictions can then be combined.
-   **Blend Data Samples**. _Can you combine models trained on different views of your data?_ Perhaps you can create multiple subsamples of your training data and train a well-performing algorithm, then combine predictions. This is called bootstrap aggregation or bagging and works best when the predictions from each model are skillful but in different ways (uncorrelated).
-   **Correct Predictions**. _Can you correct the predictions of well-performing models?_ Perhaps you can explicitly correct predictions or use a method like boosting to learn how to correct prediction errors.
-   **Learn to Combine**. _Can you use a new model to learn how to best combine the predictions from multiple well-performing models?_ This is called [stacked generalization or stacking](https://machinelearningmastery.com/stacking-ensemble-for-deep-learning-neural-networks/) and often works well when the submodels are skillful but in different ways and the aggregator model is a simple linear weighting of the predictions. This process can be repeated multiple layers deep.

**Outcome**: You should have one or more ensembles of well-performing models that outperform any single model.

**Next**: One or more ensembles could be finalized at this point and used to make predictions or put into production.