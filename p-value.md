---
title: p-value
nav_order: 2
---

# p-value

Begin with (1) a set of assumptions about the true underlying process that generated the data, also known as the null hypothesis,[^1] (2) an actual data set.

Under the assumption that your null hypothesis is perfectly true, the *p-value* is the probability that you would observe the actual data that you observed *or* any data that is as unlikely, or even less likely, than what you observed.

Usually, this is stated in terms of a set of parameters or a test statistic. For example, "the null hypothesis is that the Pearson correlation coefficient between X and Y is 0, but in my data I estimated a correlation of .15." In this case, we can restate the above definition as "under the assumption that the correlation is equal to 0, the *p-value* is the probability of observing a correlation that is .15 or higher, or -.15 or lower" or "under the assumption that the correlation is equal to 0, the *p-value* is the probability of observing a correlation as different from 0 as .15 is, or even more extremely different than that."

In application, a low *p-value* can be interpreted as "it is unlikely that I would have seen data like this if the null hypothesis were true. So either something unlikely has occurred, or some aspect of the null hypothesis is false." 

[^1]: The null hypothesis is usually stated in terms of a set of parameter values, for example "the mean of X is 5" or "the Pearson correlation coefficient between X and Y is 0". However, it also implicitly includes *every* assumption made about the data generating process, such as how variables are distributed, or the choice of overarching model.

## Basic example

MOVE THIS ALL TO A SINGLE PAGE.

For example, perhaps your null hypothesis consists of three assumptions: (a) taking Heads = 1 and Tails = 0, the expected result from averaging a set of coin flips would be .5 (50% Heads, 50% Tails), (b) the coin flips are independent of each other, and (c) the distribution of coin flips can be explained by the [binomial distribution](https://en.wikipedia.org/wiki/Binomial_distribution). For your observed data, you actually flip four coins and observe three Heads and one Tails (your average is .75).

Using the independent binomial distribution, we can calculate that, if the average is truly .5, then there is a 25% chance of getting .75 in four flips. So under the null hypothesis, there is a 25% chance of observing the data that we did actually observe.

Observing one Heads and three Tails (.25) would be exactly as much of a deviation from .5 as .75 is, and also has a 25% chance of occurring, assuming the null hypothesis is true. Observing four Heads (1), or four Tails (0), would be *even more* extremely different from .5, and each has a 6.25% chance of occurring, assuming that the null hypothesis is true.

The *p-value* is the probability of what we observed (25%) plus the probability of observing something as extreme or more extreme than that (25% + 6.25% + 6.25%). The *p-value* in this case is .25 + .25 + .0625 + .0625 = .625. There is a 62.5% chance of observing data as extreme as we saw, or more extreme, under the assumption that your null hypothesis is true. 

# Common incorrect definitions

These are common ways that people talk about p-values. None of them is accurate. They are accompanied by very brief explanations of why they are not accurate.

* ❌ A *Explanation*
* ❌ B *Explanation*
