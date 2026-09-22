<h1 id="10c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the $A$ [basis](../../../../../../basis.md), the transformations whose columns are the new [basis](../../../../../../basis.md) [vectors](../../../../../../vector.md) are

$$
U_B=\begin{pmatrix}1/2&\sqrt3/2\\\sqrt3/2&-1/2\end{pmatrix},
\qquad
U_C=\begin{pmatrix}1/2&\sqrt3/2\\-\sqrt3/2&1/2\end{pmatrix}.
$$

Thus $U_C$ is a rotation through $-\pi/3$, while $U_B$ is a real orthogonal reflection, equivalently a rotation with one basis-vector phase reversed.

For any real orthogonal [matrix](../../../../../../matrix.md) $U$ with columns $|u_j\rangle$,

$$
\sum_j|u_ju_j\rangle
=\sum_{j,k,l}U_{kj}U_{lj}|a_ka_l\rangle
=\sum_{k,l}(UU^T)_{kl}|a_ka_l\rangle
=\sum_k|a_ka_k\rangle.
$$

Applying this to $U_B$ and $U_C$ and normalizing proves

$$
\boxed{
\frac{|a_0a_0\rangle+|a_1a_1\rangle}{\sqrt2}
=\frac{|b_0b_0\rangle+|b_1b_1\rangle}{\sqrt2}
=\frac{|c_0c_0\rangle+|c_1c_1\rangle}{\sqrt2}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10C](../../10c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
