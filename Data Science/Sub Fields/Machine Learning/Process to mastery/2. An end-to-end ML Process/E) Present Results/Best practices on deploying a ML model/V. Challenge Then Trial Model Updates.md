You will need to update the model.

Maybe you devise a whole new algorithm which requires new code and new config. Revisit all of the above points.

> [!abstract] A smaller and more manageable change would be to the model coefficients.
> For example, perhaps you set up a grid or random search of model hyperparameters that runs every night and spits out new candidate models.

**You should do this.**

> [!danger] Test the model and be highly critical. Give a new model every chance to slip up.

Evaluate the performance of the new model using the [[IV. Develop Back-Testing and Now-Testing Infrastructure|Back-Test and Now-Test infrastructure]]. Review the results carefully.

Evaluate the change using the regression test, as a final automated check.

> [!abstract] Test the features of the software that make use of the model.

Perhaps roll the change out to some locations or in a beta release for feedback, again for risk mitigation.

Accept your new model once you are satisfied that it meets the minimum performance requirements and betters prior results.

Like a ratchet, consider incrementally updating performance requirements as model performance improves.