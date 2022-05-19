You need automated tests to prove that your model works as you expect.

In software land, we call these regression tests. They ensure the software has not regressed in its behavior in the future as we make changes to different parts of the system.

Write regression tests for your model.

-   Collect or contribute a small sample of data on which to make predictions.
-   Use the production algorithm code and configuration to make predictions.
-   Confirm the results are expected in the test.

These tests are your early warning alarm. If they fail, your model is broken and you can’t release the software or the features that use the model.

> [!warning] Make the tests strictly enforce the minimum performance requirements of the model.

I strongly recommend **contriving test cases that you understand well, in addition to any raw datasets from the domain you want to include.**

> [!caution] Aim to break the model in tests
> I also strongly recommend gathering outlier and interesting cases from operations over time that produce unexpected results (or break the system). These should be understood and added to the regression test suite.

Run the regression tests after each code change and before each release. Run them nightly.