<h1 id="17i/solution">Solution</h1>

↑ **Parent:** [17I](../17i.md)

The [diagonal Ramsey number](../../../../../diagonal-ramsey-number.md) $R(s)$ is the least [positive integer](../../../../../positive-integer.md) $N$ such that every red-blue [edge colouring](../../../../../edge-coloring.md) of the [complete graph](../../../../../complete-graph.md) $K_N$ contains a [monochromatic](../../../../../monochromatic-set.md) copy of $K_s$.

For the existence and bound, write $R(r,s)$ for the least $N$ forcing either a red $K_r$ or a blue $K_s$. Given a vertex $v$ of $K_{R(r-1,s)+R(r,s-1)}$, the [pigeonhole principle](../../../../../pigeonhole-principle.md) says that at least $R(r-1,s)$ incident edges are red or at least $R(r,s-1)$ are blue. In the first case those red neighbours contain a red $K_{r-1}$, which joins to $v$ to make a red $K_r$, or a blue $K_s$; the second case is symmetric. Hence

$$
R(r,s)\leq R(r-1,s)+R(r,s-1).
$$

Starting from $R(1,s)=R(r,1)=1$ and using [Pascal's identity](../../../../../pascal-s-rule.md) gives the [binomial upper bound for a Ramsey number](../../../../../binomial-upper-bound-for-a-ramsey-number.md)

$$
R(r,s)\leq\binom{r+s-2}{r-1}.
$$

Therefore

$$
R(s)\leq\binom{2s-2}{s-1}<\sum_{j=0}^{2s-2}\binom{2s-2}{j}=2^{2s-2}<4^s,
$$

which proves both existence and the required estimate.

To determine $R(3)$, color a [cycle graph](../../../../../cycle-graph.md) $C_5$ red and its [complement graph](../../../../../complement-graph.md), also a $C_5$, yellow. This colors $K_5$ without a monochromatic triangle, so $R(3)>5$. At any vertex of a red-yellow $K_6$, at least three of the five incident edges have one color. If an edge among their three other endpoints has that color, it completes a monochromatic triangle with the chosen vertex; if none does, those three endpoints themselves form a triangle of the other color. Thus $R(3)\leq6$, and

$$
\boxed{R(3)=6}.
$$

The same local argument proves uniqueness on $K_5$. No vertex can have three incident edges of one color: their other endpoints would either contain an edge of that color or form a triangle of the other color. Every vertex therefore has [vertex degree](../../../../../degree-graph-theory.md) at most two in each color, and because the two degrees sum to four, each is exactly two. Each color class is consequently a [regular graph](../../../../../regular-graph.md) of degree two on five vertices, hence a single $C_5$. Up to relabelling, the coloring is exactly the cycle-and-complement coloring above.

Finally, the [monochromatic-triangle counting formula](../../../../../monochromatic-triangle-counting-formula.md) gives, for a coloring of $K_6$ with red degrees $d_v$,

$$
M=\binom63-\frac12\sum_vd_v(5-d_v)
\geq20-\frac12(6\cdot6)=2.
$$

The bound is attained by coloring all edges of $K_{3,3}$ red and the two complementary copies of $K_3$ yellow: there are no red triangles and exactly two yellow triangles. The least requested number is therefore

$$
\boxed{n=2}.
$$

## ↑ Ancestors (10)

1. [17I](../17i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
