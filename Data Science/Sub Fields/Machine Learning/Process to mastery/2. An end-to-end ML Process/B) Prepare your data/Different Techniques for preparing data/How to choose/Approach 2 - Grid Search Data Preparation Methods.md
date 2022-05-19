```ad-abstract
This approach acknowledges that algorithms may have expectations and requirements, and does ensure that transforms of the dataset are created to meet those requirements, although it does not assume that meeting them will result in the best performance.

It leaves the door open to non-obvious and unintuitive solutions.
```

<mark style="background: #FF5582A6;">This might be a data transform that “_should not work_” or “_should not be appropriate for the algorithm_” yet results in good or great performance. Alternatively, it may be the absence of a data transform for an input variable that is deemed “_absolutely required_” yet results in good or great performance.</mark> 

<mark style="background: #FFF3A3A6; color: black; font-weight: 800">This can be achieved by designing a grid search of data preparation techniques and/or sequences of data preparation techniques in pipelines. This may involve evaluating each on a single chosen machine learning algorithm, or on a suite of machine learning algorithms.</mark> 

The result will be a large number of outcomes that will clearly indicate those data transforms, transform sequences, and/or transforms coupled with models that result in good or best performance on the dataset.

**These could be used directly, although more likely would provide the basis for further investigation by tuning data transforms and model hyperparameters to get the most out of the methods, and ablative studies to confirm all elements of a modeling pipeline contribute to the skillful predictions.**

I generally use this approach myself and advocate it to beginners or practitioners looking to achieve good results on a project quickly.

<mark style="background: #FF5582A6;">The benefit of this approach is that it always results in suggestions of modeling pipelines that give good relative results. Most importantly, it can unearth the non-obvious and unintuitive solutions to practitioners without the need for deep expertise.</mark> 

<mark style="background: #FF5582A6;">The downside is the need for some programming aptitude to implement the grid search and the added computational cost of evaluating many different data preparation techniques and pipelines.</mark> 