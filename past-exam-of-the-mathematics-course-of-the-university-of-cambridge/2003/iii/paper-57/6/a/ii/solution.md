<h1 id="6/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

On the three-dimensional vector space of real symmetric matrices, write

$$
X=\begin{pmatrix}t+x&y\\y&t-x\end{pmatrix},\qquad -\det X=x^2+y^2-t^2.
$$

The [special linear group](../../../../../../../special-linear-group.md) acts by $X\mapsto AXA^T$, preserving this [quadratic form](../../../../../../../quadratic-form.md) when $\det A=1$. A kernel element satisfies $AA^T=I$ and commutes with every symmetric matrix, so it is scalar and equals $\pm I$. Its derivative is injective: if $aX+Xa^T=0$ for every symmetric $X$, taking $X=I$ makes $a$ skew-symmetric, and commuting with diagonal matrices then makes $a=0$.

Both real [Lie group](../../../../../../../lie-group.md) dimensions are three. The derivative is consequently an isomorphism, so the image is an open subgroup. The source $SL(2,\mathbb R)$ is connected: polar decomposition deforms it onto $SO(2)$, with the positive symmetric determinant-one factor contractible. Its image is thus the full identity component $SO_0(2,1)$, since a connected group has no proper open subgroup. This is the [symmetric-matrix double cover of SO0(2,1)](../../../../../../../symmetric-matrix-double-cover-of-so0-2-1.md).

For $J=\left(\begin{smallmatrix}0&1\\-1&0\end{smallmatrix}\right)$, direct multiplication gives $A^TJA=(\det A)J$. Hence preserving the two-dimensional [symplectic form](../../../../../../../symplectic-form.md) is exactly the determinant-one condition, so

$$
\boxed{SO_0(2,1)\cong SL(2,\mathbb R)/\{\pm I\}\cong Sp(2,\mathbb R)/\{\pm I\}.}
$$

The subscript zero is necessary. The full $SO(2,1)$ also contains a component reversing time orientation, which cannot be the image of the connected source.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Paper 57](../../../../paper-57-split.md)
5. [Iii](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
