<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a Cartesian change of components $x_i'=R_{ij}x_j$, a rank-$n$ [tensor](../../../../../tensor.md) transforms according to

$$
\boxed{T'_{i_1\cdots i_n}=R_{i_1j_1}\cdots R_{i_nj_n}T_{j_1\cdots j_n},}
$$

with repeated indices summed. An [isotropic tensor](../../../../../isotropic-tensor.md) has unchanged components under every proper [rotation matrix](../../../../../rotation-matrix.md).

For rank two write $T'=RTR^T$. Invariance under quarter-turns implies invariance under their squares, the coordinate half-turns

$$
R_x(\pi)=\operatorname{diag}(1,-1,-1),\qquad R_y(\pi)=\operatorname{diag}(-1,1,-1).
$$

Each off-diagonal entry changes sign under at least one of these, so all off-diagonal entries vanish. A quarter-turn about the third axis then interchanges the first two diagonal entries, making them equal; a quarter-turn about the first axis equates the other two. Therefore

$$
\boxed{T_{ij}=\lambda\delta_{ij}.}
$$

Conversely $R(\lambda I)R^T=\lambda I$ for every rotation. This proves the [isotropic second-rank tensor](../../../../../isotropic-second-rank-tensor.md) classification without assuming that the original [tensor](../../../../../tensor.md) was symmetric. Also $\lambda=T_{kk}/3$ is a [scalar](../../../../../scalar.md), since the [trace](../../../../../matrix-trace.md) is rotation-invariant.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
