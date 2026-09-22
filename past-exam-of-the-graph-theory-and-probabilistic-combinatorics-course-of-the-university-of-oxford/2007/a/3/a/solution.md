<h1 id="a/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Ramsey number](../../../../../ramsey-number.md) $R(k,l)$ is the least $N$ such that every [graph](../../../../../graph-split.md) on $N$ vertices has a $k$-[clique](../../../../../clique-graph-theory.md) or an [independent set](../../../../../independent-set-graph-theory.md) of size $l$. Choose a vertex in a [graph](../../../../../graph-split.md) of order $R(k-1,l)+R(k,l-1)$. It has either at least $R(k-1,l)$ neighbours or at least $R(k,l-1)$ nonneighbours. In the first set, a $(k-1)$-[clique](../../../../../clique-graph-theory.md) extends with the vertex to a $k$-[clique](../../../../../clique-graph-theory.md), while an independent $l$-set already suffices. The complementary argument handles the second set. Thus

$$
R(k,l)\le R(k-1,l)+R(k,l-1).
$$

The boundary values are $R(k,2)=k$ and $R(2,l)=l$. Induction on $k+l$, using Pascal's identity, therefore gives

$$
\boxed{R(k,l)\le\binom{k+l-3}{k-2}+\binom{k+l-3}{k-1}=\binom{k+l-2}{k-1}}.
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
