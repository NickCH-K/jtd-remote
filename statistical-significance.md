---
title: Statistical Significance
nav_order: 3
---

# Statistical significance

Begin with (1) a set of assumptions about the true underlying process that generated the data, also known as the null hypothesis,[^1] (2) an actual data set, and (3) a cutoff value called "alpha".

Then, calculate the [*p-value*](https://whatpmeans.github.io/p-value.html) for this null hypothesis and data set.

The result is *statistically significant* if the *p-value* is smaller than alpha.

In other words, the *p-value* can be interpreted as "how likely it is that I would have seen the data we actually see (or more extremely different from the null) if the null hypothesis were true." In the case of a low *p-value*, either (1) the null is true and something unlikely has occurred, or (2) some aspect of the null hypothesis is false. *Statistical significance* is when "the probability that something unlikely has occurred" is small enough that the researcher rejects (1) and concludes that some aspect of the null hypothesis is false.

Note that alpha is selected by the researcher based on the probability threshold they would like to use, and statistical significance can be applied with any value of alpha between 0 and 1. While alpha = .05 is very common, there is nothing particularly special about it other than it being a common standard.

[^1]: The null hypothesis is usually stated in terms of a set of parameter values, for example "the mean of X is 5" or "the Pearson correlation coefficient between X and Y is 0". However, it also implicitly includes *every* assumption made about the data generating process, such as how variables are distributed, or the choice of overarching model.

# Common incorrect definitions

These are common ways that people talk about statistical significance. None of them is accurate. They are accompanied by very brief explanations of why they are not accurate.

* ❌ A *Explanation*
* ❌ B *Explanation*
