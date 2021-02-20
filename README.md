# **Biden vs. Trump: An Empirical Bayesian Approach.**

## Introduction 
In 2016 Donald John Trump became the president of the United States against all odds, many prominent election research organisations gave the then contender Hillary Clinton a higher chance of winning, with confident predictions in favor of the former secretary of state ranging around eighty to ninety percent, nevertheless Donald Trump emerged as the winner. 

### Bayesian Statistics
The 2016 presidential election is proof that elections can be notoriously difficult to predict acurately. However, certain techniques such as Bayesian statistics has been known to produce more accurate results. The core idea behind bayesian methods is to update an uninformed/best-guess judgement based on new information/data. 

### Assumptions
1. A key assumption is that the distribution of votes in the population and its sample is aproximately normal. This of course comes with its own set of assumptions. for more click on [this link](https://en.wikipedia.org/wiki/Normal_distribution)


### Polling Data
The data we use to model the election was gotten from opinion polls conducted by various organisations. It was sourced from FiveThirtyEight a popular data journalism platform. A little cleaning will be neccesary to ensure the integrity of the data.

### Modelling The Outcome
Earlier, I mentioned bayesian statistics, here i will go into futher detail. As i said earlier bayesian methods enable us to make decisions by factoring new information, as such, this methods allow us to model several levels of varibility as we would "new information". Here and throughout the analysis we would assume that the outcome of the elections will not be affected by other candidates other than Trump and Biden.


For the purpose of this analysis we would denote the true proportion of Biden voters as $p$ and the spread as: $d$. We can make a priori(uninformed) estimate of the spread, denoted as $\mu$. We assume that $\mu$ which is an priori estimate of the spread is assumed to be approximately normal with a standard error of $\tau^2$. Represented as, 

$$ d\ \sim\ N(\mu,\ \tau^2).$$ 

While the following formular represents randomness due to sampling and pollster effect:

$$ Y|d \sim N(d,\ \sigma^2).$$


The spread is the difference between the proportions observed in our data, this can be denoted mathematically as:         
$$ d = p\ -\ (1-p),$$
$$ d = 2p\ - \ 1.$$

Therefore, p can be derived as,
$$ p = \frac {d + 1} {2} $$

we can derive an estimate of $p$ from the polling data represented as $\hat X$, and use this to compute a standard deviation of the observed data.

### Conclusion
Here we see that Biden wins about 80% of the time in our simulation of 10000 iterations.

#### ***Note***
Predicting elections is not straight forward, in 2016 most people predicted that Hillary clinton will with overwhelming odds, technically speaking you can only call an election if it falls within a predetermined confidence interval. Famous mathematians and quantitative analyst have long quarrelled about the soundness of the method. Nevertheless, this method or a slightly more complex variation of it is championed by top poll agregators.
