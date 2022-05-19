From my perspective, problem-solving for a data scientist is:

-   More about “how to abstract the problem out of the business context”, not just “be handed with a specific task”
-   More about “solve the problem with an algorithm”, not just “use the best algorithm to solve a problem”
-   More about “iteratively deliver business value”, not just “implement the code and call it a day”.


# A framework

1. Define the problem.
2. Develop a plan to solve the problem.
3. Acquire the data needed to solve the problem.
4. Clean and prepare the data.
5. Explore the data to gain insights.
6. Model the data to solve the problem.
7. Evaluate the model.
8. Communicate the results.

![](https://www.techedgegroup.com/hs-fs/hubfs/2019%20-%20Big%20Data%20Analytics%20Data%20Intelligence/DI-DataScienceProcess.png?width=1200&name=DI-DataScienceProcess.png)

## 1. Define the problem.

  

Before beginning any work on a data science project, it is important to define the problem that you are trying to solve. This will help to ensure that you are focused on the right task, and will also help to guide your data acquisition and modeling efforts. For example, if you are trying to build a predictive model to identify potential customers for a new product, you would first need to define what characteristics of a customer you are trying to predict.

  

## 2. Develop a plan to solve the problem.

  

Once you have defined the problem, you will need to develop a plan for solving it. This plan will involve acquiring the data needed to build your model, preparing the data for modeling, building the model, and evaluating the results. For example, if you are building a predictive model, you will need to decide which type of model to build, what data to use, and how you will evaluate the results.

  

## 3. Acquire the data needed to solve the problem.

  

Acquiring the data needed to solve a data science problem can be a challenge in itself. Often, the data you need will be scattered across different sources, and may be in different formats. For example, if you are trying to build a predictive model to identify potential customers for a new product, you may need to gather data on customer demographics, purchase history, and product usage.

  

## 4. Clean and prepare the data.

  

Once you have acquired the data, you will need to clean and prepare it for modeling. This step will involve removing any invalid or missing data, and formatting the data in a way that is suitable for modeling. For example, if you are building a predictive model, you will need to ensure that all of the data is in a numerical format.

Below are some of the typical data issues that require modifications,

-   **_Noisy data_** — The dataset could have noise in it. Noise in the dataset doesn’t help in solving a problem. Missing data are noise. They do not generally help in making a correct prediction. We need to handle the noisy data for better results.
-   **_Scaling_** — Having attributes in different scales can be an issue. Especially if we use distance-based algorithms. It is always a good practice to normalize the data to a similar scale.
-   **_Correlated attributes_** — When we have many correlated attributes it is called Multicollinearity. This doesn’t generally impact the model prediction. But, they do have an impact on the interpretation of the independent variables.
-   **_Outliers_** — The outliers in the data impact the variance and the standard deviation.

Finally after analyzing the data for the above issues. We need to use relevant techniques to transform them into a preferred format. The transformation techniques will depend on the algorithm and the data itself.

  

## 5. Explore the data to gain insights.

  

Exploring the data is an important step in data science, as it can help you to gain insights into the problem you are trying to solve. This step will involve using various data visualization techniques to explore the data, and to look for patterns and relationships. For example, if you are building a predictive model, you may want to look for relationships between customer demographics and purchase history.

### Data exploration

Data exploration is key to any data science project. The success of a project depends on the level of understanding of the data. Some of the techniques that helps in better data analysis are,

-   **_Univariate analysis_** — To best understand the individual attributes. We pick one variable at a time to study the patterns. This will be the first step in any data exploration activity. It helps in building a good understanding of the dataset.
-   **_Multivariate analysis_** — To establish the relationship between the different attributes in the dataset. To explore the relationship between independent variables and the dependent variable.
-   **_Visual analysis_** — Useful in catching the patterns in the dataset. It is easy to find patterns in visual data. Visualizations are effective tools to communicate with the stakeholders.

  

## 6. Model the data to solve the problem.

Once you have explored the data, you will need to model it in order to solve the problem. This step will involve using a data mining or machine learning algorithm to build a predictive model. For example, if you are trying to build a predictive model to identify potential customers for a new product, you would use a machine learning algorithm to build a model that predicts whether or not a customer is likely to purchase the product.

  

## 7. Evaluate the model.

  

Once you have built a model, it is important to evaluate its performance. This step will involve using a test set of data to assess how well the model performs. For example, if you are building a predictive model, you would use a test set of data to see how accurately the model predicts whether or not a customer is likely to purchase the product.

  

## 8. Communicate the results.

  

Once you have evaluated the model, it is important to communicate the results. This step will involve writing a report or presenting the results to a decision maker. For example, if you are building a predictive model, you would write a report explaining the accuracy of the model, and recommending whether or not to use it.