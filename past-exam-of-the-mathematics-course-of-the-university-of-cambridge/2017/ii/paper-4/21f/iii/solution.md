<h1 id="21f/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Apply the [spectral theorem for compact Hermitian operators](../../../../../../spectral-theorem-for-compact-hermitian-operators.md) to positive $A=T^*T$. Its positive [eigenvalues](../../../../../../eigenvalue.md) $\mu_i$ have [orthonormal](../../../../../../orthonormal-set.md) [eigenvectors](../../../../../../eigenvector.md) $u_i$ spanning $\ker A^\perp$, with a finite or countable list. In the infinite case $\mu_i\to0$. Define

$$
\lambda_i=\sqrt{\mu_i}>0,\qquad v_i=\frac{Tu_i}{\lambda_i}.
$$

Then $(v_i,v_j)=(u_i,T^*Tu_j)/(\lambda_i\lambda_j)=\delta_{ij}$, so the $v_i$ are orthonormal. Also $\ker A=\ker T$, because $(x,Ax)=\|Tx\|^2$. Decompose $x=x_0+\sum_i(u_i,x)u_i$ with $x_0\in\ker T$ and apply bounded $T$ to the norm-convergent expansion. This gives the [singular value decomposition](../../../../../../singular-value-decomposition.md)

$$
\boxed{Tx=\sum_{i=1}^N\lambda_i(u_i,x)v_i.}
$$

The series converges in [norm](../../../../../../norm.md); its squared tail [norm](../../../../../../norm.md) is $\sum_{i>m}\mu_i|(u_i,x)|^2\to0$. No separability of the whole [Hilbert space](../../../../../../hilbert-space-split.md) is necessary: the nonzero spectral subspace of a [compact operator](../../../../../../compact-operator-split.md) is separable. For $T=0$ use the empty list $N=0$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [21F](../../21f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
