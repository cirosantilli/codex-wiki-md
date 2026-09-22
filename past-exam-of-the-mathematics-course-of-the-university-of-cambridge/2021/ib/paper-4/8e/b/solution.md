<h1 id="8e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [symmetric matrix](../../../../../../symmetric-matrix.md) of the [quadratic form](../../../../../../quadratic-form.md) in the standard basis is

$$
A=\begin{pmatrix}
1&1&1\\
1&1&-1\\
1&-1&2
\end{pmatrix},
$$

because the off-diagonal entries contribute twice to $x^TAx$.

Apply [Gram-Schmidt orthogonalization for a symmetric bilinear form](../../../../../../gram-schmidt-orthogonalization-for-a-symmetric-bilinear-form.md) to

$$
u_1=e_1,
\qquad
u_2=e_3-e_1,
\qquad
u_3=e_2-e_1+2u_2=-3e_1+e_2+2e_3.
$$

These vectors are pairwise orthogonal for $B(u,v)=u^TAv$, and

$$
B(u_1,u_1)=1,
\qquad
B(u_2,u_2)=1,
\qquad
B(u_3,u_3)=-4.
$$

Thus the form is diagonal in the basis $(u_1,u_2,u_3)$, with matrix

$$
\operatorname{diag}(1,1,-4).
$$

It follows that its [rank](../../../../../../rank-of-a-quadratic-form.md) is $3$ and its [signature](../../../../../../signature-of-a-quadratic-form.md) is

$$
\boxed{2-1=1}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8E](../../8e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
