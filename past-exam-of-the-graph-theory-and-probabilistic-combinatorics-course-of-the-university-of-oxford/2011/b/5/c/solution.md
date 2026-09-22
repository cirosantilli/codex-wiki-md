<h1 id="b/5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If there are no [triangles](../../../../../triangle-in-a-graph.md), any [edge colouring](../../../../../edge-coloring.md) works. Otherwise $\Delta\geq2$. Put $q=\lceil3\sqrt\Delta\rceil$ and colour each [edge](../../../../../edge-of-a-graph.md) independently and uniformly from $q$ colours. For each [triangle](../../../../../triangle-in-a-graph.md) $T$, let $A_T$ be the [event](../../../../../event.md) that its three [edges](../../../../../edge-of-a-graph.md) have one colour. Then

$$
\mathbb P(A_T)=q\left(\frac1q\right)^3=\frac1{q^2}.
$$

[Events](../../../../../event.md) for [triangles](../../../../../triangle-in-a-graph.md) sharing no [edge](../../../../../edge-of-a-graph.md) depend on disjoint edge-colour variables, so each [event](../../../../../event.md) is jointly [independent](../../../../../independent-random-variables.md) of the collection of all such nonneighbours. Each [edge](../../../../../edge-of-a-graph.md) of a [triangle](../../../../../triangle-in-a-graph.md) lies in at most $\Delta-2$ other [triangles](../../../../../triangle-in-a-graph.md): a common [neighbour](../../../../../neighbour-of-a-vertex.md) of its endpoints must be one of at most $\Delta-1$ [neighbours](../../../../../neighbour-of-a-vertex.md) besides the other endpoint, and one of these is the third [vertex](../../../../../vertex-graph-theory.md) of $T$ itself. Thus the dependency degree is at most $d=3(\Delta-2)$.

Because $q^2\geq9\Delta$,

$$
e\,\frac1{q^2}(d+1)\leq\frac{e(3\Delta-5)}{9\Delta}<\frac e3<1.
$$

The symmetric local lemma gives positive [probability](../../../../../probability.md) of avoiding every monochromatic [triangle](../../../../../triangle-in-a-graph.md). Hence

$$
\boxed{\lceil3\sqrt\Delta\rceil\text{ colours suffice}.}
$$

For an edgeless [graph](../../../../../graph-split.md) the empty [colouring](../../../../../colouring-of-a-set.md) handles even the zero-colour case $\Delta=0$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
