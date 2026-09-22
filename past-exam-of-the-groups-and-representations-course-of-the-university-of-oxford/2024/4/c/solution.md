<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the standard chain ordering of the five simple [roots](../../../../root-of-a-root-system.md) of $SU(6)$. A [Young diagram](../../../../young-diagram.md) of row lengths $r_1\geq\cdots\geq r_6=0$ has [highest weight](../../../../highest-weight-of-a-representation.md) [Dynkin labels](../../../../dynkin-label.md) $a_i=r_i-r_{i+1}$. A full column of six boxes can be removed because it is the trivial [determinant representation](../../../../determinant-representation.md). The required data are

$$
\boxed{\begin{array}{c|c|c|c|r}
\text{representation}&(a_1,a_2,a_3,a_4,a_5)&\text{row lengths}&\text{tensor}&\dim\\\hline
\mathbf6&(1,0,0,0,0)&[1]&v^i&6\\
\bar{\mathbf6}&(0,0,0,0,1)&[1,1,1,1,1]&w_i&6\\
\mathbf{21}&(2,0,0,0,0)&[2]&S^{ij}=S^{ji}&21\\
\mathbf{15}&(0,1,0,0,0)&[1,1]&A^{ij}=-A^{ji}&15\\
\mathbf{35}&(1,0,0,0,1)&[2,1,1,1,1]&M^i{}_j,\ M^i{}_i=0&35
\end{array}.}
$$

In the same order, the [Young tableaux](../../../../young-tableau.md) are

$$
\square,\qquad
\begin{array}{l}\square\\[-4pt]\square\\[-4pt]\square\\[-4pt]\square\\[-4pt]\square\end{array},\qquad
\square\,\square,\qquad
\begin{array}{l}\square\\[-4pt]\square\end{array},\qquad
\begin{array}{l}\square\,\square\\[-4pt]\square\\[-4pt]\square\\[-4pt]\square\\[-4pt]\square\end{array}.
$$

Each upper index transforms by $U$, and each lower index by $U^{-1}$. In particular $M\mapsto UMU^{-1}$ is the complex [Adjoint representation](../../../../adjoint-representation-of-a-lie-algebra.md). The column of five boxes can be represented either by $w_i$ or by the totally [antisymmetric tensor](../../../../antisymmetric-tensor.md) $B^{i_1\ldots i_5}$, using the invariant six-index alternating tensor:

$$
w_j=\frac1{5!}\epsilon_{j i_1\ldots i_5}B^{i_1\ldots i_5}.
$$

Thus it really is the [conjugate representation](../../../../conjugate-representation.md), rather than a second independent six-dimensional choice. Similarly converting the lower index of $M^i{}_j$ into five alternating upper indices gives the displayed hook [Young diagram](../../../../young-diagram.md); the removed [trace](../../../../matrix-trace.md) would be its full six-box column component.

The dimension counts are

$$
\dim\operatorname{Sym}^2\mathbb C^6=\frac{6\cdot7}{2}=21,\qquad
\dim\Lambda^2\mathbb C^6=\frac{6\cdot5}{2}=15,\qquad
\dim\operatorname{End}_0(\mathbb C^6)=6^2-1=35.
$$

The first two count independent entries of [symmetric tensors](../../../../symmetric-tensor.md) and [antisymmetric tensors](../../../../antisymmetric-tensor.md); the last removes one [trace](../../../../matrix-trace.md) from a mixed [tensor](../../../../tensor.md). The [hook-content formula](../../../../hook-content-formula.md) independently gives these dimensions from the [Young diagrams](../../../../young-diagram.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
