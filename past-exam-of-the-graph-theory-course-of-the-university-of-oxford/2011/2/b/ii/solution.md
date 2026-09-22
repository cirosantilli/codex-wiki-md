<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For each [vertex](../../../../../vertex-graph-theory.md) $v$, let $c(v)$ be the [maximum](../../../../../maximum-of-a-subset-of-a-total-order.md) number of [vertices](../../../../../vertex-graph-theory.md) in a [directed path](../../../../../directed-path.md) ending at $v$. These numbers lie between one and $\ell$.

If $u\to v$ is an [edge](../../../../../edge-of-a-graph.md), a longest [graph path](../../../../../path-in-a-graph.md) ending at $u$ cannot already contain $v$, since that would give a [directed cycle](../../../../../directed-cycle.md) on appending $u\to v$. Appending it therefore creates a [graph path](../../../../../path-in-a-graph.md) ending at $v$, so $c(v)\geq c(u)+1$. Adjacent [vertices](../../../../../vertex-graph-theory.md) consequently receive different colours. Hence

$$
\boxed{c\text{ is a proper colouring using at most }\ell\text{ colours}.}
$$

Acyclicity is exactly what justifies extending the [graph path](../../../../../path-in-a-graph.md) without repeating a [vertex](../../../../../vertex-graph-theory.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the graph theory course of the University of Oxford](../../../../split.md)
6. [Graph theory course of the University of Oxford](../../../../../graph-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
