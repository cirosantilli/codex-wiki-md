<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The Markov factorization is

$$
p(\mathbf y\mid\mathbf t,\mu,\tau)
=\varphi(y_1;\mu,R)
\prod_{j=2}^3
\varphi\!\left(y_j;\mu+\rho(y_{j-1}-\mu),R(1-\rho^2)\right).
$$

Differentiating its log-likelihood with respect to $\mu$ gives

$$
\widehat\mu
=\frac{y_1+(1-\rho)y_2+y_3}{3-\rho}.
$$

Its coefficients sum to one, so it is unbiased. Direct covariance calculation, equivalently inversion of its [Fisher information](../../../../../../fisher-information-matrix.md), gives

$$
\operatorname{Var}(\widehat\mu)
=R\frac{1+\rho}{3-\rho}.
$$

**Thus the variance tends to $R$ as $\Delta t/\tau\to0$, because the observations become perfectly correlated, and to $R/3$ as $\Delta t/\tau\to\infty$, because they become three independent draws.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
