<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The Gaussian maximum-likelihood covariance estimate is

$$
\boxed{\widehat\Sigma=\frac1n\sum_{i=1}^n
(x_i-\overline x)(x_i-\overline x)^T.}
$$

For each $i,k$,

$$
|(AB)_{ik}|
\leq\sum_j|A_{ij}||B_{jk}|
\leq\|A\|_\infty\sum_j|B_{jk}|
\leq\|A\|_\infty\|B\|_{L^1},
$$

so $\|AB\|_\infty\leq\|A\|_\infty\|B\|_{L^1}$. If $A$ is square and symmetric, its maximum row sum equals its maximum column sum, and the same calculation gives

$$
\|AB\|_\infty\leq\|A\|_{L^1}\|B\|_\infty.
$$

Both the objective $\|\Omega\|_1=\sum_j\|\Omega_j\|_1$ and the constraints separate by columns. Replacing one column of a global minimizer by a better feasible column would improve the global objective. Therefore each $\widehat\Omega_j$ minimizes

$$
\|\beta\|_1
\quad\text{subject to}\quad
\|\widehat\Sigma\beta-e_j\|_\infty\leq\lambda.
$$

Moreover,

$$
\|\widehat\Sigma\Omega^0_j-e_j\|_\infty
=\|(\widehat\Sigma-\Sigma^0)\Omega^0_j\|_\infty
\leq\|\widehat\Sigma-\Sigma^0\|_\infty
\|\Omega^0_j\|_1\leq\lambda.
$$

Thus $\Omega^0_j$ is feasible and

$$
\|\widehat\Omega_j\|_1\leq\|\Omega^0_j\|_1.
$$

For every column,

$$
\begin{aligned}
\|\Sigma^0(\widehat\Omega_j-\Omega^0_j)\|_\infty
&\leq\|(\Sigma^0-\widehat\Sigma)\widehat\Omega_j\|_\infty
 +\|\widehat\Sigma\widehat\Omega_j-e_j\|_\infty\\
&\leq\lambda+\lambda=2\lambda.
\end{aligned}
$$

Finally $\widehat\Omega-\Omega^0=\Omega^0\Sigma^0(\widehat\Omega-\Omega^0)$, and symmetry of $\Omega^0$ gives

$$
\boxed{\|\widehat\Omega-\Omega^0\|_\infty
\leq2\lambda\|\Omega^0\|_{L^1}.}
$$

This is the basic error bound for the [CLIME precision-matrix estimator](../../../../../clime-precision-matrix-estimator.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
