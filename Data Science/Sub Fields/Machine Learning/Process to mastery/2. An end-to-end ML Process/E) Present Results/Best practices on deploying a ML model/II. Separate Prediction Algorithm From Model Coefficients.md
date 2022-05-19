You may have used a library to create your predictive model. For example, R, scikit-learn or Weka.

You can choose to deploy your model using that library or re-implement the predictive aspect of the model in your software. You may even want to [setup your model as a web service](https://www.quora.com/What-is-the-easiest-way-to-deploy-a-machine-learning-model-say-a-regression-for-production).

> [!abstract] Separate the algorithm that makes predictions from the model internals. 
> That is the specific coefficients or structure within the model learned from your training data.

## 2a. Select or Implement The Prediction Algorithm

Often the complexity a machine learning algorithms is in the model training, not in making predictions.

> [!example] 
> For example, making predictions with a regression algorithm is quite straightforward and easy to implement in your language of choice. This would be an example of an obvious algorithm to re-implement rather than the library used in the training of the model.

If you decide to use the library to make predictions, get familiar with the API and with the dependencies. The software used to make predictions is just like all the other software in your application.



> [!abstract] **Treat it like software.**
> Implement it well, write unit tests, make it robust.

## 2b. Serialize Your Model Coefficients

Let’s call the numbers or structure learned by the model: _coefficients_.

These data are not configuration for your application.

> [!abstract] **Treat it like software configuration.**
> Store it in an external file with the software project. Version it. Treat configuration like code because it can just as easily break your project.
> 
> <mark>You very likely will need to update this configuration in the future as you improve your model.</mark>