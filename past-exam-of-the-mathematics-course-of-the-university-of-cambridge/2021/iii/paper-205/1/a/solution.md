<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write

$$
L(\beta)=\frac1n\sum_{i=1}^n\left[-y_ix_i^T\beta+\log(1+e^{y_ix_i^T\beta})\right].
$$

Its score is

$$
\nabla_jL(\beta)=-\frac1n\sum_{i=1}^n\frac{y_ix_{ij}}{1+e^{y_ix_i^T\beta}}.
$$

The [Karush-Kuhn-Tucker conditions](../../../../../../karush-kuhn-tucker-conditions.md) for [L1-penalized logistic regression](../../../../../../l1-penalized-logistic-regression.md) are therefore

$$
-\frac1n\sum_{i=1}^n\frac{y_ix_{ij}}{1+e^{y_ix_i^T\widehat\beta}}+\lambda z_j=0,
\qquad
z_j\in\begin{cases}
\{\operatorname{sgn}(\widehat\beta_j)\},&\widehat\beta_j\ne0,\\
[-1,1],&\widehat\beta_j=0.
\end{cases}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
