<h1 id="3/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Here is an explicit [simplicial complex](../../../../../simplicial-complex.md) on six vertices. Take every subset of one of the following ten triangular facets:

$$
\boxed{123,\ 124,\ 135,\ 146,\ 156,\ 236,\ 245,\ 256,\ 345,\ 346.}
$$

For example, $135$ denotes $\{1,3,5\}$, with all its edges and vertices included. Its [one-skeleton](../../../../../1-skeleton.md) has all fifteen edges of the [complete graph](../../../../../complete-graph.md). Every edge belongs to exactly two triangles. The [links of a simplex](../../../../../link-of-a-simplex.md) at the six vertices are the following cycles, with the first vertex understood to repeat at the end:

$$
\begin{array}{c|c}
\text{vertex}&\text{link cycle}\\\hline
1&2,3,5,6,4\\
2&1,3,6,5,4\\
3&1,2,6,4,5\\
4&1,2,5,3,6\\
5&1,3,4,2,6\\
6&1,4,3,2,5
\end{array}
$$

Thus every vertex has a disk neighbourhood, as do edge and face interior points. The realization is a compact connected [surface](../../../../../topological-surface-split.md) without boundary. Its [Euler characteristic](../../../../../euler-characteristic.md) is

$$
\chi=V-E+F=6-15+10=1.
$$

The [classification theorem for surfaces](../../../../../classification-theorem-for-surfaces.md) identifies the unique closed connected surface with this Euler characteristic as the [real projective plane](../../../../../real-projective-plane.md). Consequently **this complex triangulates $\mathbb{RP}^2$**. The explicit facet and link checks make this a genuine [simplicial complex](../../../../../simplicial-complex.md), not a polygon whose boundary identifications have been mistaken for simplicial faces.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the topology course of the University of Oxford](../../../../split.md)
6. [Topology course of the University of Oxford](../../../../../topology-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
