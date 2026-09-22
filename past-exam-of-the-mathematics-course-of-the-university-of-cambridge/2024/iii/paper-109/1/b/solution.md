<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose symmetric chain decompositions of $\mathcal P(X_1)$ and $\mathcal P(X_2)$. Their Cartesian products partition $\mathcal P(X)$ into grids $C_1\times C_2$. Within one grid, two members in the same row differ only in $X_1$, and two in the same column differ only in $X_2$. The hypothesis on $\mathcal F$ therefore permits at most one member in each row and each column. Hence

$$
|\mathcal F\cap(C_1\times C_2)|
\leq\min\{|C_1|,|C_2|\}.
$$

Because $n_1$ and $n_2$ are even, both symmetric chains have odd length and are centred at ranks $n_1/2$ and $n_2/2$. The grid contains exactly $\min\{|C_1|,|C_2|\}$ points whose two ranks sum to $n/2$: they lie on its central antidiagonal. Thus the bound for $\mathcal F$ in each grid is the number of rank-$n/2$ subsets in that grid. Summing over all grids gives

$$
\boxed{|\mathcal F|\leq\binom n{n/2}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
