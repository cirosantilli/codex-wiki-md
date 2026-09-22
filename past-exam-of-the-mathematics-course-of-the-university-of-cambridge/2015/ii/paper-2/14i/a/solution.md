<h1 id="14i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [graph Ramsey number](../../../../../../graph-ramsey-number.md) $R(s,t)$ is the least $N$ for which every [graph](../../../../../../graph-split.md) on $N$ vertices has a [clique](../../../../../../clique-graph-theory.md) of size $s$ or an [independent set](../../../../../../independent-set-graph-theory.md) of size $t$; $R(s)=R(s,s)$ is the [diagonal Ramsey number](../../../../../../diagonal-ramsey-number.md). The base cases are $R(2,t)=t$ and $R(s,2)=s$.

Assume the smaller parameters already have finite [graph Ramsey numbers](../../../../../../graph-ramsey-number.md), and take $N=R(s-1,t)+R(s,t-1)$. For any vertex, either its neighbourhood has at least $R(s-1,t)$ vertices, or its nonneighbourhood has at least $R(s,t-1)$ vertices. In the first case it contains an independent $t$-set, or an $(s-1)$-clique which extends with the chosen vertex. In the second it contains an $s$-clique, or a $(t-1)$-independent set which extends with that vertex. Induction proves existence and

$$
\boxed{R(s,t)\leq R(s-1,t)+R(s,t-1).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [14I](../../14i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
