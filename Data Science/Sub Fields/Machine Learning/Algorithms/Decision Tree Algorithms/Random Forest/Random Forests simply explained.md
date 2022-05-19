<center>
	<br>
	<img src="https://miro.medium.com/max/1184/1*i0o8mjFfCn-uD79-F1Cqkw.png" width=500 style="border-radius: 20%" />
</center>

[[Decision Trees in our daily life|My prediction for the maximum temperature of today is probably wrong]]. And I hate to break it to you, but so is yours. There are **too many factors to take into account, and chances are, each individual guess will be high or low. Every person comes to the problem with different background knowledge and may interpret the exact same answer to a question entirely differently.** In technical terms, the predictions have variance because **they will be widely spread around the right answer.**

```ad-example
icon: question
title: What if we take predictions from hundreds or thousands of individuals, some of which are high and some of which are low, and decided to average them together?

Well, congratulations, we have created a random forest!
```

<mark style="background: green;">The fundamental idea behind a random forest is to combine many decision trees into a single model. Individually, predictions made by decision trees (or humans) may not be accurate, but combined together, the predictions will be closer to the mark on average.</mark> 

----
# Metadata

- Tags: #algorithms #data-science #machine-learning
- Connections. [[Decision Trees in our daily life]]