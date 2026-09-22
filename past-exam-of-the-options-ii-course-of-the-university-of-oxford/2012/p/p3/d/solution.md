<h1 id="p/p3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $J_1,J_2,J_3$ for the actual successive [rotations](../../../../../rotation-mathematics.md) $J(1,2)$, $J(1,3)$, and $J(2,3)$, each selected using the currently transformed [matrix](../../../../../matrix.md). The first eliminates position $(2,1)$; the second eliminates $(3,1)$ while leaving row two unchanged. After these, the first column is $(r_{11},0,0)^T$. The final [rotation](../../../../../rotation-mathematics.md) of rows two and three preserves both zeros in that column and eliminates $(3,2)$. Hence

$$
\boxed{R=J_3J_2J_1A\text{ is upper triangular}.}
$$

A lower-triangular starting [matrix](../../../../../matrix.md) does not [force](../../../../../force-split.md) any further zeros above the diagonal. For example, the lower-triangular [matrix](../../../../../matrix.md) with all entries on and below its diagonal equal to one gives, with the nonnegative [pivot](../../../../../pivotal-quantity.md) convention,

$$
R=\begin{pmatrix}\sqrt3&2/\sqrt3&1/\sqrt3\\0&\sqrt{2/3}&1/\sqrt6\\0&0&1/\sqrt2\end{pmatrix},
$$

which has all upper-triangular entries nonzero.

Inverting the product of [rotations](../../../../../rotation-mathematics.md) yields the [QR factorization](../../../../../qr-decomposition.md)

$$
\boxed{Q=J_1^TJ_2^TJ_3^T,\qquad A=QR.}
$$

The order reverses when taking the [transpose](../../../../../transpose.md). If $A$ is [orthogonal](../../../../../orthogonal-vectors.md), then $R$ is both [orthogonal](../../../../../orthogonal-vectors.md) and [upper triangular](../../../../../upper-triangular-matrix.md). Its first column forces $|r_{11}|=1$ and [orthogonality](../../../../../orthogonal-vectors.md) with the other columns forces $r_{12}=r_{13}=0$. Applying the same argument to the remaining block makes $R$ diagonal with entries of modulus one.

Our elimination rule makes $r_{11}$ and $r_{22}$ positive when nonzero, so they are both one. Every [rotation](../../../../../rotation-mathematics.md) has [determinant](../../../../../determinant.md) one; thus $\det R=\det A$ and

$$
\boxed{R=\operatorname{diag}(1,1,\det A).}
$$

Without a fixed pivot-sign convention one could only specify a diagonal sign [matrix](../../../../../matrix.md). The convention chosen in part (c) determines the precise signs above.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [P3](../../p3.md)
3. [P](../../../p.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
