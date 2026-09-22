<h1 id="17f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The first assertion is **false**. The [complete graph](../../../../../../complete-graph.md) $K_4$ has $\chi(K_4)=4$, but $\chi'(K_4)=3$: color each of its three perfect matchings with its own color. It is connected and has more than two vertices.

The second assertion is **false**. Take the [crown graph](../../../../../../crown-graph.md) with bipartition $a_1,\ldots,a_5$ and $b_1,\ldots,b_5$, joining $a_i$ to $b_j$ exactly when $i\ne j$. Its [chromatic number](../../../../../../chromatic-number.md) is two. In the ordering $a_1,b_1,a_2,b_2,\ldots,a_5,b_5$, the [greedy coloring](../../../../../../greedy-coloring.md) algorithm assigns color $i$ to both $a_i,b_i$: both see all previously used colors, but they are not adjacent to each other. It therefore uses five colors, exceeding $2\chi(G)=4$. Taking more pairs makes the ratio arbitrarily large.

The third assertion is **true**. When an edge is colored greedily, at most $2\Delta-2$ adjacent edges have previously received colors. Thus the [greedy coloring](../../../../../../greedy-coloring.md) algorithm uses at most $2\Delta-1\le2\chi'(G)-1<2\chi'(G)$ colors whenever the graph has an edge. The edgeless case is trivial. This bound holds for every edge ordering.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [17F](../../17f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
