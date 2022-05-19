## Complex Problems

<mark style="background: #FF5582A6;">Writing programs in a computer can be summarized as ***automating procedures on input data to create output artifacts. Almost always, they are linear, procedural and logical.***</mark> A traditional program is written in a programming language to some specification, and it has properties like:

-   <u>You know or can control the inputs to the program</u>
-   <u>You can specify how the program will achieve its goal</u>
-  <u> **You can map out what decisions the program will make and under what conditions it makes them**</u>
-   <u>**You can test your program and be confident that because the inputs and outputs are known and all conditions have been exercised the program will achieve its goal**</u>

<mark style="background: #FF5582A6;">There are some problems that you can represent in a computer that you cannot write a traditional program to solve. They resist a procedural and logical solution.</mark> They have properties such as:

-   The **scope of all possible inputs is not known beforehand**
-   You **cannot specify how to achieve the goal of the program, only what that goal is**
-   You **cannot map out all the decisions the program will need to make to achieve its goal**
-   You **can collect sample input data for the program**

Problems like this resist traditional programmed solutions because manually specifying a solution would require a disproportionate amount of resources.

You are probably a programmer, and you might be an experienced programmer. This might sound very odd, even unbelievable. <mark style="background: #FF5582A6;">As programmers, we believe as long as we can define what a program needs to do, we are confident we can define how a program can achieve that goal. This is not always the case.</mark> 

## Spam Filter Example

An example of an every-day decision problem that resists a manually defined solution is the discrimination of spam email from non-spam email.

How would you write a program to filter emails as they come into your email account and decide whether to put them in the spam folder or the inbox folder?

[![Spam/Non-Spam Discrimination](https://machinelearningmastery.com/wp-content/uploads/2013/12/spam-nonspam.jpg)](https://machinelearningmastery.com/wp-content/uploads/2013/12/spam-nonspam.jpg)


Some of my thoughts on how to do this are:

-   I’d collect examples of emails I knew to be spam or not-spam
-   I’d read the emails I had collected and write down any patterns I saw in either group
-   I’d think about abstracting those patterns into more general rules I could program
-   I’d look for emails that I could safely and quickly categorize as either spam or non-spam
-   I’d write tests for my program to ensure it was making accurate decisions
-   I’d monitor the deployed system and keep an eye on the decisions it was making

```ad-warning
I could write a program to do this, and so could you. It would take a lot of time. A lot of emails would have to be read. The problem would need to be thought about very deeply. It would take a lot of development and testing time before the system could be trusted enough to be put into operations. Once in operations, there would be so many hard coded rules that were specific to the email I had read that it would be a maintenance nightmare.
```

The process above also describes a machine learning solution to the problem of discriminating spam email from non-spam email. The punch line is that machine learning methods can automate the process for you.

```ad-tip
title: **Pro Tip**:
Approaching complex problems in this way is an incredibly valuable skill that will serve you well later on in preparing data and selecting the right machine learning method. [[III. How would I solve the problem|Thinking through the process of “how would I manually write a program to solve this” is a master skill that is often overlooked and forgotten by professionals.]]
```