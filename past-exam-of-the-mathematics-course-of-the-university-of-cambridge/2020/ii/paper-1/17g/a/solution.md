<h1 id="17g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $G$ have $n$ vertices and $e$ edges. Its [complement graph](../../../../../../complement-graph.md) $\overline G$ has

$$
\binom n2-e
$$

edges. If both graphs were [planar](../../../../../../planar-graph.md), the [planar graph edge bound](../../../../../../planar-graph-edge-bound.md) would give

$$
\binom n2=e+e(\overline G)
\le(3n-6)+(3n-6)=6n-12.
$$

Equivalently, $n^2-13n+24\le0$, whose larger root is $(13+\sqrt{73})/2<11$. Thus an integer $n\ge11$ is impossible, proving that

$$
\boxed{\text{no planar graph of order greater than 10 has a planar complement}}.
$$

Now suppose that $G$ and $\overline G$ are both [bipartite](../../../../../../bipartite-graph.md). In a bipartition $V(G)=A\sqcup B$, every pair within $A$ and every pair within $B$ is adjacent in $\overline G$. Since a bipartite graph contains no triangle, $|A|,|B|\le2$, and hence $|V(G)|\le4$. Equality is attained by the path $P_4$, whose complement is again a copy of $P_4$. Therefore the maximum order is

$$
\boxed4.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17G](../../17g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
