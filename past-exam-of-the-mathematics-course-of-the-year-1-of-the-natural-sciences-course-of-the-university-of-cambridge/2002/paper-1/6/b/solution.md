<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $\mathbf u=(1,1)^T$ and $\mathbf v=(1,-1)^T$, the [outer products](../../../../../outer-product.md) are

$$
\mathbf u\mathbf u^T=\begin{pmatrix}1&1\\1&1\end{pmatrix},\qquad \mathbf v\mathbf v^T=\begin{pmatrix}1&-1\\-1&1\end{pmatrix}.
$$

Their [inner product](../../../../../inner-product-split.md) is zero and both squared [norms](../../../../../norm.md) are two. Thus $P_u=\mathbf u\mathbf u^T/2$ and $P_v=\mathbf v\mathbf v^T/2$ are orthogonal [spectral projectors](../../../../../spectral-projector.md), with $P_u+P_v=I$. Since $A\mathbf u=5\mathbf u$ and $A\mathbf v=\mathbf v$, the [eigenvalues](../../../../../eigenvalue.md) are $\lambda=5$, $\mu=1$, and

$$
\boxed{A=\frac52\mathbf u\mathbf u^T+\frac12\mathbf v\mathbf v^T,\qquad A^{-1}=\frac1{10}\mathbf u\mathbf u^T+\frac12\mathbf v\mathbf v^T.}
$$

Multiplying these decompositions uses $P_uP_v=0$ and $P_u^2=P_u$, $P_v^2=P_v$, giving the [identity matrix](../../../../../identity-matrix.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
