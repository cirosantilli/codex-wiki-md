<h1 id="30j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The exponential loss is $\phi(z)=e^{-z}$. For a score $f:\mathcal X\to\mathbb R$, its [exponential classification risk](../../../../../../exponential-classification-risk.md) and empirical risk are

$$
R_\phi(f)=\mathbb E[e^{-Yf(X)}],
\qquad
\widehat R_\phi(f)=\frac1n\sum_{i=1}^ne^{-Y_if(X_i)}.
$$

For the set of evaluation vectors

$$
B(x_{1:n})
=\{(h(x_1),\ldots,h(x_n)):h\in B\},
$$

its empirical [Rademacher complexity](../../../../../../rademacher-complexity.md) is

$$
\boxed{
\widehat R(B(x_{1:n}))
=\frac1n\mathbb E_\sigma
\sup_{h\in B}\sum_{i=1}^n\sigma_ih(x_i)},
$$

where the $\sigma_i$ are independent uniform random signs.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [30J](../../30j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
