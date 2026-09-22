<h1 id="12a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Cartesian second-rank tensor](../../../../../../cartesian-second-rank-tensor.md) transformation convention $T'=RTR^T$, where $R$ is the orthogonal matrix converting components to the new [orthonormal basis](../../../../../../orthonormal-basis.md). The coordinate half-turns are

$$
R_x=\operatorname{diag}(1,-1,-1),\quad
R_y=\operatorname{diag}(-1,1,-1),\quad
R_z=\operatorname{diag}(-1,-1,1).
$$

For a diagonal rotation $R=\operatorname{diag}(s_1,s_2,s_3)$, invariance gives $t_{ij}=s_is_jt_{ij}$, with no summation in this equation. For each $i\ne j$, one of the listed half-turns makes $s_is_j=-1$, so $t_{ij}=-t_{ij}=0$. Thus

$$
\boxed{T=\operatorname{diag}(t_{11},t_{22},t_{33}).}
$$

This is [coordinate half-turn invariance of a second-rank tensor](../../../../../../coordinate-half-turn-invariance-of-a-second-rank-tensor.md). It does not force equal diagonal entries; invariance under all rotations would be the stronger [isotropic second-rank tensor](../../../../../../isotropic-second-rank-tensor.md) condition.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12A](../../12a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
