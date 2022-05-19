### Step 1: Define Problem

This step is concerned with learning enough about the project to select the framing or framings of the prediction task. For example, is it classification or regression, or some other higher-order problem type?

It involves collecting the data that is believed to be useful in making a prediction and clearly defining the form that the prediction will take. It may also involve talking to project stakeholders and other people with deep expertise in the domain.

This step also involves taking a close look at the data, as well as perhaps exploring the data using summary statistics and data visualization.

### Step 2: Prepare Data

This step is concerned with transforming the raw data that was collected into a form that can be used in modeling.

> Data pre-processing techniques generally refer to the addition, deletion, or transformation of training set data.

— Page 27, [Applied Predictive Modeling](https://amzn.to/3b2LHTL), 2013.

We will take a closer look at this step in the next section.

### Step 3: Evaluate Models

This step is concerned with evaluating machine learning models on your dataset.

It requires that you design a robust test harness used to evaluate your models so that the results you get can be trusted and used to select among the models that you have evaluated.

This involves tasks such as selecting a performance metric for evaluating the skill of a model, establishing a baseline or floor in performance to which all model evaluations can be compared, and a resampling technique for splitting the data into training and test sets to simulate how the final model will be used.

For quick and dirty estimates of model performance, or for a very large dataset, a single train-test split of the data may be performed. It is more common to use k-fold cross-validation as the data resampling technique, often with repeats of the process to improve the robustness of the result.

This step also involves tasks for getting the most out of well-performing models such as hyperparameter tuning and ensembles of models.

### Step 4: Finalize Model

This step is concerned with selecting and using a final model.

Once a suite of models has been evaluated, you must choose a model that represents the “_solution_” to the project. This is called [model selection](https://machinelearningmastery.com/a-gentle-introduction-to-model-selection-for-machine-learning/) and may involve further evaluation of candidate models on a hold out validation dataset, or selection via other project-specific criteria such as model complexity.

It may also involve summarizing the performance of the model in a standard way for project stakeholders, which is an important step.

Finally, there will likely be tasks related to the [productization of the model](https://machinelearningmastery.com/deploy-machine-learning-model-to-production/), such as integrating it into a software project or production system and designing a monitoring and maintenance schedule for the model.

Now that we are familiar with the process of applied machine learning and where data preparation fits into that process, let’s take a closer look at the types of tasks that may be performed.