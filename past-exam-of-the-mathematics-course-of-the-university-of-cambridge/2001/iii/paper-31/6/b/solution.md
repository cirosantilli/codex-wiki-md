<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [core of a cooperative game](../../../../../../core-game-theory.md) is the set of efficient allocations for which every [coalition](../../../../../../coalition-game-theory.md) receives at least its own value: $x(S)\ge v(S)$ for every $S\subseteq N$. The singleton constraints give individual rationality, and the remaining proper-coalition inequalities are

$$
x_1+x_2\ge3,\qquad x_1+x_3\ge10,\qquad x_2+x_3\ge6.
$$

Efficiency turns the second into $x_2\le2$; together with $x_2\ge2$ this forces $x_2=2$. Put $x_1=t$ and $x_3=10-t$. The remaining constraints give $t\ge1$, $t\le6$, and $t\le7$ from $x_3\ge3$. The first pair constraint adds only $t\ge1$. Hence

$$
\boxed{C(v)=\{(t,2,10-t):1\le t\le6\}.}
$$

Each point in this segment satisfies all singleton, pair, and grand-coalition constraints, so the description is sufficient as well as necessary. Its endpoints are $(1,2,9)$ and $(6,2,4)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
