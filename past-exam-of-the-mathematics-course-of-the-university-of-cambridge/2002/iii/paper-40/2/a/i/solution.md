<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume independent samples $X_i\sim g$, $\int f|\theta|<\infty$, and $g>0$ wherever $f\theta$ can contribute. The [importance weight](../../../../../../../importance-weight.md) is $w(x)=f(x)/g(x)$, and the ordinary [importance sampling](../../../../../../../importance-sampling.md) [estimator](../../../../../../../estimator.md) is

$$
\boxed{\widehat\mu_g=\frac1n\sum_{i=1}^n\theta(X_i)\frac{f(X_i)}{g(X_i)}.}
$$

Its [expectation](../../../../../../../expected-value.md) is $\int \theta(x)f(x)\,dx=\mu$, by cancellation of $g$ in the [expectation](../../../../../../../expected-value.md) [integral](../../../../../../../integral.md). The [strong law of large numbers](../../../../../../../strong-law-of-large-numbers.md) gives almost-sure convergence to $\mu$. Common [probability support](../../../../../../../support-of-a-probability-distribution.md) is sufficient; the precise [support condition for importance sampling](../../../../../../../support-condition-for-importance-sampling.md) only requires covering the nonzero integrand for this particular [expectation](../../../../../../../expected-value.md).

## ↑ Ancestors (12)

1. [I](../i.md)
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
