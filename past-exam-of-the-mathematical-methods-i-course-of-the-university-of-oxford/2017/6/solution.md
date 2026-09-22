<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

With the [Einstein summation convention](../../../einstein-notation.md), the [magnetic force](../../../magnetic-force.md) has components $F_i=q\epsilon_{ijk}v_jB_k$. Thus its matrix acting on velocity is

$$
\boxed{M_{ij}=q\epsilon_{ijk}B_k,\qquad
M=q\begin{pmatrix}0&B_z&-B_y\\-B_z&0&B_x\\B_y&-B_x&0\end{pmatrix}.}
$$

The [Levi-Civita symbol](../../../levi-civita-symbol.md) changes sign on exchanging $i,j$, so $M^T=-M$; the diagonal vanishes and the matrix has zero [trace](../../../matrix-trace.md). For nonzero $\mathbf B$, $M\mathbf B=q\mathbf B\times\mathbf B=0$, exhibiting a nontrivial [kernel](../../../kernel-of-a-linear-map-split.md) and proving noninvertibility. If $\mathbf B=0$ or $q=0$, $M$ is the zero matrix and is again noninvertible.

Equivalently, an odd-dimensional real [antisymmetric matrix](../../../skew-symmetric-matrix.md) has $\det M=\det M^T=\det(-M)=-\det M$, hence zero [determinant](../../../determinant.md). The same antisymmetry gives $\mathbf v^TM\mathbf v=0$, expressing that the magnetic force does no work.

## ↑ Ancestors (11)

1. [6](../6.md)
2. [2017](../../2017-split.md)
3. [Past exam of the mathematical methods I course of the University of Oxford](../../split.md)
4. [Mathematical methods I course of the University of Oxford](../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
