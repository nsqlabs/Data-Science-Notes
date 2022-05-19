Effective data preparation requires that <mark style="background: #FF5582A6;">the data preparation techniques available are organized and considered in a structured and systematic way.</mark> 

This allows you to <mark style="background: #FF5582A6;">ensure that approach techniques are explored for your dataset and that potentially effective techniques are not skipped or ignored.</mark> 

This can be achieved **using a framework to organize data preparation techniques that consider their effect on the raw dataset.**


````ad-abstract
For example, structured machine learning data, such as data we might store in a CSV file for classification and regression, consists of rows, columns, and values. We might consider data preparation techniques that operate at each of these levels.

-   Data Preparation for Rows
-   Data Preparation for Columns
-   Data Preparation for Values

```ad-important
Data preparation for rows may be techniques that add or remove rows of data from the dataset. Similarly, data preparation for columns may be techniques that add or remove columns (features or variables) from the dataset. Whereas data preparation for values may be techniques that change the values in the dataset, often for a given column.
```
````


There is one more type of data preparation that does not neatly fit into this structure, and that is dimensionality reduction techniques. **These techniques change the columns and the values at the same time, e.g. projecting the data into a lower-dimensional space.**

-   Data Preparation for Columns + Values

This raises the question of techniques that might apply to rows and values at the same time. This might include data preparation that consolidates rows of data in some way.

-   Data Preparation for Rows + Values

We can summarize this framework and some high-level groups of data preparation methods in the following image.

![Machine Learning Data Preparation Framework](https://machinelearningmastery.com/wp-content/uploads/2020/07/Machine-Learning-Data-Preparation-Framework.png)