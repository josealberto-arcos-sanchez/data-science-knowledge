# General Data Science Knowledge

## Index

1. [Always use all the domain knowledge at your disposal](#always-use-all-the-domain-knowledge-at-your-disposal)
2. [Use a checklist](#use-a-checklist)

---

### Always use all the domain knowledge at your disposal

Models and algorithms are silly. They know nothing, and they can just learn what we show to them. So, in order to obtain the most from them, we need to make things easy. 

**Example 1**  
If you give a model a datetime as a feature, it will be difficult for the model to use all the information that variable contains. The model doesn't know that we, humans, have defined cyclical periods of time that influence our behavior (days, weeks, months, years,...). So, how can we show it that kind of information? We can create extra features containing the day of the week, day of the month, hour of the day, etc. This way, the model can learn relationships concerning cyclical patterns. 

**Experience: Kaggle Santa 2018 (optimization)**  
In this competition I tried a direct (dumb) approach consisting on using Simulated annealing to solve the problem from scratch. The generation of the initial solution was random. The generation of new individuals was random. How much information I was discarding! 

---

### Use a checklist

There are lots of thing to check in a data science project. Use a [checklist](https://blog.k2datascience.com/essential-checklist-for-any-data-analysis-or-science-project-7c4fa924e563) to ensure you do everything is needed!
