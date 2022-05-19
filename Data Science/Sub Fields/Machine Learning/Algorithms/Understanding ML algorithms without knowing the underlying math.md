Learning a machine learning algorithm can be overwhelming. There are so many papers, books and websites describing how the algorithm works mathematically and textually. If you are really lucky you might find a pseudocode description of the algorithm.

If you are really really lucky you might find some suggested ways to configure the method for different situations. These descriptions are rare and typically buried deep in the original publication or in technical notes by the original authors.

A fact you learn quickly when you want to implement a method from research papers is that algorithms are almost never described in sufficient detail for you to reproduce them. The reasons vary, from the micro-decisions that are left out of the paper, to whole procedures that are summarized ambiguously in text, to symbols that are used inconsistently.

## Piece it Together

To understand an algorithm you have to piece together an understanding yourself from disparate descriptions. This is the only tactic that I have found to be successful.

Disparate descriptions means resources such as the original descriptions of the method in the primary sources as well as authoritative secondary interpretations made of original descriptions in review papers and books.

It is common for there to be prototype implementations of a method released with the primary sources and reading this code (typically C, FORTRAN, R or Matlab) can be very enlightening for the details you need to reproduce an algorithm.

## Algorithm Descriptions

An algorithm is an island of research and in all reality it can be difficult to pin down the canonical definition. For example, is it the version described in the primary source or is it the version that includes all the fixes and enhancements that are “best practice”.

A solution is to consider a given algorithm from multiple perspectives, each of which can serve a different purpose. For example, the abstract information processing description of the algorithm could be realized by a variety of different specific computational implementations.

I like this approach because it defends the need to telescope in on a specific case of the algorithm from many possible cases at each step of the description while also leaving the option open for the description of variations.

There are many descriptions you could use of varying specificity depending on your needs. Some that I like to use include: inspiration for the algorithm, metaphor or analogy for the strategy, information processing objectives, pseudocode and code.

## Algorithm Prescriptions

When I started my own research projects, I thought the answer to this problem was to read everything on an algorithm and create the definitive implementation in code. Nice idea perhaps, but code is just one way to communicate an algorithm, and it is limited.

There is more to an algorithm description than the computation. There is meta information around an algorithm that can be invaluable for certain use cases.

For example, usage heuristics for an algorithm are embedded in papers. Having a summary of usage heuristics collected together in one place can mean the difference of getting a good enough result quickly and running sensitivity analysis on the algorithm for days or weeks.

Other examples include the standard experimental datasets used to test the algorithm, the general classes of problem to which the algorithm is suited, and known limitations that have been identified and described for the algorithm.

## Design an Algorithm Description Template

An algorithm description template provides a structured way for you to learn about a machine learning algorithm.

You can start with a blank document and list out the section headings for the types of descriptions you need of the algorithm, for example applied, implementation, or your own personal reference cheat sheet.

To figure out what sections to include in your template, list out questions you would like to answer about the algorithm, or algorithms if you are looking to build up a reference. Some questions you could use include:

-   What is the standard and abbreviations used for the algorithm?
-   What is the information processing strategy of the algorithm?
-   What is the objective or goal for the algorithm?
-   What metaphors or analogies are commonly used to describe the behavior of the algorithm?
-   What is the pseudocode or flowchart description of the algorithm?
-   What are the heuristics or rules of thumb for using the algorithm?
-   What classes of problem is the algorithm well suited?
-   What are common benchmark or example datasets used to demonstrate the algorithm?
-   What are useful resources for learning more about the algorithm?
-   What are the primary references or resources in which the algorithm was first described?

Once you have settled on some questions, turn them into section headings.

For each section heading clearly define the requirements of the section and the form that the description in that section will take. I like to include motivating questions for each section that once answered will satisfy the section at the minimum level of detail.

## Start Small and Build it Up

The beauty of this approach is that you don’t need to be an expert in the algorithm or in research. As long as you can find some resources that mention the algorithm, you can start to capture notes about an algorithm in the template.

You can start really simply and collect high-level descriptions of the algorithm, its names and abbreviations and the resources you have found and what they talk about. From here you can decide to expand the description further, or not.

You will end up with a one-to-two page description of the algorithm very quickly.

## I Use It

I’ve been using algorithm templates for a long time. Some examples where I have found this strategy practically useful include:

