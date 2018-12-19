## Index
1. [Intelligent chatbot using HMMs](#intelligent-chatbot-using-hmms)
1. [Extreme Incremental Modeling (ArcosSan method)](#extreme-incremental-modeling-arcossan-method)

---

## Intelligent chatbot using HMMs

The problem with chatbots is that they don't know what they are talking about. They also don't know what ideas they need to transmit. But that is possible!

What if we create a huge HMM whose states are "ideas", and whose samples are sentences? Each state would contain an idea, like:  
State 1: "I want something to drink"   
State 2: "I want to sleep"  
State 3: "You can find something to drink at the coffee shop"

And each of those states (ideas) would generate different samples (sentences):  
State 1 > Sentence 1: "I want something to drink" with probability 0.01  
State 1 > Sentence 2: "I want some water" with probability 0.02  
State 1 > Sentence 3: "I want a coke" with probability 0.05  
Etc  

The variability of natural language is huge, but if we focus on a particular field (a chatbot with a specific task) and reduce variability with the typical text processing pipeline, this may be doable!

Once the HMM is trained, another model would be necessary in order to link ideas. For example, the chatbot needs to know that a correct answer to State 1 is State 3.

---

## Extreme Incremental Modeling (ArcosSan method)

This is a crazy idea I want to try as soon as possible. It is inspired in Bayesian Networks and similar approaches.

When using machine learning, we usually create a set of features and throw them to a model. But I find that method quite ineffective for some projects for several reasons:
- We usually don't give the model explicit information about feature relationship, even when we know it. Something as simple as dependence or independence between features is specially interesting at this point. Causality is even better!
- We often input as much information as possible. But most of the time, we are just increasing the noise in the input.
- Interpretability. It is usually very difficult (or just impossible) to perfectly understand what's going on in our model. So we loose the ability to understand the complete pipeline!
- This way of working does not encourage the data scientist to better (deeper) understand the problem at hand.

So, I propose the following modeling method:
1. Study the problem. Understand the theory, the way things work, as best as you can.
1. Perform a deep exploratory analysis of the data set at hand.
1. Define a well-suited metric.
1. Choose the variable you consider is the most important to predict the target variable. It may not be in your data set right now! If it isn't, can you build it? You may need to create a model using external data. This model should start being a one-feature model.
1. Create a one-feature model to solve the problem. You can plot the model, so it is fully understandable!
1. Calculate the metric and save all the pipeline.
1. Choose another important variable. It may not be in your data set...!
1. Create a two-feature model to solve the problem. Understand how the new feature changes the previous model.
1. Calculate the metric and save all the pipeline. Has your model improved?
1. Repeat the process endlessly :smile: 

The final result should be:
- A deep understanding of the problem.
- A useful extended data set.
- A good model you understand quite well.

This method is also very "agile-minded". Fast and complete iterations. Each iteration finishes with a complete model, subject to be improved in later iterations.

The final model will probably be deep, as this process promotes the creation of features over other features. And each step will be composed of simple and transparent models.

One important detail is to avoid building a "greedy" model in the sense of selecting only the most likely class in each step. That may drastically reduce performance. It is better to assign probabilities to each class and to use all the classes (or at least some of them) in the subsequent calculations.

---
