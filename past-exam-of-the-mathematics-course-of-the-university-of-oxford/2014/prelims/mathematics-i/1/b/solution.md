<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose a [basis](../../../../../../basis.md) $u_1,\ldots,u_r$ of $U$, extend it to a [basis](../../../../../../basis.md) $u_1,\ldots,u_r,w_1,\ldots,w_s$ of $W$, and extend again to a [basis](../../../../../../basis.md) of $V$ by adding $v_1,\ldots,v_t$. Define

$$
\boxed{W'=\operatorname{span}\{u_1,\ldots,u_r,v_1,\ldots,v_t\}.}
$$

Every member of the full [basis](../../../../../../basis.md) lies in $W$ or $W'$, so the [sum of vector subspaces](../../../../../../sum-of-vector-subspaces.md) is $W+W'=V$. If $x\in W\cap W'$, express it in both displayed [bases](../../../../../../basis.md). Uniqueness of the coordinates in the full [basis](../../../../../../basis.md) forces its $w_j$ and $v_j$ coefficients to vanish. Thus $x\in U$. The reverse inclusion is built into the construction, proving $W\cap W'=U$. This is a [subspace supplement with a prescribed intersection](../../../../../../subspace-supplement-with-a-prescribed-intersection.md).

For the matrix example, let

$$
J=\begin{pmatrix}0&1\\-1&0\end{pmatrix},\qquad
I=\begin{pmatrix}1&0\\0&1\end{pmatrix}.
$$

The [skew-symmetric matrices](../../../../../../skew-symmetric-matrix.md) are exactly $U=\operatorname{span}\{J\}$, and the traceless [matrices](../../../../../../matrix.md) form $W$. A suitable answer is

$$
\boxed{W'=\operatorname{span}\{I,J\}
=\left\{\begin{pmatrix}a&b\\-b&a\end{pmatrix}:a,b\in\mathbb R\right\}.}
$$

The [matrix trace](../../../../../../matrix-trace.md) of $aI+bJ$ is $2a$, so $W\cap W'=\operatorname{span}\{J\}=U$. Every $2\times2$ real [matrix](../../../../../../matrix.md) has the decomposition

$$
A=\left(A-\frac{\operatorname{tr}A}{2}I\right)+\frac{\operatorname{tr}A}{2}I,
$$

whose first term lies in $W$ and second in $W'$. Therefore $W+W'=M_2(\mathbb R)$, as required.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Mathematics I](../../../mathematics-i-split.md)
4. [Prelims](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
