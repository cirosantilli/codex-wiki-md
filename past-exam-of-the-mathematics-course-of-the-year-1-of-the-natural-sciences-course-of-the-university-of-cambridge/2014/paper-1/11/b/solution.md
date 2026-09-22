<h1 id="11/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The symmetry between the first and third coordinates makes $(1,0,-1)^{\mathsf T}$ an [eigenvector](../../../../../eigenvector.md), with [eigenvalue](../../../../../eigenvalue.md) $-6$. In the remaining invariant [plane](../../../../../plane.md), write a [vector](../../../../../vector.md) as $(s,t,s)^{\mathsf T}$. Its image is $(8s-4t,-8s+4t,8s-4t)^{\mathsf T}$, so the reduced [eigenvalue](../../../../../eigenvalue.md) equation has [determinant](../../../../../determinant.md)

$$
\det\begin{pmatrix}8-\lambda&-4\\-8&4-\lambda\end{pmatrix}
=\lambda(\lambda-12).
$$

The corresponding directions have $t=2s$ for $\lambda=0$ and $t=-s$ for $\lambda=12$. Normalizing gives

$$
\boxed{\begin{array}{c|c}
\lambda=-6&\mathbf e_-=(1,0,-1)^{\mathsf T}/\sqrt2\\[2pt]
\lambda=0&\mathbf e_0=(1,2,1)^{\mathsf T}/\sqrt6\\[2pt]
\lambda=12&\mathbf e_+=(1,-1,1)^{\mathsf T}/\sqrt3.
\end{array}}
$$

Their squared unnormalized norms are $2,6,3$. The pairwise unnormalized [dot products](../../../../../dot-product.md) are $1-1=0$, $1-1=0$, and $1-2+1=0$, so these unit [eigenvectors](../../../../../eigenvector.md) are mutually orthogonal. The [eigenvalues](../../../../../eigenvalue.md) sum to $6$ and have product zero, agreeing with part (a).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [11](../../11.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
