<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Partition $M$ into the same five-by-five blocks as $R$. The equation for block $(i,j)$ is $M_{ij}R_j(g)=R_i(g)M_{ij}$, so each block is an [intertwiner](../../../../intertwiner.md). By [Schur's lemma](../../../../schur-s-lemma.md), blocks between the two inequivalent [irreducible representations](../../../../irreducible-representation.md) vanish, whereas blocks between identical copies are arbitrary scalar multiples of the relevant identity [matrix](../../../../matrix.md). Thus the [commutant of a semisimple representation](../../../../commutant-of-a-semisimple-representation.md) is

$$
\boxed{
M=\begin{pmatrix}
a_{11}I_{n_1}&a_{12}I_{n_1}&a_{13}I_{n_1}&0&0\\
a_{21}I_{n_1}&a_{22}I_{n_1}&a_{23}I_{n_1}&0&0\\
a_{31}I_{n_1}&a_{32}I_{n_1}&a_{33}I_{n_1}&0&0\\
0&0&0&b_{11}I_{n_2}&b_{12}I_{n_2}\\
0&0&0&b_{21}I_{n_2}&b_{22}I_{n_2}
\end{pmatrix},\quad a_{ij},b_{ij}\in\mathbb C.}
$$

Equivalently, $M=(A\otimes I_{n_1})\oplus(B\otimes I_{n_2})$, where $A\in M_3(\mathbb C)$ and $B\in M_2(\mathbb C)$. Substitution proves every such [matrix](../../../../matrix.md) commutes with every $R(g)$. There is no invertibility requirement on $M$, and its solution space has complex dimension $3^2+2^2=13$, even if $n_1=n_2$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
