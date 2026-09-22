<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an [invertible matrix](../../../../invertible-matrix.md) $P$ whose columns give the new [basis](../../../../basis.md) in old coordinates, the new [matrix](../../../../matrix.md) is $B=P^{-1}AP$. Multiplicativity of the [determinant](../../../../determinant.md) gives

$$
\det B=\det(P^{-1})\det A\det P=\det A,
$$

since $\det(P^{-1})\det P=1$.

To justify the [cyclic property of the trace](../../../../cyclic-property-of-the-trace.md) directly, for two [square matrices](../../../../square-matrix.md) $R,S$,

$$
\operatorname{tr}(RS)=\sum_{i,j}R_{ij}S_{ji}
=\sum_{j,i}S_{ji}R_{ij}=\operatorname{tr}(SR).
$$

Apply it with $R=P^{-1}A$ and $S=P$:

$$
\boxed{\det(P^{-1}AP)=\det A,\qquad
\operatorname{tr}(P^{-1}AP)=\operatorname{tr}(PP^{-1}A)=\operatorname{tr}A.}
$$

Thus both the [determinant](../../../../determinant.md) and [trace](../../../../matrix-trace.md) are invariant under [change of basis](../../../../change-of-basis.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [2021 resit](../../../2021-resit-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
