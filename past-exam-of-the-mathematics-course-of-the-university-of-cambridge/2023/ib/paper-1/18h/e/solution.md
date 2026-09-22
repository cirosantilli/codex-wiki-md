<h1 id="18h/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [Rao-Blackwell theorem](../../../../../../rao-blackwell-theorem.md) suggests conditioning $S$ on $T$. Part (d) gives

$$
\widetilde S
=\mathbb E[X_1^2-1\mid T]
=\frac12+\frac{T^2}{4}-1
=\frac{T^2}{4}-\frac12.
$$

It remains unbiased. Since $T\sim N(2\mu,2)$ and a normal variable with mean $m$ and variance $v$ satisfies $\operatorname{var}(T^2)=2v^2+4m^2v$,

$$
\operatorname{MSE}(\widetilde S)
=\frac1{16}\operatorname{var}(T^2)
=\frac1{16}(8+32\mu^2)
=\boxed{\frac12+2\mu^2}.
$$

This is strictly below $2+4\mu^2$ for every $\mu$. The calculation is recorded as the [Rao-Blackwell estimator of a squared normal mean](../../../../../../rao-blackwell-estimator-of-a-squared-normal-mean.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [18H](../../18h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
