<h1 id="5e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Move the origin to the [centroid](../../../../../../centroid.md) and write the four vertex vectors as $r_1,r_2,r_3,r_4$. Their sum is zero. The [midpoints](../../../../../../midpoint.md) of the first opposite-edge pair have vectors $(r_1+r_2)/2$ and $(r_3+r_4)/2=-(r_1+r_2)/2$, so their distances from the [centroid](../../../../../../centroid.md) are equal. The same argument applies to the other two opposite-edge pairs.

Choose the three [midpoint](../../../../../../midpoint.md) distances as $u=|r_1+r_2|/2$, $v=|r_1+r_3|/2$, $w=|r_1+r_4|/2$. Expanding the [dot products](../../../../../../dot-product.md),

$$
4(u^2+v^2+w^2)=3|r_1|^2+\sum_{j=2}^4|r_j|^2+2r_1\cdot\sum_{j=2}^4r_j=\sum_{i=1}^4|r_i|^2.
$$

Identifying these four norms with the vertex distances proves the [tetrahedron centroid-to-midpoint sum of squares](../../../../../../tetrahedron-centroid-to-midpoint-sum-of-squares.md):

$$
\boxed{u^2+v^2+w^2=\frac14(a^2+b^2+c^2+d^2)}.
$$

The proof uses no orthogonality or regularity assumption on the [tetrahedron](../../../../../../tetrahedron.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5E](../../5e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
