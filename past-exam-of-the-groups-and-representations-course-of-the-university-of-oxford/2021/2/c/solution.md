<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The two [invariant subspaces](../../../../invariant-subspace.md) are

$$
U_0=\mathbb C(1,1,1)^T,\qquad
U_2=\{(z_1,z_2,z_3)^T:z_1+z_2+z_3=0\}.
$$

Coordinate [permutations](../../../../permutation.md) preserve both equal coordinates and the coordinate sum. Their [dimensions](../../../../dimension-vector-space.md) add to three and their intersection is zero, so $\mathbb C^3=U_0\oplus U_2$. On $U_0$, the [basis](../../../../basis.md) $u_0=(1,1,1)^T$ gives $R_{U_0}(\tau)=(1)$ for every [transposition](../../../../transposition-permutation.md).

On $U_2$ choose the [basis](../../../../basis.md) $u=e_1-e_3$, $v=e_2-e_3$. Directly permuting their entries gives

$$
\begin{array}{c|cc}
\tau&R(\tau)u&R(\tau)v\\\hline
(12)&v&u\\
(13)&-u&v-u\\
(23)&u-v&-v
\end{array}
$$

Thus, taking images as columns, the [matrices](../../../../matrix.md) of the [matrix representation](../../../../matrix-representation.md) are

$$
\boxed{D(12)=\begin{pmatrix}0&1\\1&0\end{pmatrix},\quad
D(13)=\begin{pmatrix}-1&-1\\0&1\end{pmatrix},\quad
D(23)=\begin{pmatrix}1&0\\-1&-1\end{pmatrix}.}
$$

Each has [trace](../../../../matrix-trace.md) zero and squares to $I$. Their three-cycle products have [trace](../../../../matrix-trace.md) $-1$, so this is exactly the two-dimensional [irreducible representation](../../../../irreducible-representation.md) of [solution](../a/solution.md). These are all nonzero [invariant subspaces](../../../../invariant-subspace.md) affording individual [irreducible representations](../../../../irreducible-representation.md), since each occurs once in [solution](../b/solution.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../d/solution.md)
