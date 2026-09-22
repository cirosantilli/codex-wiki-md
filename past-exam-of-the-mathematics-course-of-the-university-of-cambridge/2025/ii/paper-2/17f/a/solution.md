<h1 id="17f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A matching from $X$ to $Y$ is a set of pairwise vertex-disjoint edges that covers every vertex of $X$. Equivalently, it chooses for each $x\in X$ a distinct neighbour in $Y$.

[Hall marriage theorem](../../../../../../hall-s-marriage-theorem.md) says that such a matching exists if and only if

$$
|N(S)|\geq |S|\qquad\text{for every }S\subseteq X.
$$

Necessity is immediate: the distinct partners of the vertices in $S$ all belong to $N(S)$.

For sufficiency, induct on $|X|$. The claim is clear when $|X|=1$. First suppose every nonempty proper $S\subset X$ satisfies the strict inequality $|N(S)|\geq |S|+1$. Choose an edge $xy$ and delete $x$ and $y$. For $S\subseteq X\setminus\{x\}$, deletion removes at most one neighbour, so

$$
|N_{G-\{x,y\}}(S)|\geq |N_G(S)|-1\geq |S|.
$$

Induction gives a matching of $X\setminus\{x\}$, and adding $xy$ completes it.

Otherwise there is a nonempty proper $S\subset X$ with $|N(S)|=|S|$. Hall's condition holds in the bipartite graph induced by $S\cup N(S)$, so induction matches $S$ onto $N(S)$. For $A\subseteq X\setminus S$,

$$
|N(A\cup S)|\geq |A|+|S|,
$$

and hence $A$ has at least $|A|$ neighbours outside $N(S)$. Induction therefore matches $X\setminus S$ into $Y\setminus N(S)$. The two matchings are disjoint and together cover $X$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17F](../../17f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
