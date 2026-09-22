<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $f=\widetilde f/Z_f$ and $g=\widetilde g/Z_g$. If the constants needed to evaluate $f/g$ are unavailable, use the [self-normalized importance sampling](../../../../../../../self-normalized-importance-sampling.md) [estimator](../../../../../../../estimator.md)

$$
\boxed{\widehat\mu_{\mathrm{SN}}=\frac{\sum_i\widetilde w_i\theta(X_i)}{\sum_i\widetilde w_i},\qquad\widetilde w_i=\frac{\widetilde f(X_i)}{\widetilde g(X_i)}.}
$$

The unknown common factor $Z_g/Z_f$ cancels. Under full target [probability support](../../../../../../../support-of-a-probability-distribution.md) and integrability, the numerator and denominator sample means converge to $\int\widetilde f\theta/Z_g$ and $\int\widetilde f/Z_g$, respectively, whose ratio is $\mu$. The same construction applies if only one normalization is unknown by taking the other [probability density function](../../../../../../../probability-density-function.md) already normalized. Sampling from $g$ itself is assumed available, even when its normalization is not explicitly known.

This ratio [estimator](../../../../../../../estimator.md) is generally biased at finite $n$, unlike the ordinary normalized-weight [estimator](../../../../../../../estimator.md). Also, its [variance](../../../../../../../variance-split.md) is not the formula in the next part: that formula concerns the ordinary unbiased [estimator](../../../../../../../estimator.md). Full [probability support](../../../../../../../support-of-a-probability-distribution.md) for $f$ is needed here because the denominator estimates the entire target normalizing [integral](../../../../../../../integral.md), not just the [probability support](../../../../../../../support-of-a-probability-distribution.md) of $f\theta$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 40](../../../../paper-40-split.md)
5. [Iii](../../../../split.md)
6. [2002](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
