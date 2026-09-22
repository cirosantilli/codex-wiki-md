<h1 id="5b/solution">Solution</h1>

↑ **Parent:** [5B](../5b.md)

Let $a_1,a_2,a_3$ denote the columns. The [Gram-Schmidt process](../../../../../gram-schmidt-process.md) begins with $\|a_1\|=2$, so

$$
q_1=\frac12(1,1,1,1)^{\mathsf T},\qquad r_{11}=2.
$$

The second column has $r_{12}=q_1^{\mathsf T}a_2=4$ and residual

$$
a_2-4q_1=(-1,1,-1,1)^{\mathsf T}.
$$

This residual has norm $2$, giving $q_2=\tfrac12(-1,1,-1,1)^{\mathsf T}$ and $r_{22}=2$.

For the third column the [orthogonal projections](../../../../../orthogonal-projection.md) are $r_{13}=6$ and $r_{23}=4$. Subtracting them gives

$$
a_3-6q_1-4q_2=(1,1,-1,-1)^{\mathsf T}.
$$

Its norm is $2$, so $q_3=\tfrac12(1,1,-1,-1)^{\mathsf T}$ and $r_{33}=2$. Thus the requested thin [QR decomposition](../../../../../qr-decomposition.md) is

$$
\boxed{Q=\frac12\begin{pmatrix}1&-1&1\\1&1&1\\1&-1&-1\\1&1&-1\end{pmatrix},\qquad R=\begin{pmatrix}2&4&6\\0&2&4\\0&0&2\end{pmatrix}}.
$$

The three displayed columns have pairwise zero [inner products](../../../../../inner-product.md) and unit norms; direct multiplication gives $QR=A$.

## ↑ Ancestors (10)

1. [5B](../5b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
