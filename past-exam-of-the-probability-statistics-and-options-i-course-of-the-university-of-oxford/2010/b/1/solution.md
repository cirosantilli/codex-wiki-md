<h1 id="b/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Burnside lemma](../../../../burnside-s-lemma.md) states that the number of [orbits](../../../../orbit-dynamical-system.md) of a finite [group action](../../../../group-action-split.md) is

$$
|G|^{-1}\sum_{g\in G}|\operatorname{Fix}(g)|.
$$

For $m=2n-1\geq3$, the [dihedral group](../../../../dihedral-group.md) consists of $m$ rotations $r^j$ by $2\pi j/m$, and $m$ reflections $r^js$, each across the line through one vertex and the midpoint of the opposite edge. Thus $|G|=2m=4n-2$.

For the pentagon, the identity fixes $v^5e^5$ colourings. Each of the four nonidentity rotations has a single cycle on [vertices](../../../../vertex-graph-theory.md) and a single cycle on [edges](../../../../edge-of-a-graph.md), fixing $ve$ colourings. Each of the five reflections has one fixed vertex and two vertex pairs, and one fixed edge and two edge pairs, fixing $v^3e^3$ colourings. Applying the [Burnside lemma](../../../../burnside-s-lemma.md) to simultaneous vertex and edge colourings gives

$$
\boxed{\frac{v^5e^5+4ve+5v^3e^3}{10}.}
$$

Vertex colours and edge colours may be chosen independently; each symmetry must preserve both assignments.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [B](../../b.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
