<h1 id="8c/solution">Solution</h1>

↑ **Parent:** [8C](../8c.md)

The successive differences of the constant entries give a simple [LDL decomposition](../../../../../ldl-decomposition.md):

$$
\boxed{L=\begin{pmatrix}1&0&0&0\\1&1&0&0\\1&1&1&0\\1&1&1&1\end{pmatrix},\qquad
D=\operatorname{diag}(1,4,9,\lambda-14),\qquad A=LDL^T}.
$$

For example, entry $(i,j)$ of $LDL^T$ is the sum of the first $\min(i,j)$ entries of $D$, directly verifying every entry of $A$. Because $L$ is an [invertible matrix](../../../../../invertible-matrix.md), $x^TAx=(L^Tx)^TD(L^Tx)$ is strictly positive for every nonzero [vector](../../../../../vector.md) exactly when every diagonal entry of $D$ is positive. Consequently

$$
\boxed{A\text{ is positive definite}\iff\lambda>14}.
$$

At $\lambda=14$ it is a [positive semidefinite matrix](../../../../../positive-semidefinite-matrix.md) and singular; for $\lambda<14$ its [quadratic form](../../../../../quadratic-form.md) takes both positive and negative values.

When $\lambda=30$, taking positive square roots of $D$ yields the [Cholesky decomposition](../../../../../cholesky-decomposition.md)

$$
\boxed{A=CC^T,\qquad C=L\operatorname{diag}(1,2,3,4)=\begin{pmatrix}1&0&0&0\\1&2&0&0\\1&2&3&0\\1&2&3&4\end{pmatrix}}.
$$

## ↑ Ancestors (10)

1. [8C](../8c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
