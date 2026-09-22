<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Work in three-dimensional [projective space](../../../../../projective-space-split.md), with four [homogeneous coordinates](../../../../../homogeneous-coordinate.md) indexed $0,1,2,3$. Let $A$ and $B$ be independent representatives of two points. The [Plücker coordinates](../../../../../plucker-coordinates.md) of their line are

$$
\boxed{L^{ij}=A^iB^j-B^iA^j.}
$$

This [antisymmetric matrix](../../../../../skew-symmetric-matrix.md) has rank two and is defined only up to a nonzero scalar. Replacing the pair by another [basis](../../../../../basis.md) of the same two-dimensional subspace multiplies $L$ by the determinant of that basis change. Its six independent entries satisfy $L^{01}L^{23}-L^{02}L^{13}+L^{03}L^{12}=0$, since the [exterior product](../../../../../exterior-product.md) $(A\wedge B)\wedge(A\wedge B)$ vanishes.

To describe the same line as an intersection of planes, choose a volume orientation with $\varepsilon_{0123}=1$ and define the dual [Plücker coordinates](../../../../../plucker-coordinates.md) by

$$
\boxed{L_{ij}=\frac12\varepsilon_{ijkl}L^{kl}.}
$$

The independent components pair as

$$
L_{01}=L^{23},\quad L_{02}=-L^{13},\quad L_{03}=L^{12},\quad
L_{12}=L^{03},\quad L_{13}=-L^{02},\quad L_{23}=L^{01}.
$$

Conversely, $L^{ij}=\tfrac12\varepsilon^{ijkl}L_{kl}$ with the matching volume convention. The lower-index form annihilates both defining points: $L_{ij}A^j=L_{ij}B^j=0$. Its columns span the pencil of planes containing their line. This dualization uses the volume form, **not a Euclidean metric for raising and lowering indices**. Two-index point and plane representations are dual in projective dimension three; in higher dimensions the corresponding dual exterior form has a different degree.

For a general plane covector $F_i$, contract the upper-index form:

$$
\boxed{P^i=L^{ij}F_j=A^i(F_jB^j)-B^i(F_jA^j).}
$$

This is a [linear combination](../../../../../linear-combination.md) of $A,B$, so it is on the line, and $F_iP^i=0$ by antisymmetry, so it is on the plane. Provided the resulting vector is nonzero, its [homogeneous coordinates](../../../../../homogeneous-coordinate.md) give the unique intersection, including intersections at infinity. If $F(A)=F(B)=0$, the whole line lies in the plane and the zero result correctly indicates that there is no unique intersection. These are the [line-plane incidence in Plücker coordinates](../../../../../line-plane-incidence-in-plucker-coordinates.md) operations used in the subparts.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
