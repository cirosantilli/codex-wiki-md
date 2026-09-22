<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Coordinate descent](../../../../../../coordinate-descent.md) cycles through the intercept and coefficient coordinates, minimizing the convex ridge objective in one coordinate while holding the others fixed. Given current coefficients, update

$$
\alpha\leftarrow\frac1n\sum_{i=1}^n
\left(Y_i-\sum_{k=1}^pX_{ik}\beta_k\right).
$$

For coordinate $j$, form the partial residual

$$
r^{(j)}=Y-\alpha\mathbf1-\sum_{k\ne j}X_k\beta_k
$$

and update it by the exact one-dimensional minimizer

$$
\beta_j\leftarrow
\frac{X_j^Tr^{(j)}}{X_j^TX_j+\lambda}.
$$

Repeated sweeps converge to the unique fitted value because the objective is a [convex function](../../../../../../convex-function.md); with $\lambda>0$ it is strictly convex in $\beta$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
