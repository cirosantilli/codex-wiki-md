<h1 id="40c/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The displayed matrix is an [upper bidiagonal matrix](../../../../../../upper-bidiagonal-matrix.md). For $\lambda_1=1$, the [right eigenvector](../../../../../../right-eigenvector.md) equation $(A-I)v=0$ successively gives

$$
v_2=v_3=\cdots=v_n=0.
$$

We may therefore take the unit right eigenvector to be $v=e_1$.

For a [left eigenvector](../../../../../../left-eigenvector.md), $(A^T-I)u=0$ gives

$$
u_{i-1}+(\lambda_i-1)u_i=0
\qquad(2\leq i\leq n).
$$

Since $\lambda_i-1=-1/i$,

$$
u_i=i\,u_{i-1}.
$$

Choosing the initial scale $u_1=1$ produces

$$
u=(1,2!,3!,\ldots,n!)^T.
$$

After normalization,

$$
\widehat u=
\frac{(1,2!,3!,\ldots,n!)^T}
{\sqrt{1+(2!)^2+\cdots+(n!)^2}}.
$$

The [eigenvalue sensitivity](../../../../../../eigenvalue-sensitivity.md) is therefore

$$
s(1)=\frac1{|\widehat u^Tv|}
=\sqrt{1+(2!)^2+\cdots+(n!)^2}
\geq n!,
$$

where $n!$ is the [factorial](../../../../../../factorial.md). Hence

$$
\boxed{s(\lambda_1)\geq n!}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [40C](../../40c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
