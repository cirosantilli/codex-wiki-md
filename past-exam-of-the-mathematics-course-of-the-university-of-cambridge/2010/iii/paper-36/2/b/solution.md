<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Multiplying the [Poisson distribution](../../../../../../poisson-distribution.md) [likelihood](../../../../../../likelihood-function.md) by the [Jeffreys prior](../../../../../../jeffreys-prior.md) gives the [posterior density](../../../../../../posterior-density.md) kernel

$$
\pi(\lambda_i\mid y_i)\propto\lambda_i^{y_i-1/2}e^{-E_i\lambda_i}.
$$

Thus, in shape-rate convention,

$$
\boxed{\lambda_i\mid y_i\sim\operatorname{Gamma}(y_i+1/2,E_i).}
$$

It is a proper [posterior distribution](../../../../../../bayesian-posterior.md) even when $y_i=0$, provided $E_i>0$. The [posterior mean](../../../../../../posterior-mean.md) and [posterior variance](../../../../../../posterior-variance.md) are $(y_i+1/2)/E_i$ and $(y_i+1/2)/E_i^2$. This is [Poisson-gamma conjugacy with unequal exposures](../../../../../../poisson-gamma-conjugacy-with-unequal-exposures.md), with the zero-rate prior interpreted as an improper kernel.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
