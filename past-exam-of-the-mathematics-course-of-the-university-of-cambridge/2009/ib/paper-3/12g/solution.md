<h1 id="12g/solution">Solution</h1>

↑ **Parent:** [12G](../12g.md)

For a polygonal cell decomposition of the sphere, [Euler characteristic](../../../../../euler-characteristic.md) gives

$$
\boxed{V-E+F=2.}
$$

Count incidences between faces and edges. Each edge borders two faces, and each face has at least three sides, so $2E\geq3F$. If every vertex had valence at least six, counting edge endpoints would also give $2E\geq6V$. Hence $V\leq E/3$ and $F\leq2E/3$, implying $V-E+F\leq0$, contrary to Euler's formula. Thus **some vertex has valence less than six**.

There is a missing qualification in the printed affine-line conclusion. Two distinct parallel lines have no intersection point, so its intersection condition holds vacuously, but they do not meet at a finite point. Even three or more distinct parallel lines give the same counterexample. Consequently that conclusion is false literally without a restriction on parallel lines.

Here is the intended spherical argument when the lines are pairwise nonparallel. Lift each line in the plane $z=1$ to the plane through it and the origin in $\mathbb R^3$; intersect these planes with the unit sphere to obtain [great circles](../../../../../great-circle.md). A common axis of all these planes meets $z=1$ in the required common point. Suppose no such axis exists. Their circle arrangement then decomposes the sphere into polygonal faces with at least three edges. To see why a two-sided face is impossible, its two great-circle edges would have antipodal endpoints. Every defining hemisphere containing that face would contain both endpoints and would therefore have its boundary plane through their axis, contradicting the absence of a common axis.

Every circle-arrangement vertex corresponds to an intersection of lifted planes. Because no two affine lines are parallel, this axis meets $z=1$, so the vertex corresponds to a finite intersection of the original lines. By the assumed multiplicity, at least three circles pass through it, giving valence at least six. This contradicts the preceding sphere count, proving concurrence in the nonparallel case. It is the [ordinary vertex in a nonconcurrent great-circle arrangement](../../../../../ordinary-vertex-in-a-nonconcurrent-great-circle-arrangement.md) argument.

Alternatively the corrected projective statement allows parallel lines, but requires the intersection condition at infinity as well, and concludes concurrence at a possibly infinite projective point. The same great-circle proof applies; concurrence at infinity represents a parallel family. The printed condition about finite affine intersections alone must not be used to assert a finite common point for such a family.

## ↑ Ancestors (10)

1. [12G](../12g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
