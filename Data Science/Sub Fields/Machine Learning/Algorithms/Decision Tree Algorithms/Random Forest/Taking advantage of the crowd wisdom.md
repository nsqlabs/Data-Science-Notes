```ad-example
icon: question
title: Why exactly is a random forest better than a single decision tree?

[[Why the name of random forest|We can think about it terms of having hundreds of humans make estimates for the max temperature problem: by pooling predictions, we can incorporate much more knowledge than from any one individual.]]
```
![](https://miro.medium.com/max/1200/0*YEwFetXQGPB8aDFV)
Each individual brings their own background experience and information sources to the problem. Some people may swear by Accuweather, while others will only look at NOAA (National Oceanic and Atmospheric Administration) forecasts.

- Perhaps one person relies on a meteorologist friend for their predictions.
- Perhaps another uses hundred of years of temperature data.

```ad-warning
If we only ask one individual, we would only take advantage of their limited scope of information, but by combining everyone’s predictions together, our net of information is much greater. Furthermore, the more diverse each person’s source of information, the more robust the random forest is because it will not be swayed by a single anomalous data source. If instead, individuals in our ‘forest’ use a number of different weather sources, then our model will not be greatly affected by a single source and we can continue to make reasonable predictions.
```

----
# Metadata

- Tags: #algorithms #data-science #machine-learning
- Connections. [[Random Forests simply explained]]