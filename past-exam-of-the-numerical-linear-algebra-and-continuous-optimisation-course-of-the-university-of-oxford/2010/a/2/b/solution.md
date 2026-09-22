<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An [orthogonal similarity transformation](../../../../../orthogonal-similarity.md) is $H=Q^TAQ$ with $Q^TQ=I$. An [upper Hessenberg matrix](../../../../../upper-hessenberg-matrix.md) has $H_{ij}=0$ whenever $i>j+1$; its first subdiagonal may be nonzero.

At step $k=1,\ldots,m-2$, choose a [Householder reflector](../../../../../householder-transformation.md) $Q_k=\operatorname{diag}(I_k,\widehat Q_k)$ whose trailing block sends the current column segment in rows $k+1,\ldots,m$ to a multiple of its first coordinate. The left multiplication zeros positions $(k+2,k),\ldots,(m,k)$. Apply the matching right multiplication to retain similarity: $A\leftarrow Q_k^TAQ_k$. Since $Q_k$ acts only on rows and columns $k+1,\ldots,m$, earlier Hessenberg zeros are preserved. Finally $Q=Q_1\cdots Q_{m-2}$ gives $H=Q^TAQ$.

Each reflector is applied through a rank-one update, costing $O(m^2)$ rather than a full matrix multiplication. Across $m-2$ steps, the [Hessenberg reduction](../../../../../hessenberg-reduction.md) costs $O(m^3)$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
