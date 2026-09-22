<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the plug-in [Neyman allocation](../../../../../../neyman-allocation.md), the estimated [Bernoulli distribution](../../../../../../bernoulli-distribution.md) variances are $6/25$ and $3/16$, so

$$
\widehat R^*=\sqrt{\frac{6/25}{3/16}}=\frac{4\sqrt2}{5},\qquad
\boxed{\mathbb P(\text{treatment }0)=\frac{\widehat R^*}{1+\widehat R^*}
=\frac{4\sqrt2}{5+4\sqrt2}.}
$$

This uses the target ratio directly as the allocation odds; a procedure that actively corrects previous allocation imbalances would need an additional rule.

For the [randomized play-the-winner rule](../../../../../../randomized-play-the-winner-rule.md) RPW$(1,1)$, return the drawn ball and add one ball of the same treatment after a success or of the opposite treatment after a failure. Treatment 0 has three successes and two failures, and treatment 1 has one success and three failures. The urn therefore has $1+3+3=7$ treatment-0 balls and $1+1+2=4$ treatment-1 balls. Hence

$$
\boxed{\mathbb P(\text{treatment }0)=\frac7{11}.}
$$

For [dynamic programming](../../../../../../dynamic-programming.md) with only the final patient left, there is no future value from learning. Independent uniform [prior distributions](../../../../../../prior-probability.md) and [Beta-binomial conjugacy](../../../../../../beta-binomial-conjugacy.md) give posteriors $p_0\mid\mathcal D\sim\operatorname{Beta}(4,3)$ and $p_1\mid\mathcal D\sim\operatorname{Beta}(2,4)$. Their [posterior predictive probabilities](../../../../../../posterior-predictive-probability.md) of success are $4/7$ and $2/6=1/3$. The optimal terminal action therefore gives

$$
\boxed{\mathbb P(\text{treatment }0)=1.}
$$

This is optimal for expected successes with no imposed lower bound on the [randomization](../../../../../../randomization.md) probabilities.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
