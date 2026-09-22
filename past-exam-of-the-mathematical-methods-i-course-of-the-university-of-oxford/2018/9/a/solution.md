<h1 id="9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The $j$th column of the [matrix representation of a linear map](../../../../matrix-representation-of-a-linear-map.md) is the [coordinate vector](../../../../coordinate-vector.md) of the image of the $j$th [basis vector](../../../../basis-vector.md):

$$
\phi(u_j)=\sum_iA_{ij}u_i.
$$

Define $C$ by $w_j=\sum_iC_{ij}u_i$, so its columns express the new [basis vectors](../../../../basis-vector.md) in the old [basis](../../../../basis.md). For every [vector](../../../../vector.md), $[v]_u=C[v]_w$. Applying $\phi$ in either coordinate system gives $AC[v]_w=CA'[v]_w$, proving the [change of basis](../../../../change-of-basis.md) formula

$$
\boxed{A'=C^{-1}AC.}
$$

To make $A'$ diagonal, choose the columns of $C$ to be [linearly independent](../../../../linear-independence.md) [eigenvectors](../../../../eigenvector.md) of $A$, expressed in the $u$ [basis](../../../../basis.md), and put their corresponding [eigenvalues](../../../../eigenvalue.md) on the diagonal in the same order. This is possible precisely when $A$ is a [diagonalizable matrix](../../../../diagonalizable-matrix.md) over the stated [field](../../../../field.md); an [eigenbasis](../../../../eigenbasis.md) need not exist over an arbitrary [field](../../../../field.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [9](../../9.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
