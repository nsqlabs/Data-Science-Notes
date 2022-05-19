The model will change, as will the software and the data on which predictions are being made.

You want to automate the evaluation of the production model with a specified configuration on a large corpus of data.

This will allow you to efficiently back-test changes to the model on historical data and determine if you have truly made an improvement or not.

This is not the small dataset that you may use for hyperparameter tuning, this is the full suite of data available, perhaps partitioned by month, year or some other important demarcation.

-   Run the current operational model to baseline performance.
-   Run new models, competing for a place to enter operations.

Once set-up, run it nightly or weekly and have it spit out automatic reports.

**Next, add a Now-Test.**

This is a test of the production model on the latest data.

Perhaps it’s the data from today, this week or this month. The idea is to get an early warning that the production model may be faltering.

This can be caused by content drift, where the relationships in the data exploited by your model are subtly changing with time.

This Now-Test can also spit out reports and raise an alarm (by email) if performance drops below minimum performance requirements.