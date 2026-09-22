<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [empirical distribution](../../../../../../type-information-theory.md) gives each observed value mass $1/n$, so its [empirical distribution function](../../../../../../empirical-distribution-function.md) is

$$
\widehat F_n(x)=\frac1n\sum_{i=1}^n\mathbf1_{\{x_i\le x\}}.
$$

For each of $B$ independent replications, draw $n$ values with replacement from this [empirical distribution](../../../../../../type-information-theory.md), recompute the same [estimator](../../../../../../estimator.md) $\widehat\theta^{*(b)}$, and use their sample [standard deviation](../../../../../../standard-deviation.md):

$$
\boxed{\widehat{\operatorname{se}}_{\rm boot}=\left[\frac1{B-1}\sum_{b=1}^B(\widehat\theta^{*(b)}-\overline\theta^*)^2\right]^{1/2}.}
$$

This estimates the conditional [bootstrap standard error](../../../../../../bootstrap-standard-error.md); dividing it by $\sqrt B$ would instead estimate simulation uncertainty in the bootstrap mean and is not the requested sampling [standard error](../../../../../../standard-error.md).

When the original observations are distinct, the first resampled index may be arbitrary. After $j$ distinct indices have been drawn, the next index avoids them with [probability](../../../../../../probability.md) $1-j/n$. Multiplying conditional [probabilities](../../../../../../probability.md) gives

$$
P_*(\text{all distinct})=\prod_{j=0}^{n-1}\left(1-\frac jn\right)=\frac{n!}{n^n},\qquad
\boxed{P_*(\text{at least one repeat})=1-\prod_{j=0}^{n-1}\left(1-\frac jn\right).}
$$

Here $P_*$ denotes [probability](../../../../../../probability.md) conditional on the data.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
