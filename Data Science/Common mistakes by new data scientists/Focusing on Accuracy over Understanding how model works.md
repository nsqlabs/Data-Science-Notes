How a predictive model makes a prediction is an very common overlooked part of the data science workflow. Accuracy isn’t always everything. A predictive model which can predict with 95% accuracy is obviously good but if you can’t explain it to the other person, how the model got there, which features led it there, and what your thinking was when building the model, your client will reject it.

As mentioned above, accuracy isn’t always what the business is after. Sure a model that predicts loan default with 95% accuracy is good, but if you can’t explain how the model got there, which features led it there, and what your thinking was when building the model, your client will reject it.

You will rarely, if ever, find a deep neural network being used in commercial applications. It’s just not possible to explain to the client how a neural network (let alone a deep one) worked with hidden layers, convolutions layers, etc. The first preference is, and will always be, on ensuring that we are able to understand what’s going on underneath the model. If you can’t tell whether age, or number of family members, or previous credit history went into rejecting a loan application, how will the business run?

Another key aspect is whether your model will fit within the organization’s existing framework. Using 10 different types of tools and libraries will fail spectacularly if the production environment cannot support it. You will have to redesign and retrain the model from scratch with a simpler approach.

## How to avoid this mistake?

The best way to prevent yourself from making this mistake is speaking to people working in the industry. There is no better teacher than experience. You can **practice making simpler models and then try explaining them to non-technical people. Then slowly add complexity to your model and keep doing this until even you don’t understand what’s going on beneath your data model.** This will teach you when to stop, and why simple models are always given preference in real-life applications. 

There is no better teacher than experience. Pick a domain (finance, HR, marketing, sales, operations, etc.) and reach out to people to understand how their project works.

Apart from that, practice making simpler models and then explaining them to non-technical people. Then add complexity to your model and keep doing this until even you don’t understand what’s going on beneath. This will teach you when to stop, and why simple models are always given preference in real-life applications.

> Additional reading link for assistance : [Click me](https://www.datascience.com/learn-data-science/fundamentals/model-interpretation-algorithms)