<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $P=(P_{ij})_{i,j=1}^3$, where $P_{ij}:\mathbb C^{m_j}\to\mathbb C^{m_i}$. Block multiplication makes the commuting condition equivalent to

$$
P_{ij}R_j(g)=R_i(g)P_{ij}\qquad(\forall g\in G).
$$

Thus every block is an [intertwiner](../../../../intertwiner.md). For $i\ne j$, the [irreducible representations](../../../../irreducible-representation.md) are inequivalent, so the [Schur lemma](../../../../schur-s-lemma.md) gives $P_{ij}=0$. On each diagonal block, the same [Schur lemma](../../../../schur-s-lemma.md) gives $P_{ii}=\lambda_iI_{m_i}$. Therefore

$$
\boxed{P=\begin{pmatrix}
\lambda_1I_{m_1}&0&0\\
0&\lambda_2I_{m_2}&0\\
0&0&\lambda_3I_{m_3}
\end{pmatrix},\qquad \lambda_1,\lambda_2,\lambda_3\in\mathbb C.}
$$

Conversely, every displayed [matrix](../../../../matrix.md) commutes with $R(g)$, proving both necessity and sufficiency. This [commutant of a semisimple representation](../../../../commutant-of-a-semisimple-representation.md) has complex [dimension](../../../../dimension-vector-space.md) three. The parameters may vanish: $P$ was not required to be invertible.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2020](../../../2020-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
