## General Examples of Feature Engineering

Let’s make the concepts of feature engineering more concrete.

In this section we will consider tabular data like that you might have in an excel spreadsheet. We will look at some examples of manual feature construction that you might like to consider on your own problems.

When I hear “_feature engineering is critically important_”, this is the type of feature engineering I think of. It is the most common form that I am familiar with and practice.

Which of these is best? You cannot know before hand. You must try them and evaluate the results to achieve on your algorithm and performance measures.

### Decompose Categorical Attributes

Imagine you have a categorical attribute, like “_Item_Color_” that can be _Red_, _Blue_ or _Unknown_.

_Unknown_ may be special, but to a model, it looks like just another colour choice. It might be beneficial to better expose this information.

You could create a new binary feature called “_Has_Color_” and assign it a value of “_1_” when an item has a color and “_0_” when the color is unknown.

Going a step further, you could create a binary feature for each value that _Item_Color_ has. This would be three binary attributes: _Is_Red_, _Is_Blue_ and _Is_Unknown_.

These additional features could be used instead of the _Item_Color_ feature (if you wanted to try a simpler linear model) or in addition to it (if you wanted to get more out of something like a decision tree).

### Decompose a Date-Time

A date-time contains a lot of information that can be difficult for a model to take advantage of in it’s native form, such as [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) (i.e. 2014-09-20T20:45:40Z).

If you suspect there are relationships between times and other attributes, you can decompose a date-time into constituent parts that may allow models to discover and exploit these relationships.

For example, you may suspect that there is a relationship between the time of day and other attributes.

You could create a new numerical feature called _Hour_of_Day_ for the hour that might help a regression model.

You could create a new ordinal feature called _Part_Of_Day_ with 4 values _Morning_, _Midday_, _Afternoon_, _Night_ with whatever hour boundaries you think are relevant. This might be useful for a decision tree.

You can use similar approaches to pick out time of week relationships, time of month relationships and various structures of seasonality across a year.

Date-times are rich in structure and if you suspect there is time dependence in your data, take your time and tease them out.

### Reframe Numerical Quantities

<mark style="background: #FF5582A6;">Your data is very likely to contain quantities, which can be reframed to better expose relevant structures. This may be a transform into a new unit or the decomposition of a rate into time and amount components.
</mark> 
You may have a quantity like a weight, distance or timing. A linear transform may be useful to regression and other scale dependent methods.

For example, you may have _Item_Weight_ in grams, with a value like 6289. You could create a new feature with this quantity in kilograms as 6.289 or rounded kilograms like 6. If the domain is shipping data, perhaps kilograms is sufficient or more useful (less noisy) a precision for _Item_Weight_.

The _Item_Weight_ could be split into two features: _Item_Weight_Kilograms_ and _Item_Weight_Remainder_Grams_, with example values of 6 and 289 respectively.

There may be domain knowledge that items with a weight above 4 incur a higher taxation rate. That magic domain number could be used to create a new binary feature _Item_Above_4kg_ with a value of “_1_” for our example of 6289 grams.

You may also have a quantity stored as a rate or an aggregate quantity for an interval. For example, _Num_Customer_Purchases_ aggregated over a year.

In this case you may want to go back to the data collection step and create new features in addition to this aggregate and try to expose more temporal structure in the purchases, like perhaps seasonality. For example, the following new binary features could be created: _Purchases_Summer_, _Purchases_Fall_, _Purchases_Winter_ and _Purchases_Spring_.

## Concrete Examples of Feature Engineering

A great place to study examples of feature engineering is in the results from competitive machine learning.

Competitions typically use data from a real-world problem domain. A write-up of methods and approach is required at the end of a competition. These write-ups give valuable insight into effective real-world machine learning processes and methods.

In this section we touch on a few examples of interesting and notable post-competition write-ups that focus on feature engineering.

### Predicting Student Test Performance in KDD Cup 2010

The [KDD Cup](http://www.sigkdd.org/kddcup/index.php) is a machine learning competition held for attendees of the ACM Special Interest Group on Knowledge Discovery and Data Mining conferences, each year.

In 2010, the focus of the competition was the problem of modeling how students learn. A corpus of student results on algebraic problems was provided to be used to predict those students’ future performance.

The winner of the competition were a group of students and academics at the National Taiwan University. Their approach is described in the paper “[Feature Engineering and Classifier Ensemble for KDD Cup 2010](https://pslcdatashop.web.cmu.edu/KDDCup/workshop/papers/kdd2010ntu.pdf)”.

The paper credits feature engineering as a key method in winning. Feature engineering simplified the structure of the problem at the expense of creating millions of binary features. The simple structure allowed the team to use highly performant but very simple linear methods to achieve the winning predictive model.

The paper provides details of how specific temporal and other non-linearities in the problem structure were reduced to simple composite binary indicators.

This is an extreme and instructive example of what is possible with simple attribute decomposition.

### Predicting Patient Admittance in the Heritage Health Prize

The [heritage health prize](https://www.heritagehealthprize.com/c/hhp) was a 3 million dollar prize awarded to the team who could best predict which patients would be admitted to hospital within the next year.

The prize had milestone awards each year where the top teams would be awarded a prize and their processes and methods made public.

I remember reading the papers released at the first of the three milestones and being impressed with the amount of feature engineering involved.

Specifically, the paper “[Round 1 Milestone Prize: How We Did It – Team Market Makers](https://foreverdata.org/1015/content/milestone1-2.pdf)” by Phil Brierley, David Vogel and Randy Axelrod. Most competitions involve vast amounts of feature engineering, but it struck me how clearly this paper made the point.

The paper provides both tables of attributes and SQL required to construct the attributes.

The paper gives some great real-world examples of feature engineering by simple decomposition. There are a lot of counts, mins, maxes, lots of binary attributes, and discretized numerical attributes. Very simple methods used to great effect.