<h1 id="18/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [matrix](../../../../../matrix.md) is symmetric under interchange of the first and third coordinates. For an antisymmetric [vector](../../../../../vector.md) $(1,0,-1)$, direct multiplication gives $A(1,0,-1)^{\mathsf T}=-6(1,0,-1)^{\mathsf T}$. For a symmetric [vector](../../../../../vector.md) $(p,q,p)$, the [linear transformation](../../../../../linear-map.md) reduces to

$$
\begin{pmatrix}p\\q\end{pmatrix}\longmapsto\begin{pmatrix}8&-4\\-8&4\end{pmatrix}\begin{pmatrix}p\\q\end{pmatrix}.
$$

The reduced [characteristic polynomial](../../../../../characteristic-polynomial.md) is $\lambda(\lambda-12)$. At $\lambda=0$, its equations give $q=2p$; at $\lambda=12$, they give $q=-p$. Normalizing the three [eigenvectors](../../../../../eigenvector.md) gives

$$
\boxed{\begin{aligned}
\lambda=-6:&\quad\mathbf v_-=(1,0,-1)^{\mathsf T}/\sqrt2,\\
\lambda=0:&\quad\mathbf v_0=(1,2,1)^{\mathsf T}/\sqrt6,\\
\lambda=12:&\quad\mathbf v_+=(1,-1,1)^{\mathsf T}/\sqrt3.
\end{aligned}}
$$

Their [norms](../../../../../norm.md) are one. Their unnormalized pairwise [dot products](../../../../../dot-product.md) are $1-1=0$, $1-1=0$ and $1-2+1=0$, proving mutual [orthogonality](../../../../../orthogonal-vectors.md). The [eigenvalues](../../../../../eigenvalue.md) sum to six and have product zero, agreeing with the [matrix trace](../../../../../matrix-trace.md) and [determinant](../../../../../determinant.md) from part (a).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [18](../../18.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
