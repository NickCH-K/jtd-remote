---
title: p-value
nav_order: 2
---

# p-value

Begin with (1) a set of assumptions about the true underlying process that generated the data, also known as the null hypothesis,[^1] (2) an actual data set.

Under the assumption that your null hypothesis is perfectly true, the *p-value* is the probability that you would observe the actual data that you observed *or* any data that is as unlikely, or even less likely, than what you observed.

Usually, this is stated in terms of a set of parameters or a test statistic. For example, "the null hypothesis is that the Pearson correlation coefficient between X and Y is 0, but in my data I estimated a correlation of .15." In this case, we can restate the above definition as "under the assumption that the correlation is equal to 0, the *p-value* is the probability of observing a correlation that is .15 or higher, or -.15 or lower" or "under the assumption that the correlation is equal to 0, the *p-value* is the probability of observing a correlation as different from 0 as .15 is, or even more extremely different than that."

In application, a low *p-value* can be interpreted as "it is unlikely that I would have seen the data we actually see (or more extremely different from the null) if the null hypothesis were true. So either the null is true and something unlikely has occurred, or some aspect of the null hypothesis is false." 

[^1]: The null hypothesis is usually stated in terms of a set of parameter values, for example "the mean of X is 5" or "the Pearson correlation coefficient between X and Y is 0". However, it also implicitly includes *every* assumption made about the data generating process, such as how variables are distributed, or the choice of overarching model.

# Common incorrect definitions

These are common ways that people talk about p-values. None of them is accurate. They are accompanied by very brief explanations of why they are not accurate.

* ❌ "*p* is the probability that the result occurred by random chance." *Why it's wrong*: *p* is the probability that the result, **or a more extreme result,** occurred by random chance **assuming that the null hypothesis is true.** Without these two additions, this definition is wrong. The latter addition is especially important because the null contains all sorts of assumptions beyond just "the effect is zero" (or whatever value).
* ❌ "The lower *p* is, the more likely it is that the result is correct" *Why it's wrong*: A lower *p*-value can help you determine that 
