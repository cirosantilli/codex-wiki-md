<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For an [exponential distribution](../../../../../../exponential-distribution.md) of rate $\theta>0$, the [probability density function](../../../../../../probability-density-function.md) and [survivor function](../../../../../../survival-function.md) are $f(t)=\theta e^{-\theta t}$ and $F(t)=e^{-\theta t}$. Set

$$
D=\sum_i v_i,\qquad E=\sum_i x_i,
$$

where $D$ is the observed event count and $E$ is total [person-time at risk](../../../../../../person-time-at-risk.md). The [log-likelihood](../../../../../../log-likelihood.md), up to a constant, becomes

$$
\ell(\theta)=D\log\theta-\theta E.
$$

When $D>0$ and $E>0$, its [score function](../../../../../../informant-function.md) is $D/\theta-E$, which vanishes at

$$
\boxed{\widehat\theta=\frac{D}{E}.}
$$

Its second derivative is negative, so this is the unique [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md). This is [exponential-rate estimation from censored exposure](../../../../../../exponential-rate-estimation-from-censored-exposure.md): the estimate is observed events divided by all observed exposure, including exposure from [right-censored](../../../../../../right-censoring.md) individuals.

If $D=0$ and $E>0$, $\ell=-\theta E$ decreases strictly. There is no maximizer in the open parameter space $\theta>0$; its supremum occurs as $\theta\downarrow0$, or the extended boundary estimate is $\widehat\theta=0$ if a zero rate is permitted. The formula should not be interpreted as an interior regular fit in this case.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
