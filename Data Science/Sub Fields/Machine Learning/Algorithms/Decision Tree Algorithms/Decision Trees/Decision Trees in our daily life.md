**We all use decision trees in our daily life, and even if you don’t know it by that name, I’m sure you’ll recognize the process. To illustrate the concept, we’ll use an everyday example: **predicting the tomorrow’s maximum temperature for our city.**

In order to answer the single max temperature question, we actually need to work through an entire series of queries. We start by forming an initial reasonable range given our domain knowledge, which for this problem might be 30–70 degrees (Fahrenheit) if we do not know the time of year before we begin. Gradually, through a set of questions and answers we reduce this range until we are confident enough to make a single prediction.

![](https://46gyn61z4i0t1u1pnq2bbk2e-wpengine.netdna-ssl.com/wp-content/uploads/2018/07/what-is-a-decision-tree.png)

What makes a good question to ask? Well, if we want to limit the range as much as is possible, it would be wise to **think of queries that are relevant to the problem at hand.**
- Since temperature is highly dependent on time of year, a decent place to start would be: what is the season? In this case, the season is winter, and so we can limit the prediction range to 30–50 degrees because we have an idea of what the general max temperatures are in the Pacific Northwest during the winter.

```ad-success
This first question was **a great choice because it has already cut our range in half. If we had asked something non-relevant, such as the day of the week, then we could not have reduced the extent of predictions at all and we would be back where we started.** Nonetheless, this single question isn’t quite enough to narrow down our estimate so we need to find out more information.
```

- A good follow-up question is: what is the historical average max temperature on this day? For Seattle on December 27, the answer is 46 degrees. This allows us to further restrict our range of consideration to 40–50 degrees. Again, this was a high-value question because it greatly reduced the scope of our estimate.

```ad-hint
Two questions are still not quite enough to make a prediction because this year might be warmer or colder than average. Therefore, we also would want to look at the max temperature today to get an idea if the year has been unusually warm or cold.
```
- Our question is simple: **what is the maximum temperature today? If the max temperature today was 43 degrees, it might be colder this year and our estimate for tomorrow should be a little lower than the historical average.** At this point, we can feel pretty confident in making a prediction of 44 degrees for the max temperature tomorrow.
> If we wanted to be even more sure, we could consult additional sources such as AccuWeather to get information such as the forecast for the max temperature that we could incorporate into our mental model. 
```ad-warning
At some point there is a diminishing return to asking more questions, and we cannot keep gathering more data for ever. For now, let us settle with using those three questions to make a prediction.
```

So, <mark style="background: #FF5582A6; font-weight: 600; color: white">to arrive at an estimate, we used a series of questions, with each question narrowing our possible values until we were confident enough to make a single prediction. We repeat this decision process over and over again in our daily lives with only the questions and answers changing.</mark> At this point we are nearly ready to make the connection to the decision tree, but let’s take just a minute to look at a graphical representation of the intuitive steps we took to find our answer:

<center>
	<img src="https://miro.medium.com/max/786/1*rvbyhgZYTQ3oc57X0nProw.png" />
</center>

----
# Metadata

- Tags: #algorithms #data-science #machine-learning
- Connections: