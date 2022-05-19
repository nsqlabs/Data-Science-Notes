## The Traditional Approach is DEAD WRONG!

Think about this bottom-up approach to teaching machine learning for a second. It’s rigorous and systematic and sounds like the right idea on the surface. How could it be wrong?

### Bottom-Up Programming (or, how to kill off budding programmers)

Imagine you’re a young developer. You’ve picked up some of this and that language and you’re starting to learn how to create standalone software.

You tell friends and family that you want to get into a career where you get to program every day. They tell you that you need to do a degree in computer science before you can get a job as a programmer.

You sign-up and start a computer science degree. Semester after semester you are exposed to more and more esoteric algebra, calculus and discrete math. You use antiquated programming languages. Your passion for programming and building software wavers.

![Machine Learning for Programmers - Gap in Bottom Up](https://machinelearningmastery.com/wp-content/uploads/2015/08/Machine-Learning-for-Programmers-Gap-in-Bottom-Up-e1439699570377.png)

The traditional approach to getting started in machine learning has a gap on the path to practitioner.

Perhaps you somehow make it to the other side. Looking back, you realize you were not taught one thing about modern software development practices, languages, tooling, or anything that you can use in your pursuit of creating and delivering software.

See the parallels to the teaching of machine learning?

Thankfully, programming has been around long enough, is popular enough and is important enough to the economy that we have found other ways to give budding young (or old) programmers the skills they need to actually do the thing they want to do – e.g. create software.

It does not make sense to load up a budding programmer’s head with theory on [computability](https://en.wikipedia.org/wiki/Computability_theory) or [computational complexity](https://en.wikipedia.org/wiki/Computational_complexity_theory), or even deep details of algorithms and data structures. Some of this useful material (the latter on algorithmic complexity and data structures) can come later. Perhaps with focused material – but importantly in the context of an engineer that is already programming and delivering software, not in isolation.

Thankfully we have focused software engineering degrees. We also have resources like [codecademy](https://www.codecademy.com/) where you learn to program by… yep, actually programming.

If a developer wants to “do” machine learning, should they really have to go and spend a bunch of years and tens or hundreds of thousands of dollars to get the requisite math and higher degrees?

The answer is of course not! There is a better way.

## A Better Approach

As with computer science, you can’t just invert the model and teach the same material top-down.

The reason is, like a computer science course never making it to the subjects that cover the practical concerns of developing and delivering software, machine learning courses and books fall well short. They stop at algorithms.

You need a top-down approach to machine learning. An approach where you focus on the actual result you want: working real machine learning problems from end-to-end using modern and “_best of breed_” tools and platforms.

![Machine Learning for Programmers - A Better Approach](https://machinelearningmastery.com/wp-content/uploads/2015/08/Machine-Learning-for-Programmers-A-Better-Approach-e1439699675138.png)

A better approach to learning machine learning that starts with working machine learning problems end-to-end.

Here’s what I think your yellow brick road looks like.

### 1. Repeatable Results with a Systematic Process

Once you know some tooling, it is relatively easy to blast a problem with a machine learning algorithm and call it “_done_“.

This could be dangerous.

How do you know you’re done? How do you know the results are any good? How do you know the results are reliable on the dataset?

You need to be systematic when working a machine learning problem. It’s a project, like a software project, and good processes can make achieving a high-quality result repeatable from project to project.

Contemplating such a process you can think of some clear requirements, such as:

-   A process that guides you from end-to-end, from problem specification to presentation or deployment of results. Like a software project, you can think you’re done, but you’re probably not. Having the end deliverable in mind from the beginning sets an unambiguous project stop condition and focuses effort.
-   A process that is step-by-step so that you always know what to do next. Not knowing what to do next is a project killer.
-   A process that guarantees “_good_” results, e.g. better than average or good enough for the needs of the project. It is very common for projects to need good results delivered reliably with known confidence levels, not necessarily the very best accuracy possible.
-   A process that is invariant to the specific tools, programming languages and algorithm fads. Tools come and go and the process must be adaptive. Given the algorithm obsession in the field, there are always new and powerful algorithms coming out of academia.

![Machine Learning for Programmers - Select a Systematic Process](https://machinelearningmastery.com/wp-content/uploads/2015/08/Machine-Learning-for-Programmers-Select-a-Systematic-Process-e1439699783406.png)

Select a systematic and repeatable process that you can use to deliver results consistently.

There are many great processes out there, including some older processes that you can adapt to your needs.

For example:

-   [Knowledge Discovery in Databases](https://machinelearningmastery.com/what-is-data-mining-and-kdd/) (KDD), [which I have adapted here](https://machinelearningmastery.com/process-for-working-through-machine-learning-problems/)
-   [CRISP-DM](https://en.wikipedia.org/wiki/Cross_Industry_Standard_Process_for_Data_Mining)
-   [OSEMN](https://machinelearningmastery.com/how-to-work-through-a-problem-like-a-data-scientist/)
-   others…

Pick or adapt a process that works best for you and meets the requirements above.

# Machine Learning for Developers

by [Jason Brownlee](https://machinelearningmastery.com/author/jasonb/ "Posts by Jason Brownlee") on August 17, 2015 in [Start Machine Learning](https://machinelearningmastery.com/category/start-machine-learning/ "View all items in Start Machine Learning")

_Tweet_ _Tweet_  Share Share

Last Updated on May 18, 2020

#### _How Do I Get Started In Machine Learning?_

> I’m a developer. I have read a book or some posts on machine learning. I have watched some of the Coursera machine learning course. I still don’t know how to get started…

Does this sound familiar?

![Machine Learning Frustration](https://machinelearningmastery.com/wp-content/uploads/2015/08/Machine-Learning-Frustration.jpg)

Frustrated with machine learning books and courses?  
How do you get started in machine learning?  
Photo by [Peter Alfred Hess](https://www.flickr.com/photos/peterhess/2976755407/), some rights reserved

The most common question I’m asked by developers on my newsletter is:

> _How do I get started in machine learning?_

I honestly cannot remember how many times I have answered it.

In this post, I lay out all of my very best thinking on this topic.

-   You will discover why the traditional approach to teaching machine learning does not work for you.
-   You will discover how to flip the entire model on its head.
-   And you will discover my simple but very effective antidote that you can use to get started.

Let’s get into it…

## A Developer Interested in Machine Learning

You are a developer and you’re interested in getting into machine learning. And why not? It’s a hot topic at the moment, and it’s a fascinating and fast growing field.

You read some blog posts. You tried to go deeper but the books are dreadful. Math focused. Theory focused. Algorithm focused.

![Machine Learning for Programmers - How Do I Get Started](https://machinelearningmastery.com/wp-content/uploads/2015/08/Machine-Learning-for-Programmers-How-Do-I-Get-Started-e1439699337810.png)

Sound familiar? Have you tried books, MOOCs, blog posts and still not know how to get started in machine learning?

You try some video courses. You sign-up and make an honest attempt at the oft-cited [Coursera Stanford Machine Learning MOOC](https://www.coursera.org/learn/machine-learning). It’s not much better than the books and detailed blog posts. You can’t see what all the fuss is about, why it is recommended to beginners.

You may have even attempted some small data sets, perhaps an entry level Kaggle competition.

The problem is you can’t connect the theory, algorithms and math from the books and courses to the problem. There’s a huge gap. A gulf. **How ARE you supposed to get started in machine learning?**

## Machine Learning Engineer

When you think forward into the future, once you have captured this elusive understanding of machine learning, what does your job look like? How are you using your newfound machine learning skills in your day-to-day?

I think I can see it. You’re a machine learning engineer. You’re a developer that knows how to “do” machine learning.

![Machine Learning for Programmers - Dream](https://machinelearningmastery.com/wp-content/uploads/2015/08/Machine-Learning-for-Programmers-Dream-e1439699316636.png)

Do you want to transition from developer to a developer that can do machine learning?

### Scenario 1: The one-off model

Your boss walks over and says:

> Hey, you know machine learning, right? Can you use the customer data from last year to predict which current customers in our sales pipeline are likely to convert? I want to use it in a presentation to the board next week…

I call this the one-off model.

The problem is well defined by your boss. She gives you the data, which is small enough to look at and understand in MS Excel if you had to. She wants accurate and reliable predictions.

You can deliver. And more importantly, you can explain all the relevant caveats on the results.

### Scenario 2: The embedded model

You and your team are collecting requirements from stakeholders on a software project. There is a requirement for the user to be able to freehand draw shapes in the software, and for the software to figure out which shape it is and turn it into a crisp unambiguous version and label it appropriately.

You quickly see that the best (and only viable?) way to solve this problem is to devise and train a predictive model and embed it in your software product.

I call this the embedded model. There are variations (such as whether the model is static or updated, and whether it is local or called remotely via an API), but that’s just detail.

What’s key in this scenario is that you have the experience to notice a problem that is best solved with a predictive model and the skills to devise, train and deploy it.

### Scenario 3: The deep model

You have started a new job and the system you are working on is made up of at least one predictive model. Maintenance and the addition of features to this system require an understanding of the model, its inputs and its outputs. The accuracy of the model is a feature of the software product and part of your job will be to improve it.

For example, as a part of regular pre-release system testing, you must demonstrate that the accuracy of the model (when validated on historical data) has the same or better skill than the previous version.

I call this the deep model. You will be expected to build a deep understanding of one specific predictive model and use your experience and skill to improve and verify its accuracy as part of your routine duties.

### The Developer That “_Does_” Machine Learning

These scenarios give you a glimpse at what it’s like to be a developer that knows how to do machine learning. They’re realistic because they are all variations on scenarios I’ve been in or tasks that I have had to complete.

All three of these scenarios make one thing very clear. Although machine learning is a fascinating area, to a developer machine learning algorithms are just another bag of tricks, like multi-threading or 3d graphics programming. Nevertheless, they are a powerful group of methods that are absolutely required for a specific class of problem.

## Traditional Answer To: “_how do I get started?_“

So how do you get started in machine learning?

If you crack a book on machine learning seeking an answer to this question, you’ll get a shock. They start with definitions and move on to mathematical descriptions of concepts and algorithms of ever increasing complexity.

![Machine Learning for Programmers - The Traditional Approach](https://machinelearningmastery.com/wp-content/uploads/2015/08/Machine-Learning-for-Programmers-The-Traditional-Approach1.png)

The traditional answer to the question “how do I get started in machine learning” is bottom-up.

Definitions and mathematical descriptions are clear, succinct and often unambiguous. The thing is, they are dry, boring and require the requisite mathematical background to parse and interpret.

There is a reason why machine learning is often taught as a graduate level subject at university. It’s because this “first principles” way of teaching the subject requires years of prerequisites to understand.

For example, it is advisable that you have a good footing in:

-   Statistics
-   Probability
-   Linear Algebra
-   Multivariate Statistics
-   Calculus

This gets worse if you stray slightly into some of the more exotic and interesting algorithms.

This bottom-up and algorithm fixated approach to machine learning is pervasive.

Online courses, MOOCs and YouTube videos mimic the university approach to teaching machine learning. Again, this is great if you have the background or you’ve already put in your half-to-full-decade of studies to earn those higher degrees. It does not help your average developer.

If you skulk off to a question and answer forum like [Quora](https://www.quora.com/How-do-I-learn-machine-learning-1), [StackExchange](https://programmers.stackexchange.com/questions/79476/what-skills-are-needed-for-machine-learning-jobs) or [Reddit](https://www.reddit.com/r/learnprogramming/comments/3d5ajk/where_to_start_with_machine_learning/) and meekly ask how to get started, you’re slapped with the same response. Often this response comes from fellow developers who are just as lost. It’s one big echo chamber of the same bad advice.

It’s no wonder that honest and hard working developers seeking to do the right thing think they have to go back to school and get a Masters or Ph.D. before they feel qualified to “do” machine learning.

## The Traditional Approach is DEAD WRONG!

Think about this bottom-up approach to teaching machine learning for a second. It’s rigorous and systematic and sounds like the right idea on the surface. How could it be wrong?

### Bottom-Up Programming (or, how to kill off budding programmers)

Imagine you’re a young developer. You’ve picked up some of this and that language and you’re starting to learn how to create standalone software.

You tell friends and family that you want to get into a career where you get to program every day. They tell you that you need to do a degree in computer science before you can get a job as a programmer.

You sign-up and start a computer science degree. Semester after semester you are exposed to more and more esoteric algebra, calculus and discrete math. You use antiquated programming languages. Your passion for programming and building software wavers.

![Machine Learning for Programmers - Gap in Bottom Up](https://machinelearningmastery.com/wp-content/uploads/2015/08/Machine-Learning-for-Programmers-Gap-in-Bottom-Up-e1439699570377.png)

The traditional approach to getting started in machine learning has a gap on the path to practitioner.

Perhaps you somehow make it to the other side. Looking back, you realize you were not taught one thing about modern software development practices, languages, tooling, or anything that you can use in your pursuit of creating and delivering software.

See the parallels to the teaching of machine learning?

Thankfully, programming has been around long enough, is popular enough and is important enough to the economy that we have found other ways to give budding young (or old) programmers the skills they need to actually do the thing they want to do – e.g. create software.

It does not make sense to load up a budding programmer’s head with theory on [computability](https://en.wikipedia.org/wiki/Computability_theory) or [computational complexity](https://en.wikipedia.org/wiki/Computational_complexity_theory), or even deep details of algorithms and data structures. Some of this useful material (the latter on algorithmic complexity and data structures) can come later. Perhaps with focused material – but importantly in the context of an engineer that is already programming and delivering software, not in isolation.

Thankfully we have focused software engineering degrees. We also have resources like [codecademy](https://www.codecademy.com/) where you learn to program by… yep, actually programming.

If a developer wants to “do” machine learning, should they really have to go and spend a bunch of years and tens or hundreds of thousands of dollars to get the requisite math and higher degrees?

The answer is of course not! There is a better way.

## A Better Approach

As with computer science, you can’t just invert the model and teach the same material top-down.

The reason is, like a computer science course never making it to the subjects that cover the practical concerns of developing and delivering software, machine learning courses and books fall well short. They stop at algorithms.

You need a top-down approach to machine learning. An approach where you focus on the actual result you want: working real machine learning problems from end-to-end using modern and “_best of breed_” tools and platforms.

![Machine Learning for Programmers - A Better Approach](https://machinelearningmastery.com/wp-content/uploads/2015/08/Machine-Learning-for-Programmers-A-Better-Approach-e1439699675138.png)

A better approach to learning machine learning that starts with working machine learning problems end-to-end.

Here’s what I think your yellow brick road looks like.

### 1. Repeatable Results with a Systematic Process

Once you know some tooling, it is relatively easy to blast a problem with a machine learning algorithm and call it “_done_“.

This could be dangerous.

How do you know you’re done? How do you know the results are any good? How do you know the results are reliable on the dataset?

You need to be systematic when working a machine learning problem. It’s a project, like a software project, and good processes can make achieving a high-quality result repeatable from project to project.

Contemplating such a process you can think of some clear requirements, such as:

-   A process that guides you from end-to-end, from problem specification to presentation or deployment of results. Like a software project, you can think you’re done, but you’re probably not. Having the end deliverable in mind from the beginning sets an unambiguous project stop condition and focuses effort.
-   A process that is step-by-step so that you always know what to do next. Not knowing what to do next is a project killer.
-   A process that guarantees “_good_” results, e.g. better than average or good enough for the needs of the project. It is very common for projects to need good results delivered reliably with known confidence levels, not necessarily the very best accuracy possible.
-   A process that is invariant to the specific tools, programming languages and algorithm fads. Tools come and go and the process must be adaptive. Given the algorithm obsession in the field, there are always new and powerful algorithms coming out of academia.

![Machine Learning for Programmers - Select a Systematic Process](https://machinelearningmastery.com/wp-content/uploads/2015/08/Machine-Learning-for-Programmers-Select-a-Systematic-Process-e1439699783406.png)

Select a systematic and repeatable process that you can use to deliver results consistently.

There are many great processes out there, including some older processes that you can adapt to your needs.

For example:

-   [Knowledge Discovery in Databases](https://machinelearningmastery.com/what-is-data-mining-and-kdd/) (KDD), [which I have adapted here](https://machinelearningmastery.com/process-for-working-through-machine-learning-problems/)
-   [CRISP-DM](https://en.wikipedia.org/wiki/Cross_Industry_Standard_Process_for_Data_Mining)
-   [OSEMN](https://machinelearningmastery.com/how-to-work-through-a-problem-like-a-data-scientist/)
-   others…

Pick or adapt a process that works best for you and meets the requirements above.

### 2. Mapping of “_Best of Breed_” Tools onto Your Process

Machine learning tools and libraries come and go, but at any single point in time you have to use something that best maps onto your chosen process of delivering results.

You don’t want to evaluate and select any old algorithm or library, you want the so-called “_best of breed_” that is going to give you fast, reliable and high-quality results and automate as much of your process that you can afford.

Again, you are going to have to make these selections yourself. If you ask anyone, you’re going to hear their biases, often the latest tool they’re using.

I have my own biases, and I like to use different tools and platforms for different types of work.

For example, in the scenarios listed above, I would advise the following best of breed tools:

-   **One-off predictive model**: The [Weka platform](https://machinelearningmastery.com/how-to-run-your-first-classifier-in-weka/), because I can load a CSV, design an experiment and get the best model in no time at all without a line of programming ([see my mapping onto the process](https://machinelearningmastery.com/template-for-working-through-machine-learning-problems-in-weka/)).
-   **Embedded predictive model**: Python with [scikit-learn](https://machinelearningmastery.com/a-gentle-introduction-to-scikit-learn-a-python-machine-learning-library/), because I can develop the model in the same language in which it is deployed. IPython is a great way to demonstrate your pipeline and results to the broader team. A MLaaS is also an option for bigger data.
-   **Deep-dive model**: [R](https://machinelearningmastery.com/how-to-get-started-with-machine-learning-algorithms-in-r/) with the [caret package](https://machinelearningmastery.com/caret-r-package-for-applied-predictive-modeling/), because I can quickly and automatically try a lot of state-of-the-art models and devise more and more elaborate feature selection, feature engineering and algorithm tuning experiments using the whole R platform.

In reality, these three tools bleed across the three scenarios depending on the specifics of a situation.

![Machine Learning for Programmers - Select Tools](https://machinelearningmastery.com/wp-content/uploads/2015/08/Machine-Learning-for-Programmers-Select-Tools-e1439699936331.png)

Map your preferred machine learning tools onto your chosen systematic process for working through problems.

Like development, you need to study your tools to get the most from them. You also need to keep your ear to the ground and jump to newer better tools if and when they are available, forever adapting them to your repeatable process.

### 3. Targeted Practice with Semi-Formal Work Product

You get good at development by practicing – by developing lots of software. Use this familiar approach to get good at machine learning. The more of the process you practice in each project, the better (ideally, work problems end-to-end).

#### Carefully Select Your Practice Datasets

You want to pick datasets that are realistic rather than contrived. There are hundreds of free datasets out there of ever increasing complexity.

-   I would advise starting with small in-memory datasets from places like the [UCI Machine Learning Repository](https://machinelearningmastery.com/practice-machine-learning-with-small-in-memory-datasets-from-the-uci-machine-learning-repository/). They are well known, relatively clean and a good place to start as you feel out your new process and tooling.
-   From there, I would recommend larger in-memory datasets, like those from some [Kaggle](https://www.kaggle.com/) and [KDD cup](http://www.sigkdd.org/kddcup/index.php) competitions. They are little more dirty and require you to flex work on more and different skills.

Stick with tabular data, this is what I advise all of my students.

Working with image and text data are new and different fields in their own right (computer vision and natural language processing respectively) that require you to learn specialized methods and tooling to those fields. If these are types of problems you want or need to work then it might be best to start there, and there are great resources available.

I go into a lot more detail on how to do targeted practice in the post “[Practice Machine Learning with Small In-Memory Datasets from the UCI Machine Learning Repository](https://machinelearningmastery.com/practice-machine-learning-with-small-in-memory-datasets-from-the-uci-machine-learning-repository/)“.

#### Write-Up Your Results and Build A Public Portfolio of Work

Create and retain semi-formal outcomes (I refer to outcomes as “work product”) from each project. By this I mean, write up what you did and what you learned into some kind of standalone document so that you can refer back and leverage the results on future and following projects.

This is akin to keeping a directory for each programming project as a developer and reusing code and ideas from previous projects. It speeds up the journey a lot, and I strongly recommend it.

Keep any scripts, code and generated images, but it is also important to write up your findings. Think of it as akin to comments in your code. A standalone write-up could be a simple PPT or text file, or as elaborate as a presentation at a meet-up or video on YouTube.

![Machine Learning for Programmers - Targeted Practice](https://machinelearningmastery.com/wp-content/uploads/2015/08/Machine-Learning-for-Programmers-Targeted-Practice-e1439699993334.png)

Work through and complete discrete projects, write up results and build a portfolio of projects.

Save each project in a public version control repository (like [GitHub](https://github.com/)) so that other beginners can learn from you and extend your work. Link to the projects from your blog, LinkedIn or wherever and use the public portfolio to demonstrate your growing skills and capabilities.

See more on this important idea in my post titled “[Build a Machine Learning Portfolio: Complete Small Focused Projects and Demonstrate Your Skills](https://machinelearningmastery.com/build-a-machine-learning-portfolio/)“.

A portfolio of public GitHub repositories is fast becoming the resume in the hiring process at companies that actually care about skills and delivering results.

## Yes, This Approach Is Tailored For Developers

What we have laid out above is an approach that you can use as a developer to learn, get started and make progress in machine learning.

It’s natural you may have some doubts about whether this approach is really suited to you. Let me address some of your concerns.

### You do not need to write code

You may be a web developer or similar where you do not write a lot of code. You can use this approach to get started and apply machine learning. Tools like [Weka](https://machinelearningmastery.com/how-to-run-your-first-classifier-in-weka/) make it easy to devise machine learning experiments and build models without any programming at all.

Writing code can unlock more and different tools and capabilities, but it is not required, and it does not need to come first.

### You do not need to be good at mathematics

Just like development where you don’t need to know a thing about computability or [Big O notation](https://en.wikipedia.org/wiki/Big_O_notation) to write code and ship useful and reliable software, you can work through machine learning problems end-to-end without a background in statistics, probability and linear algebra.

It is important to note that we do not start with theory, but we do not ignore it. Dive in and pull out what you need on a method or algorithm, when you need it. In fact, you won’t be able to hold yourself back. The reason is, working machine learning problems is addictive and consuming. In the pursuit of getting better results and more accurate predictions, you will draw from any resources you can find, learning just enough to extract the nuggets of wisdom for you to apply on your problem.

If your goal is to master the theory, this approach is slower and less efficient. And this is why it so uncomfortable when seen through that lens. When viewed from the goal of being a developer that does machine learning, it makes a lot of sense.

### You do not need a higher degree

There are no gatekeepers to this knowledge. It’s all available and you can study it yourself, today, now. You do not need to trade a lot of time and money for a degree before you can start working on machine learning problems.

If you heart is set on getting that higher degree, why not just start working on machine learning problems first and take a look at a degree in a few weeks or months after you have a small portfolio of completed projects built up. You will have a much clearer idea of the extent of the field and the parts you like.

I did go back and get those higher degrees. I love doing research, but I love working real problems and delivering results that clients actually care about a whole lot more. Also, I was working machine learning problems before I started the degree, I just didn’t realize I already had the resources and a path in front of me.

It’s one of the reasons I’m so passionate to convince developers like you that you have what you need to get started right now.

![Machine Learning for Programmers - Limiting Beliefs2](https://machinelearningmastery.com/wp-content/uploads/2015/08/Machine-Learning-for-Programmers-Limiting-Beliefs2-e1439700549669.png)

It is so very easy to come up with excuses to not get started in machine learning.

### You do not need big data

Machine learning algorithms were developed and are best understood on small data. Data small enough for you to review in MS Excel, to load into memory and to work through on your desktop workstation.

Big data != machine learning. You can build predictive models using big data, but see this as a specialization of your skill set to a domain. I generally advise my students to start with small in memory datasets when starting in machine learning.

If big data machine learning is the area you want to work, then start there.

### You do not need a desktop supercomputer

It is true that some of the state-of-the-art algorithms like deep learning require very powerful bazillion-core GPUs. They are powerful and exciting algorithms. They are also algorithms that work on smaller problems that you can compute with your desktop CPU.

You do not need to hold off getting started in machine learning until you have access to a big-fast computer.

Before you go off and buy a desktop supercomputer or rent very large [EC2 instances](https://aws.amazon.com/), it might be worth spending some time learning how to get the most from these algorithms on smaller better-understood datasets.

### You do not need a lot of time

We all have busy lives, but if you really want something you need to put in the time.

I’ve said it before, working machine learning problems is addictive. If you get caught up in machine learning competitions you will gladly sacrifice a month of evening television to squeeze a few more percent from your algorithm.

That being said, if you start small with a clear process and a best of breed tool, you can work a dataset from end-to-end in an hour or two, perhaps spread over one or two nights. A few of these and you have a beachhead on a portfolio of completed machine learning projects that you can begin to leverage on larger and more interesting problems.

Break it down into snack-size tasks on your Kanban board and make the time to get started.

## Biggest Mistakes Developers Make and How To Avoid Them

I have been giving variations on this advice for close to two years now since I launched Machine Learning Mastery. Over that time I’ve seen five common pitfalls that I want you to avoid.

1.  **Not Taking Action**: It’s all laid out and yet I see so many developers not take action. It is so much easier to watch TV or read news than to build a new and valuable skill in a fascinating field of study. You can lead a horse to water…
2.  **Picking Problems that are Too Big**: I commonly see the first or second dataset a developer selects to work on being too difficult. It’s too large, too complex or too dirty and they’re not ready for the challenge. The awful thing is that the “failure” kills motivation and the developer flunks out of the process. Pick small problems that you can finish and write up in 60 minutes. Do that for a while before you take on something bigger.
3.  **Implementing Algorithms from Scratch**: We have algorithm implementations. It’s done. At least done enough for you to do interesting things for the next few years. If your goal is to learn how to develop and deliver reliable and accurate predictive models, do not spend time implementing algorithms from scratch, use a library. On the other hand, if you want to focus on implementing algorithms, then clearly make this your objective and focus in on it.
4.  **Not Sticking to a Process**: As with agile software development, if you deviate from the process, the wheels can come off your project pretty quickly and the result is often a big mess. Sticking to a process from start-to-finish that systematically works through a problem end-to-end is key. You can revisit “_that interesting thing you found…_” as a follow-up mini-project (an “_ideas for follow-up work_” section in your write-up), but finish the process and deliver.
5.  **Not Using Resources**: There are many great papers, books and blog posts on machine learning. You can leverage these resources to improve your process, usage of tools and accuracy of your results. Use third party resources to get more from your algorithm and your dataset. Get ideas for algorithms and framings of the problem. A nugget of wisdom can change the course of your project. Remember, if you adopt a top-down process, the theory has to come in at the back-end. Take the time to understand your final models.

Don’t let any of these happen to you!

## Your Next Step

We have covered a lot of ground and I hope I am starting to convince you that you can get started and make progress in machine learning. That a future in which you are a developer that can do machine learning is very real and very obtainable.

Your very next steps are:

1.  Select a process ([or just use this one](https://machinelearningmastery.com/process-for-working-through-machine-learning-problems/)).
2.  Select a tool or platform ([or just use this one](https://machinelearningmastery.com/how-to-run-your-first-classifier-in-weka/)).
3.  Select your first dataset ([or just use this one](https://archive.ics.uci.edu/ml/datasets/Iris)).
4.  Report back in the comment below and execute!