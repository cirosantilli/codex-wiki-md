<h1 id="20h/solution">Solution</h1>

↑ **Parent:** [20H](../20h.md)

Cover the circle by two open arcs whose intersection has two components, and take their products with $X$. Both members of this cover retract onto $X$, while their intersection retracts onto $X\sqcup X$. The [Mayer–Vietoris sequence](../../../../../mayer-vietoris-sequence.md) has the map

$$
H_j(X)\oplus H_j(X)\longrightarrow H_j(X)\oplus H_j(X),\qquad
(a,b)\longmapsto(a+b,-a-b),
$$

after consistent identifications of the two overlap components. Its kernel and cokernel are each $H_j(X)$. Exactness therefore supplies

$$
0\longrightarrow H_j(X)\longrightarrow H_j(S^1\times X)
\longrightarrow H_{j-1}(X)\longrightarrow0.
$$

This splits because the last [group](../../../../../group-split.md) is free abelian: lift a basis and extend linearly. With $H_{-1}=0$, the result is

$$
\boxed{H_j(S^1\times X)\cong H_j(X)\oplus H_{j-1}(X).}
$$

Starting from a point and iterating this decomposition, Pascal's identity yields

$$
\boxed{H_j(T^n;\mathbb Z)\cong\mathbb Z^{\binom nj}\quad(0\le j\le n),\qquad
H_j(T^n)=0\quad(j>n).}
$$

## ↑ Ancestors (10)

1. [20H](../20h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
