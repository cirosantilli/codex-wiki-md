<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Name the outer pentagon vertices, in order from the client clockwise, $c,T,R,B,L$. Name the upper inner vertex $U$, the left inner vertex $A$, and the lower-right inner vertex $D$. The two remaining inner vertices are the labelled servers $s_1,s_2$.

Four edge-disjoint server paths are

$$
c-A-s_1,\qquad c-U-s_2,\qquad c-T-R-B-D-s_2,\qquad c-L-A-U-D-s_1.
$$

Each uses different links, although some intermediary vertices are shared. Any three failed links therefore leave at least one path intact. The client has exactly four incident links; failing those four disconnects it. Thus the minimum link cut has size four, giving

$$
\boxed{k_{\max}=3.}
$$

For mixed failures use the three paths $c-A-s_1$, $c-U-s_2$ and $c-T-R-B-D-s_1$. Their internal vertices are disjoint, as are their links. One failed link or intermediary node can destroy at most one of these paths, so any two failures leave a path intact. Failing the three intermediary nodes $A,U,D$ disconnects both servers: $s_1$ has neighbors $A,D$, and $s_2$ has neighbors $U,D$. Therefore

$$
\boxed{m_{\max}=2.}
$$

The two certificates distinguish [edge-disjoint paths](../../../../../../edge-disjoint-paths.md) from [internally vertex-disjoint paths](../../../../../../internally-vertex-disjoint-paths.md), exactly the distinction needed between the two failure models.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