-   Implementing machine learning algorithms using a descriptive-focused template.
-   Applying a machine learning algorithm using an applied-focused template.
-   Building a catalog of algorithms to use and refer to using a general purpose template.

---

# How to Build and Maintain a List of Algorithms

The answer is to build your own personal list of machine learning algorithms.

I’m a list maker, and this method really lights up my brain.

Open a text file, word document or spreadsheet and start listing down the names of algorithms. It’s that simple. You can also list the general class to which the algorithm belongs and the general types of problems that it can address.

Define your own categories. This list is a tool to help you understand and navigate the machine learning tools at your disposal. Customize the list to include the algorithm details that you care about.

### Examples of Algorithm Lists To Create

Below are 10 examples of machine learning algorithm lists that you could create.

-   Regression algorithms
-   SVM algorithms
-   Data projection algorithms
-   Deep learning algorithms
-   Time series forecasting algorithms
-   Rating system algorithms
-   Recommender system algorithms
-   Feature selection algorithms
-   Class imbalance algorithms
-   Decision tree algorithms

### Tips for Great Algorithm Lists

Creating a list of algorithms is relatively easy. The hard part is knowing why you want the list. The “_why_” will help you define the type of list you want to create and the algorithm properties you want to describe in your list.

Start with the current project you are working on or your current interests. For example, if you are working on a time series or image classification problem, list all the algorithms that you could apply to that problem. If you are deeply interested in Support Vector Machines, list all the variations of SVM that you can find.

Don’t try to create the perfect list in one sitting. Create it and keep adding to it over days and weeks. It is a useful resource that you can turn back to again and again and add to as your knowledge and experience grows.

In summary, 5 tips for creating great algorithm lists are:

-   Start with why you want the list and use that to define the type of list to create.
-   Only capture the algorithm properties you actually need, keep it as simple as possible.
-   Start with a current project or interest and create a list of related algorithms.
-   Don’t aim for abstract perfection, the list is for you and your needs alone.
-   Add to your list over time and expand it as your skills and experience grow.

### When To Use An Algorithm List

Algorithm lists are more valuable than you think.

For example, you can use it as a technique when tackling a problem type that you have never worked on before, such as recommender systems, face detection or rating systems. A simple algorithm list gives you a list of things to try.

When working on a familiar problem, your prior biases often limit the results that you can achieve. A list of algorithms relevant to a problem domain can get you unstuck and even push you to achieve new and better results. That does not mean you should try all algorithms you can find, you still require reasoned and systematic application. Nevertheless, a list can provide a useful starting point.

Algorithm lists are a tool, but you can take them further. To make effective use of machine learning algorithms, you need to [study them](https://machinelearningmastery.com/how-to-study-machine-learning-algorithms/ "How to Study Machine Learning Algorithms"), [research them](https://machinelearningmastery.com/how-to-research-a-machine-learning-algorithm/ "How to Research a Machine Learning Algorithm"), and even [describe them](https://machinelearningmastery.com/how-to-learn-a-machine-learning-algorithm/ "How to Learn a Machine Learning Algorithm"). This is a natural extension for the algorithm list method and your lists can provide the basis for your self-study curriculum.

You could start by collecting additional properties about each algorithm and expand your list into a mini-encyclopaedia of algorithms, with one page per algorithm. I use an algorithm description template and focus on template elements that I will find useful as I refer back to the descriptions in the future, such as pseudo code and usage heuristics.

In summary, 3 examples of when you can use an algorithm list are:

-   When you start working on a new class of problem.
-   When you are stuck or looking for algorithms to try on an existing problem.
-   When you are looking for algorithms to describe in more detail or research.

## Anyone Can Create Machine Learning Algorithm Lists

You don’t need to deep dive into machine learning textbooks or open source libraries. A simple google search or browse of wikipedia will uncover many algorithm names to start-off your list.

If you are stuck on what to create for your first list, pick one of the examples above or browse a site like [DataTau](http://www.datatau.com/) and pick a class of algorithm to list mentioned in an article or article title.

Again, you do not have to list every algorithm that you could list, narrow your scope to those algorithms in the libraries and tools you prefer. You don’t need to list every permutation of every algorithm, for example, you could focus on one aspect of an algorithm, such as the kernel functions for an SVM or the transfer functions for a neural network.

Don’t list all possible features of each algorithm. Stick to just the name and maybe the general class of algorithm and general types of problems for which it can be used. If you want to go deeper into an algorithm, consider the [algorithm description method and template](https://machinelearningmastery.com/how-to-learn-a-machine-learning-algorithm/ "How to Learn a Machine Learning Algorithm") described previously.

You don’t need to understand the algorithms yet and you don’t need to be an academic. This is a beachhead that you are taking to expand your idea of what is out there, to overcome overwhelm and to finally to provide a point of departure on your journey deeper into applied machine learning.

## Action Steps

In this post you learned about the simple tactic of creating lists of machine learning algorithms.

You discovered that this simple tactic can help you to overcome algorithm overwhelm and to help get you unstuck from the dangers of having favorite algorithms.

Your action step for this post is to create your first algorithm list. Pick something small, like a subclass of an algorithm. Pick something fun, like an algorithm that is hot right now.

Share your list if you like (or what your list is about), it would help to motivate others.

---

# 1) Learn Theory Last, Not First

The way machine learning is taught to developers is crap.

It is taught bottom-up. This is crap if you are a developer who is primarily interested in using machine learning as a tool to solve problems rather than being a researcher in the field.

The traditional approach requires that you learn all of the prerequisite mathematics like linear algebra, probability and statistics before learning the theory of algorithms. You’re lucky if you ever go near a working implementation of an algorithm or discuss how to work a problem end-to-end and deliver a working, reliable and accurate predictive model.

Why not to use a top-down approach to learning machine learning.? In this approach we start with:
1) learning a systematic process for working through problems end-to-end
2) map the process onto “best of breed” machine learning tools and platforms
3) complete targeted practice on test datasets.

