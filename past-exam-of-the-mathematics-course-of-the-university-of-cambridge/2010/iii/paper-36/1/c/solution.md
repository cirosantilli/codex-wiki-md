<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Conditional on the success probability, the count has [binomial distribution](../../../../../../binomial-distribution.md). Integrating its [likelihood](../../../../../../likelihood-function.md) under the uniform [prior distribution](../../../../../../prior-probability.md), or equivalently a [Beta distribution](../../../../../../beta-distribution.md) with parameters $(1,1)$, gives

$$
p(y\mid H_1)=\int_0^1\binom ny\theta^y(1-\theta)^{n-y}\,d\theta
=\binom ny\frac{\Gamma(y+1)\Gamma(n-y+1)}{\Gamma(n+2)}
=\boxed{\frac1{n+1}},\qquad y=0,\ldots,n.
$$

The [prior predictive distribution](../../../../../../bayesian-model-evidence.md) is therefore uniform over the possible counts. Excluding the single point $\theta=1/2$ does not alter this integral because a continuous [prior distribution](../../../../../../prior-probability.md) gives that point zero probability. This calculation is the marginalization underlying [Beta-binomial conjugacy](../../../../../../beta-binomial-conjugacy.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
