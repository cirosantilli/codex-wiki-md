<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $h=\Delta x=1/(M+1)$. The semidiscrete matrix is $B=h^{-2}\operatorname{tridiag}(1,-2,1)+\kappa I$. For $j=1,\ldots,M$, set $v_m^{(j)}=\sin(j\pi m/(M+1))$. The endpoint values vanish and the sine addition formula gives

$$
Bv^{(j)}=\lambda_j v^{(j)},\qquad
\lambda_j=\kappa-\frac4{h^2}\sin^2\frac{j\pi}{2(M+1)}.
$$

These form an [orthogonal basis](../../../../../../orthogonal-basis.md) of [eigenvectors](../../../../../../eigenvector.md). Every initial vector decays precisely when every [eigenvalue](../../../../../../eigenvalue.md) is negative. Since the largest is $\lambda_1$, the necessary and sufficient condition is

$$
\boxed{\kappa<\frac4{(\Delta x)^2}\sin^2\left(\frac{\pi}{2(M+1)}\right).}
$$

Necessity follows by taking the first eigenvector as the initial data; at equality it remains unchanged. Sufficiency follows by decomposing any vector into the displayed decaying modes. The discrete [reaction-diffusion spectral decay threshold](../../../../../../reaction-diffusion-spectral-decay-threshold.md) is below $\pi^2$, since $\sin x<x$ for $x>0$, and equals $\pi^2-\pi^4h^2/12+O(h^4)$ as the mesh is refined. Therefore a coarse semidiscretization can spuriously grow for some parameters for which the continuous equation still decays.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
