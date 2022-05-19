When starting with a problem and having defined a test harness you are happy with, it is time to spot check a variety of machine learning algorithms. Spot checking is useful because it allows you to very quickly see if there is any learnable structures in the data and estimate which algorithms may be effective on the problem.

**Spot checking also helps you work out any issues in your test harness and make sure the chosen performance measure is appropriate.**

The best first algorithm to spot check is a random. Plug in a random number generator to generate predictions in the appropriate range. This should be the worst “algorithm result” you achieve and will be the measure by which all improvements can be assessed.

**Select 5-10 standard algorithms that are appropriate for your problem and run them through your test harness. By standard algorithms, I mean popular methods no special configurations.** Appropriate for your problem means that the algorithms can handle regression if you have a regression problem.

```ad-hint
Choose methods from the [groupings of algorithms](https://machinelearningmastery.com/a-tour-of-machine-learning-algorithms/ "A Tour of Machine Learning Algorithms") we have already reviewed. I like to include a diverse mix and have 10-20 different algorithms drawn from a diverse range of algorithm types. Depending on the library I am using, I may spot check up to a 50+ popular methods to flush out promising methods quickly.

If you want to run a lot of methods, you may have to revisit data preparation and reduce the size of your selected dataset. This may reduce your confidence in the results, so test with various data set sizes. You may like to use a smaller size dataset for algorithm spot checking and a fuller dataset for algorithm tuning.
```