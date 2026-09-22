<h1 id="40e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Since $S\mathbf w=c\mathbf e^{(1)}$ and $A\mathbf w=\lambda_1\mathbf w$,

$$
\widehat A(c\mathbf e^{(1)})
=SAS^{-1}S\mathbf w
=SA\mathbf w
=\lambda_1c\mathbf e^{(1)}.
$$

Thus the first column of $\widehat A$ is $(\lambda_1,0,\ldots,0)^T$, and $\widehat A$ is a [block upper triangular matrix](../../../../../../block-upper-triangular-matrix.md):

$$
\widehat A=
\begin{pmatrix}
\lambda_1&*\\
0&B
\end{pmatrix},
$$

where $B$ is its bottom-right $(n-1)\times(n-1)$ submatrix. Therefore

$$
\det(zI-\widehat A)=(z-\lambda_1)\det(zI-B).
$$

A [similarity transformation](../../../../../../similarity-transformation.md) preserves the [characteristic polynomial](../../../../../../characteristic-polynomial.md), so

$$
\boxed{\operatorname{spec}(A)=\{\lambda_1\}\mathbin\cup\operatorname{spec}(B),}
$$

with [algebraic multiplicities](../../../../../../algebraic-multiplicity.md) included.

To construct $S$, use a [Householder transformation](../../../../../../householder-transformation.md). With $\alpha=\|\mathbf w\|_2$, choose the sign of $\alpha$ to avoid cancellation and set

$$
\mathbf v=\mathbf w-\alpha\mathbf e^{(1)},
\qquad
S=I-2\frac{\mathbf v\mathbf v^T}{\mathbf v^T\mathbf v}.
$$

Then $S$ is an [orthogonal matrix](../../../../../../orthogonal-matrix.md) and maps $\mathbf w$ to $\alpha\mathbf e^{(1)}$ up to the chosen sign. If $\mathbf w$ already lies on the first coordinate axis, take a suitable diagonal sign matrix. This is the one-vector case of [orthogonal coordinate reduction of a subspace](../../../../../../orthogonal-coordinate-reduction-of-a-subspace.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [40E](../../40e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
