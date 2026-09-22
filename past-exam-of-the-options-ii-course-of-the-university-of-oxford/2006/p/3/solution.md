<h1 id="p/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A real square [matrix](../../../../matrix.md) is orthogonal if $Q^TQ=I$. Then $\|Qx\|^2=x^TQ^TQx=x^Tx=\|x\|^2$, proving length preservation.

Define $J(i,j,\theta)$ to be identity outside rows and columns $i,j$, with block

$$
\begin{pmatrix}\cos\theta&\sin\theta\\-\sin\theta&\cos\theta\end{pmatrix}.
$$

The block's transpose times itself is identity because $\cos^2\theta+\sin^2\theta=1$ and the off-diagonal terms cancel. Thus $J$ is orthogonal, with [determinant](../../../../determinant.md) one.

For $r=\sqrt{x_i^2+x_j^2}>0$, choose $\cos\theta=x_i/r$, $\sin\theta=x_j/r$. Then $y_i=r$, $y_j=0$ and every other coordinate is unchanged. If $r=0$, choose $\theta=0$. This fixes the useful **nonnegative pivot convention**.

Apply the rotations to the current [matrix](../../../../matrix.md) in the displayed order from right to left. First $J(1,2)$ eliminates entry $(2,1)$; then $J(1,3)$ eliminates $(3,1)$ without changing row two. Finally $J(2,3)$ eliminates $(3,2)$ while preserving the zeros in column one. Thus

$$
\boxed{R=\begin{pmatrix}*&*&*\\0&*&*\\0&0&*\end{pmatrix},\qquad
Q=J(1,2)^TJ(1,3)^TJ(2,3)^T.}
$$

Inverting the product gives $A=QR$. Even if $A$ starts lower triangular, the row rotations generally create nonzero entries above the diagonal; there is no further universal simplification. For example $A=\left(\begin{smallmatrix}1&0&0\\1&1&0\\1&1&1\end{smallmatrix}\right)$ gives positive-pivot

$$
R=\begin{pmatrix}\sqrt3&2/\sqrt3&1/\sqrt3\\0&\sqrt{2/3}&1/\sqrt6\\0&0&1/\sqrt2\end{pmatrix},
$$

whose three entries above the diagonal are all nonzero.

If $A$ is orthogonal, $R$ is both [upper triangular](../../../../upper-triangular-matrix.md) and orthogonal. [Orthogonality](../../../../orthogonal-vectors.md) of its columns successively forces all off-diagonal entries to vanish and all diagonal entries to have absolute value one. The first two pivots are positive under our convention, and the rotations have [determinant](../../../../determinant.md) one. Therefore the precise result is

$$
\boxed{R=\operatorname{diag}(1,1,\det A).}
$$

Without a specified pivot-sign convention, the invariant statement is a diagonal [matrix](../../../../matrix.md) with entries $\pm1$ and product $\det A$.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [P](../../p.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
