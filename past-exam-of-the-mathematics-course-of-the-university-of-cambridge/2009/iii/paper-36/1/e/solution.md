<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Before collecting any observations, a uniform success-chance [prior distribution](../../../../../../prior-probability.md) gives

$$
\Pr(Y=y)=\binom ny\int_0^1\theta^y(1-\theta)^{n-y}\,d\theta
=\binom ny\mathrm B(y+1,n-y+1)
=\boxed{\frac1{n+1}},\qquad y=0,\ldots,n.
$$

Thus the [uniform-count predictive property](../../../../../../uniform-count-predictive-property.md) assigns equal probability to every possible number of successes in a fixed-size batch under the [prior predictive distribution](../../../../../../bayesian-model-evidence.md). It is uniform over counts, not over all ordered binary sequences. After observing $x$ successes in $m$ trials, its familiar one-step [posterior predictive probability](../../../../../../posterior-predictive-probability.md) is $(x+1)/(m+2)$; the count-uniform property refers to prediction before those data are observed.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
