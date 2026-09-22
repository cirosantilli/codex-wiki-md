<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The two diagonal generators are independent involutions, so

$$
H_1=\{\operatorname{diag}(\epsilon_1,\epsilon_2):\epsilon_1,\epsilon_2\in\{1,-1\}\},\qquad |H_1|=4.
$$

It is a [Klein four-group](../../../../../klein-four-group.md). Write the swapping generator as $J=\begin{pmatrix}0&1\\1&0\end{pmatrix}$. Then $J^2=I$, so $H_2=\{I,J\}$ has order two. Moreover,

$$
J\operatorname{diag}(\epsilon_1,\epsilon_2)J
=\operatorname{diag}(\epsilon_2,\epsilon_1)\in H_1.
$$

Thus $J$ normalizes $H_1$. The set

$$
K=\{DJ^\eta:D\in H_1,\ \eta\in\{0,1\}\}
$$

is a [group](../../../../../group-split.md): its products reduce using

$$
(DJ^\eta)(D'J^\zeta)=D(J^\eta D'J^{-\eta})J^{\eta+\zeta},
$$

and inverses reduce in the same way. It contains both generating [subgroups](../../../../../subgroup.md), so minimality gives $G\subseteq K$; conversely every displayed product is in $G$, giving $G=K$.

There are four diagonal [matrices](../../../../../matrix.md) $D$ and four off-diagonal [matrices](../../../../../matrix.md) $DJ$, all distinct. Consequently

$$
\boxed{|G|=8}.
$$

Also $H_1\cap H_2=\{I\}$, since $J$ is not diagonal, and every element of $G$ has the form $DJ^\eta\in H_1H_2$. This proves condition (I), hence the [exact factorization of a group](../../../../../exact-factorization-of-a-group.md). Here $H_1$ is a [normal subgroup](../../../../../normal-subgroup.md) and $G=H_1\rtimes H_2$ is a [semidirect product](../../../../../semidirect-product.md). Its [matrices](../../../../../matrix.md) are the two-dimensional [signed permutation matrices](../../../../../signed-permutation-matrix.md), also realizing the [dihedral group](../../../../../dihedral-group.md) of the square.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [9](../../9.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
