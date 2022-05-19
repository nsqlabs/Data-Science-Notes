[[Decision Trees in our daily life|Example for Temperature Prediction]]

1. We start with an initial guess based on our knowledge of the world and refine our estimate as we gain more information.
2. Eventually, we stop gathering data and make a decision, which in this case is the max temperature prediction.
3. Our natural approach to the problem is what we might call a question-and-answer flowchart. In fact, this flowchart is also a rudimentary model of a decision tree! 

<center>
<img 
	 src="https://miro.medium.com/max/720/1*T2mDW5eyCQE3_7FU4C_sig.jpeg" 
	 width=500
 />
<center>

```ad-important
However, we have not quite built a full decision tree because as humans we take some shortcuts that make sense for us but are not so intuitive to a machine.
```

**There are two main differences between our illustrated decision process and a real decision tree.** 
1. First, we have <mark style="background: green;">neglected to list the alternative branches, that is the predictions we would have made if the answers to the questions had been different</mark> : for example, if the season had been summer instead of winter, our range of predictions would have been shifted higher. 
```ad-hint
Moreover we phrased our questions such that they could take on any number of answers: when we asked ‘what is the maximum temperature today?’ the answer could be any real value.
```
2. In contrast, a decision tree implemented in machine learning will list all possible alternatives to every question and will ask all questions in True/False form. This is a little tough to grasp because it is not how humans naturally think, and perhaps the best way to show this difference is to create a real decision tree from our prediction process:

![](https://miro.medium.com/max/1400/1*H3nZElqhfOE35AFAq8gy0A.png)

----
# Metadata

- Tags: #algorithms #data-science #machine-learning
- Connections: [[Usage in Machine Learning]]