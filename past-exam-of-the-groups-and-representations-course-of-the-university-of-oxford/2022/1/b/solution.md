<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In a [one-dimensional representation](../../../../one-dimensional-representation.md), the scalar images of $Q$ and $P$ commute. The relation $PQP=Q^{-1}$ gives $R(Q)^2=1$, while $R(Q)^5=1$, so $R(Q)=1$ and $R(P)=\pm1$. These give exactly $R_0$ and $R_1$.

For $k=1,2$, define the two-dimensional [representations](../../../../group-representation.md)

$$
D_k(Q)=\operatorname{diag}(\alpha^k,\alpha^{-k}),\qquad
D_k(P)=\begin{pmatrix}0&1\\1&0\end{pmatrix}.
$$

The same [invariant subspace](../../../../invariant-subspace.md) argument as in [solution](../a/solution.md) proves that each is [irreducible](../../../../irreducible-representation.md). Set $R_2=D_1$ and $R_3=D_2$. Their [characters](../../../../character-of-a-representation.md) differ at $Q$, so they are inequivalent. The [sum of squares of irreducible representation dimensions](../../../../sum-of-squares-of-irreducible-representation-dimensions.md) is already $1^2+1^2+2^2+2^2=10$, proving completeness.

Put $s=2\cos(2\pi/5)=(\sqrt5-1)/2$ and $t=2\cos(4\pi/5)=-(\sqrt5+1)/2$. Taking [traces](../../../../matrix-trace.md) yields the [character table](../../../../character-table.md)

$$
\boxed{\begin{array}{c|rrrr}
 & I & Q,Q^4 & Q^2,Q^3 & Q^kP\\\hline
\text{class size}&1&2&2&5\\\hline
R_0&1&1&1&1\\
R_1&1&1&1&-1\\
R_2&2&s&t&0\\
R_3&2&t&s&0
\end{array}}
$$

The identities $s+t=-1$, $st=-1$, and $s^2+t^2=3$ also verify [character orthogonality](../../../../character-orthogonality.md) directly.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (2)

- [Solution](../c/solution.md)
- [Solution](../d/i/solution.md)
