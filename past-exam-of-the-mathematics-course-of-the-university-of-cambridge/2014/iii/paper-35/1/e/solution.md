<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [posterior predictive probability](../../../../../../posterior-predictive-probability.md) averages the conditional probability over the [Bayesian posterior](../../../../../../bayesian-posterior.md). Using its [gamma distribution](../../../../../../gamma-distribution.md) density,

$$
p_0=\frac{B^A}{\Gamma(A)}\int_0^\infty\lambda^{A-1}e^{-(B+1)\lambda}\,d\lambda
=\boxed{\left(\frac{b+T}{b+T+1}\right)^{a+n}}.
$$

For fixed $a,b$ and $n/T\to\widehat\lambda<\infty$,

$$
\log p_0=-A\log(1+1/B)=-\frac{A}{B}+O(A/B^2)=-\frac nT+o(1).
$$

Consequently $p_0/e^{-n/T}\to1$, and both tend to $e^{-\widehat\lambda}$. This is reasonable because the [posterior mean](../../../../../../posterior-mean.md) tends to the observed rate and the [posterior variance](../../../../../../posterior-variance.md) tends to zero. Averaging $e^{-\lambda}$ then approaches evaluating it at the estimated rate: **with abundant observations, predictive uncertainty about the rate vanishes**.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
