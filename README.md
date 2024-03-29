# **Biden vs. Trump: An Empirical Bayesian Approach.**

## Introduction 
In 2016 Donald John Trump became the president of the United States against all odds, many prominent election research organisations gave the then contender Hillary Clinton a higher chance of winning, with confident predictions in favor of the former secretary of state ranging around eighty to ninety percent, nevertheless Donald Trump emerged as the winner. 

### Bayesian Statistics
The 2016 presidential election is proof that elections can be notoriously difficult to predict acurately. However, certain techniques such as Bayesian statistics have been known to produce more accurate results. The core idea behind bayesian methods is to update an uninformed/best-guess judgement based on new information/data. 

### Assumptions
1. A key assumption is that the distribution of votes in the population and its sample is aproximately normal. This of course comes with its own set of assumptions. for more click on [this link](https://en.wikipedia.org/wiki/Normal_distribution)


### Polling Data
The data we use to model the election was gotten from opinion polls conducted by various organisations. It was sourced from FiveThirtyEight a popular data journalism platform. A little cleaning will be neccesary to ensure the integrity of the data.

### Conclusion
Here we see that Biden wins about 80% of the time in our simulation of 10000 iterations.

#### ***Note***/***Disclaimer***:
Predicting elections is not straight forward, in 2016 most people predicted that Hillary clinton will win with overwhelming odds, technically speaking you can only call an election if it falls within a predetermined confidence interval. Famous mathematians and quantitative analysts have long quarrelled about the soundness of the bayesian simulation approach used in this project. Nevertheless, this method or slightly more complex variations of it, is championed by top poll agregators.

### References
**Data**: FiveThirtyEight

**Introduction to Data Science: Data Analysis and Prediction Algorithms with R - Rafael Irizazzy**

*Professor Rafeal's book is not only the inspiration for this project but it also contains some of the domain knowledge that is hard coded into the simulation. i.e We a included a bias term and assumed that certain counties will always vote a certain way.* 


