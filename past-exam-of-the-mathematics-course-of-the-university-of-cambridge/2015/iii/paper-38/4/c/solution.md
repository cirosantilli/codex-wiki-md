<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The displayed graph consists of three [graph triangles](../../../../../../triangle-in-a-graph.md) sharing the vertex $v$. In a [graph colouring](../../../../../../graph-coloring.md) with three colours, every [graph triangle](../../../../../../triangle-in-a-graph.md) uses all three colours. The edge $tf$ and the edges $tv,fv$ therefore force $c(t),c(f)$ to be the two colours different from $c(v)$. Likewise the [graph triangle](../../../../../../triangle-in-a-graph.md) $vxy$ forces $c(x),c(y)$ to be those same two colours. The third [graph triangle](../../../../../../triangle-in-a-graph.md) imposes no further restriction on these four vertices. Hence

$$
\boxed{\{c(t),c(f)\}=\{c(x),c(y)\},\qquad c(t)\ne c(f),\quad c(x)\ne c(y).}
$$

Both two-element sets and their union have cardinality two. This is a [Boolean-pair colouring gadget](../../../../../../boolean-pair-colouring-gadget.md): after fixing a palette [graph triangle](../../../../../../triangle-in-a-graph.md), the pair $x,y$ encodes opposite truth values.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