## The Theory is Really All About Algorithms

The field of machine learning is theory-dense.

It’s dense because there is a tradition to describe and explain concepts mathematically.

This is useful because mathematical descriptions can be very concise, cutting down on the ambiguity. They also lend themselves to analysis by leveraging the techniques from the context in which they are described (e.g. a probabilistic understanding of a process).

A lot of these tangential mathematical techniques are often bundled in with the description of machine learning algorithms. For someone who just wants to build a superficial understanding of a method to be able to configure and apply it, this feels overwhelming. Frustratingly so.

It is frustrating if you do not have the grounding to be able to parse and understand the description of an algorithm. It’s frustrating because coming from a field like computer science, algorithms are described all the time, but the difference is the descriptions are intended for fast comprehension (e.g. for [desk checking](https://en.wikipedia.org/wiki/Informal_Methods_(Validation_and_Verification)#Desk_checking)) and implementation.

We know that for example when learning what a [hash table](https://en.wikipedia.org/wiki/Hash_table) is and how to use it, that we almost never need to know the specifics of the hashing function in our day-to-day. But we also know what a hashing function is and where to go to learn more about hashing function specifics and how to write your own. Why can’t machine learning work like that?

The bulk of the “theory” one encounters in machine learning is related to machine learning algorithms. If you ask any beginner about why they are frustrated with the theory, you will learn that it is in relation to learning how to understand or use a specific machine learning algorithm.

Here, algorithms is more broad than a process for creating a predictive model. It also refers to algorithms for selecting features, engineering new features, transforming data and estimating the accuracy of a model on unseen data (e.g. cross validation).

So, learning theory last, really means learning about machine learning algorithms.

## A Compulsion To Dive Into Theory

I generally advise targeted practice on well known machine learning datasets.

This is because well known machine learning dataset, like those on the UCI Machine Learning Repository are easy to work with. They are small so they fit into memory and can be processed on your workstation. They are also well studied and understood so you have a baseline for comparison.

You can learn more about targeted practice of machine learning datasets in the post “[Practice Machine Learning with Small In-Memory Datasets from the UCI Machine Learning Repository](https://machinelearningmastery.com/practice-machine-learning-with-small-in-memory-datasets-from-the-uci-machine-learning-repository/)“.

Understanding machine learning algorithms fits into this process. The reason is in the pursuit of getting results on standard machine learning algorithms you are going to run into limitations. You are going to want to know how to get more out of a given algorithm or to know more about how to best configure it, or how it actually works.

This need to know more and curiosity will drive you into studying the theory of machine learning algorithms. You will be compelled to piece together an understand of the algorithms in order to achieve better results.

We see this same effect in young developers from varied backgrounds that end up eventually studying the code of open source projects, textbooks and even research papers in order to hone their craft. The need to being a better more capable programmer drives them to it.

If you are curious and motivated to succeed, you cannot resist studying the theory.

## 5 Techniques To Understand Machine Learning Algorithms

The time will come to dive into machine learning algorithms as part of your targeted practice

When that time comes, there are a number of techniques and template that you can use to short cut the process.

In this section you will discover 5 techniques that you can use to understand the theory of machine learning algorithms, fast.

### 1) Create Lists of Machine Learning Algorithms

When you are just starting out you may feel overwhelmed by the larger number of algorithms available.

Even when spot testing algorithms, you may be unsure of which algorithms to include in your mix (hint, be diverse).

An excellent trick you can use when starting out is to keep track of the algorithms you read about. These lists can be as simple as the name of the algorithm, and can increase in complexity as you interest and curiosity build.

Capture details like the problem type to which they are suited (classification or regression), related algorithms, and taxonomic class (decision tree, kernel, etc.). When you see the name of an algorithm that is new to you, add it to your list. When you start a new problem, try some algorithms you have never used before. Mark a check next to algorithms you have used before. And so on.

Controlling the names of algorithms in lists gives you power. This ridiculously simple tactic can help you get on top of the overwhelm. Examples of where your simple algorithm lists can save you a lot of time and frustration are:

-   Ideas of algorithms to try on new and different problem types (time series, rating systems, etc.)
-   Algorithms that you can investigate to learn more about how to apply.
-   Get a handle on algorithm types by category (trees, kernels, etc.).
-   Avoid the problem of fixating on a favorite algorithm.

Start by creating lists of algorithms, open a spreadsheet and get started.

See the post “[Take Control By Creating Targeted Lists of Machine Learning Algorithms](https://machinelearningmastery.com/create-lists-of-machine-learning-algorithms/)” for more information on this tactic.

### 2) Research Machine Learning Algorithms

When you want to know more about a machine learning algorithm you need to research it.

The main reasons you will be interested to research an algorithm is to learn how to configure it and to learn how it works.

Research is not just for academics. A few simple tips can take you a long way in gathering information on a given machine learning algorithm.

The key is diversity of information sources. The following is a short list of the types of sources you can consult for information on an algorithm you are researching.

1.  Authoritative sources like textbooks, lecture notes, slide and overview papers.
2.  Seminal sources like the papers and articles in which the algorithm was first described.
3.  Leading-edge sources that describe state-of-the-art extensions and experiments on the algorithm.
4.  Heuristic sources like those that come out of machine learning competitions, posts on Q&A websites and conference papers.
5.  Implementation sources such as open source code for tools and libraries, blog posts and technical reports.

You do not need to be a PhD researcher nor a machine learning algorithm expert.

Take your time and pick over many sources collecting facts on a machine learning algorithm you are trying to figure out. Focus on the practical details you can apply or understand and leave the rest.

For more information on researching machine learning algorithms see the post “[How to Research a Machine Learning Algorithm](https://machinelearningmastery.com/how-to-research-a-machine-learning-algorithm/)“.

### 3) Create Your Own Algorithm Descriptions

Machine learning algorithm descriptions you will discover in your research will be incomplete and inconsistent.

An approach that you can use is to put together your own mini algorithm descriptions. This is another very simple and very powerful tactic.

You can design a standard algorithm description template with only those details that are useful to you in getting the most from algorithms, like algorithm usage heuristics, pseudo-code listings, parameter ranges and resource lists.

You can then use the same algorithm description template across a number of key algorithms and start to build up your own little algorithm encyclopedia that you can refer to on future projects.

Some questions you might like to use in your own algorithm description template include:

-   What are the standard abbreviations used for the algorithm?
-   What is the objective or goal for the algorithm?
-   What is the pseudo-code or flowchart description of the algorithm?
-   What are the heuristics or rules of thumb for using the algorithm?
-   What are useful resources for learning more about the algorithm?

You will be surprised at how useful and practical these descriptions can be. For example, I used this approach to write a book of nature-inspired algorithm descriptions that I still refer back to years later.

For more on how to create effective algorithm description templates, see the post “[How to Learn a Machine Learning Algorithm](https://machinelearningmastery.com/how-to-learn-a-machine-learning-algorithm/)“.

For more information on my book of algorithms described using a standard algorithm description template, see “[Clever Algorithms: Nature-Inspired Programming Recipes](http://cleveralgorithms.com/nature-inspired/index.html)“.

### 4) Investigate Algorithm Behavior

Machine learning algorithms are complex systems that are sometimes best understood by their behaviors on actual datasets.

By designing small experiments on machine learning algorithms using small datasets you can learn a lot about how an algorithm works, it’s limitations and how to configure it in ways that may transfer to exceptional results on other problems.

A simple procedure that you can use to investigate a machine learning algorithm is as follows:

1.  Select an algorithm that you would like to know more about (e.g. random forests).
2.  Identify a question about that algorithm you would like answered (e.g. the effect of the number of trees).
3.  Design an experiment to find an answer to that question (e.g. try different numbers of trees on a few binary classification problems and chart the relationship with classification accuracy).
4.  Execute the experiment and write-up your results so that you can make use of them in the future.
5.  Repeat the process.

This is one of the truly exciting aspects of applied machine learning, that through your own simple investigations you can achieve surprising and state of the art results.

For more information on how to study algorithms from their behavior, see the post “[How To Investigate Machine Learning Algorithm Behavior](https://machinelearningmastery.com/how-to-investigate-machine-learning-algorithm-behavior/)“.

### 5) Implement Machine Learning Algorithms

You cannot get more intimate with a machine learning algorithm than by implementing it.

In implementing a machine learning algorithm from scratch you will be confronted with the myriad of micro-decisions that go into a given implementation. You may decide to cover some up with rules of thumb of expose them all as parameters to the user.

Below is a repeatable process that you can use to implement machine learning algorithms from scratch.

1.  Select a programming language, one that you are most familiar with is probably best.
2.  Select an algorithm to implement, start with something easy (see below for a list).
3.  Select a problem to test your implementation on as you develop, 2D data is good for visualizing (even in Excel).
4.  Research the algorithm and leverage many and diverse sources of information (e.g. read tutorials, papers, other implementations, and so on).
5.  Unit test the algorithm to confirm your understanding and validate the implementation.

Start small and build confidence.

For example 3 algorithms that you select as your first machine learning algorithm implementation from scratch are:

-   Linear Regression using Gradient Descent
-   k-Nearest Neighbor ([see my tutorial in Python](https://machinelearningmastery.com/tutorial-to-implement-k-nearest-neighbors-in-python-from-scratch/))
-   Naive Bayes ([see my tutorial in Python](https://machinelearningmastery.com/naive-bayes-classifier-scratch-python/))

For more information on how to implement machine learning algorithms, see the post “[How to Implement a Machine Learning Algorithm](https://machinelearningmastery.com/how-to-implement-a-machine-learning-algorithm/)“.

Also see the posts:

-   “[Benefits of Implementing Machine Learning Algorithms From Scratch](https://machinelearningmastery.com/benefits-of-implementing-machine-learning-algorithms-from-scratch/)“
-   “[Don’t Start with Open-Source Code When Implementing Machine Learning Algorithms](https://machinelearningmastery.com/dont-start-with-open-source-code-when-implementing-machine-learning-algorithms/)“

## Theory is Not Just For the Mathematicians

Machine learning is not just for the mathematical elite. You can learn how machine learning algorithms work and how to get the most from them without diving deep into multivariate statistics.

**You do not need to be good at math.**

As we saw in the techniques section, you can start with algorithm lists and transition deeper into algorithm research, descriptions and algorithm behavior.

You can go very far with these methods without diving much at all into the math.

**You do not need to be an academic researcher.**

Research is not just for academics. Anyone can read books and papers and compile their own understanding of a topic like a specific machine learning algorithm.

Your biggest breakthroughs will come when you take on the persona of “_the scientist_” and start experimenting on machine learning algorithms as though they were complex systems in need of study. You will discover all kinds of interesting quirks in behavior that may not even be documented.

## Take Action

Pick one of the techniques listed above and get started.

I mean today, now.

**Unsure where to start?**

Here’s 5 great ideas of where you could start:

1.  Make a list of 10 machine algorithms for classification (take a look at my [tour of algorithms](https://machinelearningmastery.com/a-tour-of-machine-learning-algorithms/) to get some ideas).
2.  Find five books that give detailed descriptions of Random Forests.
3.  Create a five-slide presentation on Naive Bayes using your own algorithm description template.
4.  Open [Weka](https://machinelearningmastery.com/how-to-run-your-first-classifier-in-weka/) and see how the “k” parameter affects accuracy of k-nearest neighbor on the iris flowers data set.
5.  Implement linear regression using stochastic gradient descent.