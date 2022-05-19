You have found a model that is good enough at addressing the problem you face that you would like to put it into production. This may be an operational installation on your workstation in the case of a fun side project, all the way up to integrating the model into an existing enterprise application. The scope is enormous.

Three areas that you should think carefully about are the algorithm implementation, the automated testing of your model and the tracking of the models performance through time. These three issues will very likely influence the type of model you choose.

## 1) Algorithm Implementation

> [!warning] The limitations of research libraries
> It is likely that you were using a research library to discover the best performing method. The algorithm implementations in research libraries can be excellent, but they can also be written for the general case of the problem rather than the specific case with which you are working.

Think very hard about the dependencies and technical debt you may be creating by putting such an implementation directly into production.

> [!abstract] Consider locating a production-level library that supports the method you wish to use.
> You may have to repeat the process of algorithm tuning if you switch to a production level library at this point.

You may also consider implementing the algorithm yourself. 

> [!danger] This option may introduce risk depending on the complexity of the algorithm you have chosen and the implementation tricks it uses.

Even with open source code, there may be a number of complex operations that may be very difficult to internalize and reproduce confidently.

## 2) Model Tests

Write **automated tests that verify that the model can be constructed and achieve a minimum level of performance repeatedly.** Also write tests for any data preparation steps.

> [!warning] You may wish to control the randomness used by the algorithm (random number seeds) for each unit test run so that tests are 100% reproducible.

## 3) Tracking

> [!abstract] Add infrastructure to monitor the performance of the model over time and raise alarms if accuracy drops below a minimum level. 
> Tracking may occur in real-time or with samples of live data on a re-created model in a separate environment. A raised alarm may be an indication that that structure learned by the model in the data have changed (concept drift) and that the model may need to be updated or tuned.

There are some model types that can perform online learning and update themselves. Think carefully in allowing models to update themselves in a production environment. In some circumstances, it can be wiser to manage the model update process and switch out models (their internal configuration) as they are verified to be more performant.