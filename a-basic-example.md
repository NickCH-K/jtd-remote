---
title: A Basic Example
nav_order: 5
---

# A basic example

Let's tie all these definitions together with an example that might be easier to understand than the abstract definitions. Let's base this example on coin flips.

Perhaps your null hypothesis consists of three assumptions: (a) taking Heads = 1 and Tails = 0, the expected result from averaging a set of coin flips is .5 (50% Heads, 50% Tails), (b) the coin flips are independent of each other, and (c) the distribution of coin flips can be explained by the [binomial distribution](https://en.wikipedia.org/wiki/Binomial_distribution). For your observed data, you actually flip four coins and observe three Heads and one Tails (your average is .75).

Using the independent binomial distribution, we can calculate that, if the average is truly .5, then there is a 25% chance of getting .75 in four flips. So under the null hypothesis, there is a 25% chance of observing the data that we did actually observe.

Observing one Heads and three Tails (.25) would be exactly as much of a deviation from .5 as .75 is, and also has a 25% chance of occurring, assuming the null hypothesis is true. Observing four Heads (1), or four Tails (0), would be *even more* extremely different from .5, and each has a 6.25% chance of occurring, assuming that the null hypothesis is true.

The [*p-value*](https://whatpmeans.github.io/p-value.html) is the probability of what we observed (25%) plus the probability of observing something as extreme or more extreme than that (25% + 6.25% + 6.25%). The *p-value* in this case is .25 + .25 + .0625 + .0625 = .625. There is a 62.5% chance of observing data as extreme as you saw, or more extreme, under the assumption that your null hypothesis is true. 

To determine whether our result is [*statistically significant*](https://whatpmeans.github.io/statistical-significance.html), we must decide whether this *p-value* is low enough that we can reject the null hypothesis. If we select an alpha (cutoff value for *p*) of .05, then we would *fail* to reject the null hypothesis, since there is more than a 5% chance of observing data at least as extreme as we saw if the null hypothesis is true (p > .05). This does not mean that we accept the null as true, but rather than we do not have evidence to show that the null is *not* true.

If we did happen to reject the null - perhaps we chose an alpha of .7 (which would not be a standard choice), then we would reject the null hypothesis, since there is less than a 70% chacen of observing data at least as extreme as we saw if the null hypothesis is true (p < .7). In this case we would conclude that some part of the null hypothesis is false. Either the expected result is not truly .5, or the coin flips are not independent, or the binomial distribution is the wrong one to use, or some combination of those.

We could then calculate the [*confidence interval*](https://whatpmeans.github.io/confidence-interval.html) for our proportion. If we decide that we want a 90% confidence interval, then ..... XXX
