<h1 id="17f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

In any two-colouring of $K_7$, there is a monochromatic triangle because $f(2)=6$. Call its colour blue. If any [edge](../../../../../../edge-of-a-graph.md) from one of its vertices to an outside [vertex](../../../../../../vertex-graph-theory.md) is blue, the triangle and that [edge](../../../../../../edge-of-a-graph.md) give the required copy of $H$. Otherwise all [edges](../../../../../../edge-of-a-graph.md) from that triangle to the four outside vertices are yellow. If any [edge](../../../../../../edge-of-a-graph.md) among those four is yellow, it makes a yellow triangle with a [vertex](../../../../../../vertex-graph-theory.md) of the original triangle, and another incident yellow [edge](../../../../../../edge-of-a-graph.md) supplies the pendant [edge](../../../../../../edge-of-a-graph.md). If none is yellow, the four outside vertices form a blue $K_4$, which also contains $H$. Hence $g(2)\le7$.

For the lower bound, divide six vertices into two triples. Colour [edges](../../../../../../edge-of-a-graph.md) inside each triple blue and all cross-edges yellow. Each blue component is only a triangle, and the yellow graph is bipartite, so neither colour contains $H$. Therefore **$\boxed{g(2)=7}$**. Copies are not required to be induced: an additional [edge](../../../../../../edge-of-a-graph.md) in a monochromatic $K_4$ does not invalidate the copy of $H$.

For three colours, $f(3)=17$ supplies a triangle in $K_{17}$. If it has no pendant [edge](../../../../../../edge-of-a-graph.md) of the same colour, each of its vertices has fourteen [edges](../../../../../../edge-of-a-graph.md) to outside vertices in the other two colours. Choose one [vertex](../../../../../../vertex-graph-theory.md) $v$ and a colour occurring on at least seven of those [edges](../../../../../../edge-of-a-graph.md), with endpoint set $S$. If an internal [edge](../../../../../../edge-of-a-graph.md) of $S$ has this colour, it creates a triangle with $v$ and a fourth neighbour supplies the pendant [edge](../../../../../../edge-of-a-graph.md). Otherwise $S$ is internally two-coloured, and $g(2)=7$ supplies $H$. Thus $g(3)\le17$. Conversely the definition $f(3)=17$ ensures a three-colouring of $K_{16}$ without any monochromatic triangle, and therefore without $H$. Hence **$\boxed{g(3)=17}$**.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [17F](../../17f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
