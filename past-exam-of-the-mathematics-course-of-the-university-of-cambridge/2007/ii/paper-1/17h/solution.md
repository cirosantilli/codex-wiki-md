<h1 id="17h/solution">Solution</h1>

↑ **Parent:** [17H](../17h.md)

Label four face colors by $\mathbb F_2^2$. Give each edge the sum of its two adjacent face labels. This is nonzero because adjacent faces differ. At a cubic vertex the three face labels are pairwise distinct, so their three edge sums are the three different nonzero elements. This is a [Tait coloring](../../../../../tait-coloring.md).

Conversely, label the three edge colors by the nonzero elements of $\mathbb F_2^2$, whose sum is zero. Choose a base face with label zero and label any other face by summing crossed edge labels along a path in the [dual graph](../../../../../dual-graph.md). The result is independent of the path: a simple closed dual path encloses vertices, and summing the zero incident sums at these vertices leaves exactly its crossed boundary edges, since interior edges occur twice. General closed paths decompose into such cycles. Adjacent labels differ by a nonzero edge label, giving a four-color face coloring. The assumption that every edge borders distinct faces excludes [bridges in a graph](../../../../../bridge-graph-theory.md) and ensures this map coloring is the relevant one.

**The equivalence fails on a torus.** Use the [Heawood torus map](../../../../../heawood-torus-map.md). On seven vertices indexed modulo seven, take the triangles $A_i=(i,i+1,i+3)$ and $B_i=(i,i+3,i+2)$. Each edge of $K_7$ occurs in exactly two oppositely oriented triangles; each vertex link is a six-cycle, for example $1,3,2,6,4,5,1$ at zero. This is a connected closed orientable surface with [Euler characteristic](../../../../../euler-characteristic.md) $7-21+14=0$, hence a [torus](../../../../../torus.md).

Its [dual graph](../../../../../dual-graph.md) is cubic, with $A_i$ adjacent to $B_i,B_{i+1},B_{i-2}$. The three offsets partition its edges into [perfect matchings](../../../../../perfect-matching.md), giving a [Tait coloring](../../../../../tait-coloring.md). Its seven faces are discs and their adjacency graph is $K_7$, so they need seven colors. The obstruction to the planar proof is a possible nonzero edge-label sum around a noncontractible cycle.

## ↑ Ancestors (10)

1. [17H](../17h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
