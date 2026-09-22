<h1 id="17g/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [3-connected graph](../../../../../../3-connected-graph.md) contains a cycle, and any cycle is a [complete graph subdivision](../../../../../../complete-graph-subdivision.md) $TK_3$.

For $TK_4$, choose a cycle $C$ for which some $C$-bridge has at least three attachment vertices $a,b,c$; such a choice is always possible in a 3-connected graph. Indeed, every component outside a cycle has at least three attachments, since one or two would form a vertex cut, and if a chosen cycle is spanning, a chord can be used to choose a smaller cycle and expose the remaining bridge. In a minimal connected part of that bridge joining $a,b,c$, suppress degree-two vertices. The result has a branch vertex $w$ joined to $a,b,c$ by three paths whose interiors are mutually disjoint and avoid $C$. The three arcs of $C$ between $a,b,c$, together with these three paths, form a subdivision of the complete graph on branch vertices $w,a,b,c$. Hence

$$
\boxed{G\text{ contains a }TK_4}.
$$

A [3-connected graph](../../../../../../3-connected-graph.md) need not contain a $TK_5$. The [complete graph](../../../../../../complete-graph.md) $K_4$ itself is 3-connected and has only four [vertices](../../../../../../vertex-graph-theory.md), so it cannot contain a [graph subdivision](../../../../../../graph-subdivision.md) of $K_5$. Equally, any [planar](../../../../../../planar-graph.md) 3-connected graph is a counterexample because a subdivision of the complete graph $K_5$ would be nonplanar.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [17G](../../17g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
