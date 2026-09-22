<h1 id="21f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The simplices in a [barycentric subdivision](../../../../../../barycentric-subdivision.md) are strict chains of nonempty faces. A tetrahedron has $15$ nonempty faces, so $f_0=15$. Counting strict two-face chains gives

$$
f_1
=\sum_{j=1}^4\binom4j(2^j-2)
=50.
$$

A strict three-face chain amounts to choosing a terminal face and partitioning its vertices into three nonempty ordered blocks. Hence

$$
f_2
=\binom43\,3!\,S(3,3)+\binom44\,3!\,S(4,3)
=24+36=60,
$$

where $S(-,-)$ denotes a Stirling number of the second kind. Therefore

$$
\boxed{\chi(|M|)=f_0-f_1+f_2=15-50+60=25}.
$$

Equivalently, the full subdivision has $4!=24$ tetrahedra and Euler characteristic one, so deleting its three-dimensional simplices from the alternating count gives $1+24=25$. This is the f-vector computation for the [barycentric subdivision of a tetrahedron](../../../../../../barycentric-subdivision-of-a-tetrahedron.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [21F](../../21f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
