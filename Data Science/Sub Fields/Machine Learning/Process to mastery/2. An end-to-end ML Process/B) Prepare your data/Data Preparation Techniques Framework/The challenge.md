Data preparation refers to transforming raw data into a form that is better suited to predictive modeling.

This may be required because the **data itself contains mistakes or errors. It may also be because the chosen algorithms have expectations regarding the type and distribution of the data.**

To make the task of data preparation even more challenging, it is also common that **the data preparation required to get the best performance from a predictive model may not be obvious and may bend or violate the expectations of the model that is being used.**

As such, **it is common to treat the choice and configuration of data preparation applied to the raw data as yet another hyperparameter of the modeling pipeline to be tuned.**

<mark style="background: #FF5582A6;">This framing of data preparation is very effective in practice, as it allows you to use automatic search techniques like grid search and random search to discover unintuitive data preparation steps that result in skillful predictive models.</mark> 

This framing of data preparation can also feel overwhelming to beginners given the large number and variety of data preparation techniques.

The solution to this overwhelm is to <mark style="background: #FFB8EBA6; color: #232323; font-weight: 800">think about data preparation techniques in a systematic way.</mark> 