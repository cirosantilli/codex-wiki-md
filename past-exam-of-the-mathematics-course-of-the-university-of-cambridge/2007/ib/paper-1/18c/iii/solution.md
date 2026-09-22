<h1 id="18c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The uniform prior and [likelihood](../../../../../../likelihood-function.md) give the posterior density

$$
\pi(\theta\mid K)=\frac{(n+1)!}{K!(n-K)!}\theta^K(1-\theta)^{n-K},
$$

a [Beta distribution](../../../../../../beta-distribution.md) with parameters $K+1,n-K+1$. Under [squared-error loss](../../../../../../squared-error-loss.md) for $\phi$, the posterior expected loss is $\mathbb E[\phi^2\mid K]-2a\mathbb E[\phi\mid K]+a^2$, minimized uniquely at the posterior mean of $\phi$, not at the product of the two posterior mean factors.

Using the supplied beta integral,

$$
\mathbb E[\theta(1-\theta)\mid K]
=\frac{(K+1)!(n-K+1)!/(n+3)!}{K!(n-K)!/(n+1)!}.
$$

Thus **the Bayes estimate is**

$$
\boxed{\widehat\phi_B=\frac{(K+1)(n-K+1)}{(n+2)(n+3)}.}
$$

This remains positive even on the endpoint samples, unlike the extended MLE; it integrates over the posterior uncertainty in $\theta$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [18C](../../18c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
