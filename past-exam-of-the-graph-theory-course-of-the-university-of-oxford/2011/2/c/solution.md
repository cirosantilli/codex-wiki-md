<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix a proper [colouring](../../../../colouring-of-a-set.md) with exactly $k$ nonempty [colour classes](../../../../colour-class.md). For any class $C_i$, suppose every [vertex](../../../../vertex-graph-theory.md) in it misses at least one of the other $k-1$ colours in its [neighbourhood](../../../../neighbourhood-mathematics.md). Recolour each of these [vertices](../../../../vertex-graph-theory.md) by one of its missing colours. No [edge](../../../../edge-of-a-graph.md) joins two [vertices](../../../../vertex-graph-theory.md) of $C_i$, so these simultaneous recolourings cannot conflict with one another, and the chosen colours do not conflict with [vertices](../../../../vertex-graph-theory.md) outside $C_i$.

This would eliminate colour $i$ and produce a $(k-1)$-colouring, contradicting optimality. Therefore each [colour class](../../../../colour-class.md) contains a [vertex](../../../../vertex-graph-theory.md) adjacent to at least one [vertex](../../../../vertex-graph-theory.md) of every other colour. That [vertex](../../../../vertex-graph-theory.md) has degree at least $k-1$. Choosing one from each class gives $k$ distinct [vertices](../../../../vertex-graph-theory.md), proving

$$
\boxed{\bigl|\{v:\deg(v)\geq k-1\}\bigr|\geq k.}
$$

For $k=1$, a nonempty [graph](../../../../graph-split.md) already has a [vertex](../../../../vertex-graph-theory.md) of degree at least zero, so the conclusion holds as well.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the graph theory course of the University of Oxford](../../../split.md)
5. [Graph theory course of the University of Oxford](../../../../graph-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
