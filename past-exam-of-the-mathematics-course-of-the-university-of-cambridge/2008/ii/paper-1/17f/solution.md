<h1 id="17f/solution">Solution</h1>

↑ **Parent:** [17F](../17f.md)

[Euler characteristic](../../../../../euler-characteristic.md) for a finite connected plane graph is $v-e+f=2$. For a simple connected [planar graph](../../../../../planar-graph.md) with $v\geq3$, each facial boundary has length at least three and the total boundary length is $2e$, so $3f\leq2e$. Combining gives $e\leq3v-6$, and therefore [average degree of a graph](../../../../../average-degree-of-a-graph.md) $2e/v<6$. Some vertex has degree at most five. Components of size one or two have this property directly, so every nonempty finite simple [planar graph](../../../../../planar-graph.md) has $\delta(G)\leq5$.

Prove [five colour theorem](../../../../../five-color-theorem.md) by induction on vertex count. Remove a vertex $x$ of degree at most five and colour the remaining [planar graph](../../../../../planar-graph.md) with five colours. If its neighbours use fewer than five colours, assign an unused colour to $x$. Otherwise its five neighbours $x_1,\ldots,x_5$ occur in cyclic order around $x$ with colours $1,\ldots,5$. If no path of colours $1,3$ connects $x_1$ to $x_3$, interchange these colours in the component of $x_1$, freeing colour 1 at $x$.

If such a path exists, a simple path together with $xx_1$ and $xx_3$ makes a Jordan curve. The cyclic order puts $x_2$ and $x_4$ on opposite sides. A path of colours $2,4$ between them would have to cross the curve, impossible in the plane embedding; it cannot meet the differently coloured path or use the removed vertex. Interchange colours $2,4$ in the component of $x_2$, freeing colour 2 at $x$. The colouring extends in every case. Thus **$\chi(G)\leq5$** for finite simple [planar graphs](../../../../../planar-graph.md). The usual simple-graph convention is needed: loops would invalidate a proper-colouring assertion.

## ↑ Ancestors (10)

1. [17F](../17f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
