<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For centered square-integrable variables with positive [variances](../../../../../variance-split.md), the [correlation coefficient](../../../../../pearson-correlation-coefficient.md) is

$$
\rho(X,X')=\frac{\mathbb E[XX']}{\sqrt{\mathbb E[X^2]\mathbb E[(X')^2]}}.
$$

Put $v=\sqrt{\mathbb E[X^2]}$ and $v'=\sqrt{\mathbb E[(X')^2]}$. Then

$$
\mathbb E\left[\left(\frac Xv-\frac{X'}{v'}\right)^2\right]=2(1-\rho).
$$

Thus **$\boxed{\rho=1\iff X=(v/v')X'\text{ almost surely}}$**, with positive proportionality factor. Conversely positive proportionality immediately gives correlation one. For variables with nonzero means, this criterion applies to their centered versions and yields an affine, not necessarily proportional, relationship. That distinction is essential for the positive stock prices below.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
