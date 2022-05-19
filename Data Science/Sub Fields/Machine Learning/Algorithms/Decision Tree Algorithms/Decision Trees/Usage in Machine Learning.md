## Machine Learning Decision Tree for Temperature Prediction

![](https://miro.medium.com/max/1400/1*H3nZElqhfOE35AFAq8gy0A.png)

We notice right away that each question (the white blocks) has only two answers: True or False. Moreover, for **each True and False answer there are separate branches. No matter the answers to the questions, we eventually reach a prediction (shown in the green blocks). This ‘computer-friendly’ version of the decision tree may look different than our intuitive model, but it works in the exact same way.**

Start at the node on the left, and progress through the tree answering the questions along the way. For our example, the season is winter so we take the True branch. We said the historical average was 46, so the second question is also True. Finally, the third answer is True as the max temperature today was 43. Therefore, the final prediction is 40 degrees for the max temperature tomorrow, close to our guess of 44.

This model here encompasses all the basic qualities of a decision tree. I purposefully left out all technical details, such as how the ‘questions’ are formed and how the thresholds are set, but these aren’t really necessary to understand the model conceptually or even to implement it in Python code!

```ad-warning
One aspect of the decision tree I should mention is how it actually learns. We refined our estimated range based on how the answers to the questions fit into our framework of the world. If the season is winter, our estimate is lower than if it is summer. However, a computer model of a decision tree has _no_ prior knowledge and would never be able to make the connection ‘winter = colder’ on its own. It must learn everything about the problem from the data we provide it. We know how to translate answers from the flow-chart into reasonable predictions because our of daily experiences. In contrast, the model must be taught each of these relationships such as that if the temperature today is warmer than the historical average, the max temperature tomorrow will likely be warmer as well. As a [supervised machine learning model](https://medium.com/machine-learning-for-humans/supervised-learning-740383a2feab), a random forest learns to map data (temperature today, historical average, etc.) to outputs (max temperature tomorrow) in what is called the training (or fitting) phase of model building.
```

During training, **we give the model any historical data that is relevant to the problem domain (the temperature the day before, the season of the year, and the historical average) and the true value we want the model to learn to predict, in this case the max temperature tomorrow.**
<mark style="background: green;">The model learns any relationships between the data (known as features in machine learning) and the values we want to predict (called the target). The decision tree forms the structure shown above, calculating the best questions to ask in order to make the most accurate estimates possible</mark>.

When we ask the decision tree to make a prediction for tomorrow, **we must give it the same data it used during training (the features) and it gives us an estimate based on the structure it has learned. Much as humans learn from examples, the decision tree also learns through experience, except it does not have any previous knowledge it can incorporate into the problem. Before training, we are much ‘smarter’ than the tree in terms of our ability to make a reasonable estimate. However, after enough training with quality data, the decision tree will far surpass our prediction abilities.**
```ad-danger
icon: exclamation
Keep in mind the decision tree does not have any conceptual understanding of the problem even after training. From the model’s ‘perspective’, it is simply receiving numbers as inputs and outputting different numbers that agree with those it saw during training. In other words, the tree has learned how to map a set of features to targets with no knowledge of anything about temperature. If we ask the decision tree another weather related question, it will have no clue how to respond because it has been trained for one specific task.
```

That is basically the entire high-level concept of a [[Decision Trees in our daily life|decision tree]]: a flowchart of questions leading to a prediction. Now, we take the mighty leap from a single decision tree to a random forest!

----
# Metadata

- Tags: #algorithms #data-science #machine-learning
- Connections. [[Random Forests simply explained]]