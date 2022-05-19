Predictive modeling projects involve learning from data.

Data refers to examples or cases from the domain that characterize the problem you want to solve. In supervised learning, data is composed of examples where each example has an input element that will be provided to a model and an output or target element that the model is expected to predict.

```ad-quote
What we call data are observations of real-world phenomena. […] Each piece of data provides a small window into a limited aspect of reality.
```

Classification is an example of a supervised learning problem where the target is a label, and regression is an example of a supervised learning problem where the target is a number.

The input data may have many forms, such as an image, time series, text, video, and so on. The most common type of input data is typically referred to as tabular data or structured data. This is data as you might see it in a spreadsheet, in a database, or in a comma separated variable (CSV) file. This is the type of data that we will focus on.

Think of a large table of data. In linear algebra, we refer to this table of data as a matrix. The table is composed of rows and columns**. A row represents one example from the problem domain, and may be referred to as an “_example_“, an “_instance_“, or a “_case_“. A column represents the properties observed about the example and may be referred to as a “_variable_“, a “_feature_“, or a “_attribute_“.**

-   **Row**. A single example from the domain, often called an instance or example in machine learning.
-   **Column**. A single property recorded for each example, often called a variable or **feature** in machine learning.

```ad-abstract
For example, **the columns used for input to the model are referred to as input variables, and the column that contains the target to be predicted is referred to as the output variable. The rows used to train a model are referred to as the training dataset and the rows used to evaluate the model are referred to as the test dataset.**
```

-   **Input Variables**: Columns in the dataset provided to a model in order to make a prediction.
-   **Output Variable**. Column in the dataset to be predicted by a model.

When you collect your data, you may have to transform it so it forms one large table.

For example, if you have your data in a relational database, it is common to represent entities in separate tables in what is referred to as a “[normal form](https://en.wikipedia.org/wiki/Database_normalization)” so that redundancy is minimized. In order to create one large table with one row per “subject” or “entity” that you want to model, you may need to reverse this process and introduce redundancy in the data in a process referred to as [denormalization](https://en.wikipedia.org/wiki/Denormalization).

**If your data is in a spreadsheet or database, it is standard practice to extract and save the data in CSV format. This is a standard representation that is portable, well understood, and ready for the predictive modeling process with no external dependencies.**
