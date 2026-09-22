<h1 id="b/b1/solution">Solution</h1>

↑ **Parent:** [B1](../b1.md)

[Burnside's lemma](../../../../burnside-s-lemma.md) gives the number of orbits as

$$
|\Omega/G|=\frac1{|G|}\sum_{g\in G}|\operatorname{Fix}(g)|.
$$

For $m=2n-1\geq3$, the polygon symmetry [group](../../../../group-split.md) contains the $m$ rotations through angles $2\pi j/m$, $0\leq j<m$, and $m$ reflections. Each [reflection](../../../../reflection-mathematics.md) axis passes through a vertex and the midpoint of the opposite edge. These are all the symmetries, so $|G|=2m=\boxed{4n-2}$.

For the pentagon, apply the same [group](../../../../group-split.md) element simultaneously to vertex colours and edge colours. The identity fixes $v^5e^5$ colourings. Each of the four nonidentity rotations is a 5-cycle on vertices and also on edges, fixing $ve$ colourings. Each of the five reflections has one fixed vertex and two swapped vertex pairs, and one fixed edge and two swapped edge pairs. It therefore fixes $v^3e^3$ colourings. Averaging yields

$$
\boxed{\frac{v^5e^5+4ve+5v^3e^3}{10}.}
$$

The two colour palettes are chosen independently, but rotations and reflections act on both parts of the same pentagon.

## ↑ Ancestors (12)

1. [B1](../b1.md)
2. [B](../../b.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
