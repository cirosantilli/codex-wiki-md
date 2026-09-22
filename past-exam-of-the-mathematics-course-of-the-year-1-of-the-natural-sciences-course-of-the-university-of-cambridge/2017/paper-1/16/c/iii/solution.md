<h1 id="16/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The same [integration by substitution](../../../../../../integration-by-substitution.md) gives the [expected value](../../../../../../expected-value-split.md)

$$
\mathbb E[X]=\frac12\int_{-\infty}^{\infty}(\mu+2st)\operatorname{sech}^2t\,dt
=\mu+s\int_{-\infty}^{\infty}t\operatorname{sech}^2t\,dt.
$$

The remaining integrand is an [odd function](../../../../../../odd-function.md). Its [integral](../../../../../../integral-split.md) is absolutely convergent, since $\operatorname{sech}^2t\leq4e^{-2|t|}$ and $|t|e^{-2|t|}$ is integrable. Thus cancellation under [symmetry in integration](../../../../../../symmetry-in-integration.md) is legitimate, rather than merely a principal-value calculation. Consequently

$$
\boxed{\mathbb E[X]=\mu.}
$$

Equivalently, the [logistic distribution](../../../../../../logistic-distribution.md) is symmetric about $\mu$, and its exponentially decaying tails ensure that its [expected value](../../../../../../expected-value-split.md) exists.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [16](../../../16.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
