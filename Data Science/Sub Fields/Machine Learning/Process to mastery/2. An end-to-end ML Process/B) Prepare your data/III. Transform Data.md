The final step is to transform the process data. **The specific algorithm you are working with and the knowledge of the problem domain will influence this step and you will very likely have to revisit different transformations of your preprocessed data as you work on your problem.**

Three common data transformations are scaling, attribute decompositions and attribute aggregations. This step is also referred to as feature engineering.

-   **Scaling**: <mark style="background: #FF5582A6;">The preprocessed data may contain attributes with a mixtures of scales for various quantities such as dollars, kilograms and sales volume. Many machine learning methods like data attributes to have the same scale such as between 0 and 1 for the smallest and largest value for a given feature. Consider any feature scaling you may need to perform.</mark> 
-   **Decomposition**: <mark style="background: #FF5582A6;">There may be features that represent a complex concept that may be more useful to a machine learning method when split into the constituent parts. An example is a date that may have day and time components that in turn could be split out further.</mark> Perhaps only the hour of day is relevant to the problem being solved. consider what feature decompositions you can perform.
-   **Aggregation**: <mark style="background: #FF5582A6;">There may be features that can be aggregated into a single feature that would be more meaningful to the problem you are trying to solve.</mark> For example, there may be a data instances for each time a customer logged into a system that could be aggregated into a count for the number of logins allowing the additional instances to be discarded. Consider what type of feature aggregations could perform.

**You can spend a lot of time engineering features from your data and it can be very beneficial to the performance of an algorithm. Start small and build on the skills you learn.**