<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Writing $Q_j$ for the $j$th marginal and using $P=\prod_jP_j$,

$$
D(Q\Vert P)=-H(Q)+\sum_j\mathbb E_{Q_j}[-\log P_j(Y_j)].
$$

The analogous formula for $D(Q^{(i)}\Vert P^{(i)})$ omits coordinate $i$. Consequently

$$
\begin{aligned}
\sum_i\{D(Q\Vert P)-D(Q^{(i)}\Vert P^{(i)})\}
&=-nH(Q)+\sum_iH(Q^{(i)})\\
&\quad+\sum_j\mathbb E_{Q_j}[-\log P_j(Y_j)].
\end{aligned}
$$

Part b makes $\sum_iH(Q^{(i)})\geq(n-1)H(Q)$, so the last display is at least $D(Q\Vert P)$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
