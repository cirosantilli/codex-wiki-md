<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The nonparametric [bootstrap](../../../../../../bootstrapping-statistics.md) replaces the unknown sampling law by the [empirical distribution](../../../../../../type-information-theory.md)

$$
\widehat F_n(x)=\frac1n\sum_{i=1}^n\mathbf1_{\{x_i\le x\}}.
$$

Generate $B$ independent [bootstrap samples](../../../../../../bootstrap-sample.md), each containing $n$ independent draws with replacement from that law. Recompute the original estimator in each sample, obtaining $\widehat\theta_1^*,\ldots,\widehat\theta_B^*$. With $\overline\theta^*=B^{-1}\sum_b\widehat\theta_b^*$, the [bootstrap standard error](../../../../../../bootstrap-standard-error.md) estimate is

$$
\boxed{\widehat{\operatorname{se}}_*(\widehat\theta)
=\left[\frac1{B-1}\sum_{b=1}^B(\widehat\theta_b^*-\overline\theta^*)^2\right]^{1/2}.}
$$

This estimates the conditional [bootstrap](../../../../../../bootstrapping-statistics.md) standard deviation, which approximates the estimator's sampling standard deviation when the [bootstrap](../../../../../../bootstrapping-statistics.md) is consistent. Dividing this expression by $\sqrt B$ would instead estimate the Monte Carlo error in the [bootstrap](../../../../../../bootstrapping-statistics.md) mean, a different quantity.

For distinct original observations, each resample is an ordered index sequence with one of $n^n$ equally likely values. It contains no repeats precisely when it is a permutation of all $n$ original indices, giving $n!$ possibilities. Hence

$$
\boxed{\mathbb P_*(\text{at least one repeated observation})=1-\frac{n!}{n^n}.}
$$

The distinctness assumption is needed to equate repeated values with repeated indices.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
